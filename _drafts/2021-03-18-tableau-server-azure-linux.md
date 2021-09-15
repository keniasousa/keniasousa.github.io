---
layout: post
title: "Installing a server on the Cloud"
date: 2021-03-18 12:00:00 +0200
categories: tableau, cloud, server
---

![My dashboard published in Tableau Server](/images/posts/my-dashboard-tableau-server.png)

I have been doing data analytics for some time, focusing on the code side of duty, but recently I decided to dive in the intricate world of data backend. As a first experience I installed the Tableau Server on the Cloud to fell how hard it could be. It took a lot of reading, research and trials, but I got it done and now I want to share the steps I followed.

<!-- more -->

The reasons a company would want to install Tableau Server in the Cloud varies, but from start-ups to large corporations, moving to the cloud likely means:

- reduced operational costs since you pay as you go
- more efficient DIY infra-structure kind of thing
- responds to fluctuating demands by scaling out according to the market and user needs
- easier testing and learning before long term commitment

The process required persistence, but at the end it felt simple. I'm not sure about a production-ready installation, but straightforward steps like these can get the job done.

## In Microsoft Azure

1. Create a virtual machine in Microsoft Azure

Follow step 1 on this [page to Self-Deploy a Single Tableau Server on Microsoft Azure][self-deploy-Tableau-Server-Microsoft-Azure].

Make sure to go through all the items, when creating an inbound security rule, make sure to open the following default port for Tableau Server traffic: create one rule for the HTTPS service with the port 8850 used by the Tableau Services Manager. Information available on [Local firewall configuration][local-firewall-configuration].

2. Install the Tableau Server package

The instructions I used following the steps in this page to [Install Tableau Server and initialize Tableau Services Manager][server-linux-setup]

3. In the local folder, create a user with sudo access (with administrative access) to the computer where you want to install Tableau Server:

       $ mkdir ~/.ssh/username
       $ mv Downloads/username.pem ~/.ssh/username
       $ cd ~/.ssh/username
       $ chmod 400 username.pem
       $ mv username.pem ~/.ssh/username

4. Log in as a user with sudo access to the virtual machine where you want to install Tableau Server:

       $ ssh -i ~/.ssh/username/username.pem username@<ip_address_virtual_machine>

5. Download the Tableau Server .rpm or .deb installer package from the [Tableau Server Downloads and Release Notes page][download-tableau-server]. 

6. Navigate to the directory where you copied the .rpm or .deb package.

       $ cd ~/.ssh/username

7. In the server, use the package manager to install the Tableau Server package

       $ sudo apt-get update
       $ sudo apt-get upgrade
       $ sudo apt-get -y install gdebi-core

8. In the local machine, give permission to the user to access the virtual machine 

       $ scp -i ~/.ssh/username/username.pem tableau-server-<version>_amd64.deb username@<ip_address_virtual_machine>:/home/username

9. In the server, install the Tableau Server package

       $ sudo gdebi -n tableau-server-<version>_amd64.deb

## Initialize Tableau Services Manager (TSM)

10. Navigate to the scripts directory

       $ cd /opt/tableau/tableau_server/packages/scripts.<version_code>/

11. Start TSM 

You must include this parameter to accept the Tableau Server End User License Agreement (EULA). The EULA is available in the following location:
/opt/tableau/tableau_server/packages/docs.<version_code>/Commercial_EULA.txt

       $ sudo ./initialize-tsm --accepteula
                            
12. Set the password for my account to login in the Server

       $ sudo passwd username

13. Log off and log on again to the terminal before you configure Tableau Server. 

14. Activate and Register Tableau Server: 

I followed the steps using the [TSM web interface][activate-tableau-server]:

- Sign in to [Tableau Services Manager Web UI][sign-in-tsm-web-ui]
- On the Activate page, Enter or paste your product key and click Activate License
- When you’re finished activating product keys, click Next
- On the Register page, enter your information into the fields and click Register
 
## Configure Tableau Server

15. Configure initial server settings

I followed the steps using the [TSM web interface][configure-tableau-server] with local identity store.
Fill in the setup page and click on Initialize. 

16. Create an administrator account

Follow the steps on the page to [Add and Adminsitrator Account][add-admin-account]. I accessed the computer remotely and run the tabcmd initialuser command:

    $ tabcmd initialuser --server http://localhost --username 'tableau-admin' 

17. Access the Tableau Server

Visit https://<ip_address_virtual_machine>

18. Logon in the Tableau Server using the password for the user (in my case, user kenia) or administrator

## Access Tableau Server

18. After the Server is set up, the process to start the server is:

- Start the virtual machine in [Microsoft Azure][MS-Azure]
- Sign in [Tableau Services Manager][my-TSM]
- Click on Start the Tableau Server in TSM
- Access the [Tableau Server][my-TS]

19. When you are done, stop the Tableau Server:
- Click on Stop the Tableau Server in TSM
- Stop the virtual machine in [Microsoft Azure][MS-Azure]

There is no need to deactivate the license because a restart of the virtual machine will preserve the MAC address, as explained in this [Microsoft Developer Network Forum][static-MAC-addresses-Azure-VMs].

I'm ready to play and publish on my new Server!

[self-deploy-Tableau-Server-Microsoft-Azure]: https://help.tableau.com/current/server-linux/en-us/ts_azure_single_server.htm
[local-firewall-configuration]: https://help.tableau.com/v2020.4/server-linux/en-us/requ.htm
[download-tableau-server]: https://www.tableau.com/support/releases/server]
[activate-tableau-server]: https://help.tableau.com/v2020.4/server-linux/en-us/activate.htm
[sign-in-tsm-web-ui]: https://help.tableau.com/v2020.4/server-linux/en-us/sign_in_tsm.htm
[configure-tableau-server]: https://help.tableau.com/v2020.4/server-linux/en-us/config_general.htm
[add-admin-account]: https://help.tableau.com/v2020.4/server-linux/en-us/startup.htm
[static-MAC-addresses-Azure-VMs]: https://social.msdn.microsoft.com/Forums/en-US/598d14d3-0a07-4ae5-98f5-1ce03db102ee/fixedstatic-mac-addresses-for-azure-vms-for-software-licensing-reasons
[MS-Azure]: portal.azure.com 
[my-TSM]: https://<ip_address_virtual_machine>:8850
[my-TS]: https://<ip_address_virtual_machine>
