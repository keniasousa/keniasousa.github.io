---
layout: post
title: "Improving one problem at a time"
date: 2021-05-06 12:00:00 +0200
categories: lean six sigma, process improvement
---

Change is possible, but we've all seen processes with bottlenecks and waste that never change. When all goes smoothly, we operate in automatic mode. And as Daniel Kahneman stated, that's how our minds work most of the time and "constantly questioning our own thinking would be impossibly tedious". However, when we face a difficult situation, such as being blocked or making a mistake, we need to carefully analyze it to solve the problem. 

Last year, I volunteered with a mentorship program with a group of volunteers to manage the registration of participants. Following a manual process, we had to look up emails in a spreadsheet, assign mentors to mentees, verify who had signed up, send reminders, and track and report on registrations. Over the course of the 4-month program, it took 116 hours to manage assignments between participants, over 7 hours per week.

Clearly we needed to improve the process to register participants in order to increase the efficiency. To do that, our goal was to automate assigning mentors and mentees; sending reminders; and tracking invitation status.

In the manual process, all participants were asked to sign up in the tool. After each participant in a pair had signed up, the assignment was done manually based on the pair listed in a spreadsheet. In the automated process, the assignment is triggered by invitations. So, when a mentor invites a mentee and the mentee signs up, the assignment is done automatically. The automatic assignment via invitations removes the activities to look up participants, assign participants, verify status of assignments, update unmatched emails, and send reminders.

The automation of the assignment process will increase the efficiency of the program by removing repetitive manual tasks and improve transparency. The assignment via invitation will also increase the engagement of mentors who are the ones who trigger the beginning of this process. One consequence is the improved user experience because participants will no longer wait between sign up and access to steps because there are no longer manual tasks done between them.

By implementing this solution, we'll measure the improvements in the new program. But we can already see the impact on volunteers thinking of how we can occupy this free time to improve even more the program.

When we start solving problems, one after the other, to get closer to our objective, it puts us in the habit of improvement. This is a cycle known as Kaizen or continuous improvement.  At the heart of this cycle, there is a passion for learning that pushes us to keep this going.

++++++++++++++++++++++++++

**Project Name**: Manage the invitation of mentors and mentees in a mentorship program

Problem Statement: In 2020, the mentorship communications and technology teams managing 160 mentors and mentees spent time to look up emails of users in a spreadsheet, to assign mentors to mentees,  to verify who has signed up and send reminders, and to track and report on acceptance of invitations. Over the course of the 4-month program, it took 116 hours, over 7 hours per week, to manage assignments  between participants.


| Task | Time | Total|
|-------|--------|---------|
| look up emails of users in a spreadsheet  | 5 minutes per user for ~160 users |  13 hours |
| assign mentors to mentees  | 5 minutes per pair for 80 pairs | 7 hours |
| send reminders based on who has not signed up | 2 hours per week for 4 months | 32 hours |
| track and reports on assignments | 1 hour per week for 4 months | 16 hours |
| update unmatched emails between registration and the tool | 2 hours per week for 4 months | 32 hours |
| explain why users could not see steps without being  assigned to a mentor or mentee  | 1 hour per week for 4 months | 16 hours |
|   |  | 116 hours |


Scope: Assignment Process in the Mentorship Program

Out of Scope: communication with mentors and mentees beyond invitation and assignment.

Process Overview using SIPOC:

| Supplier | Input | Process| Outputs | Customers|
|-------|--------|---------|---------|---------|
| Mentorship Coordination  | List of mentees and mentors registered in the program |  Assignment | Invitation email sent from Mentorship to Mentors and from mentors to mentees |  Mentors and Mentees |
|  | |   | Tracking report of status of invitations |  Mentorship Program |

Activities in scope:
- Mentorship invites mentors
- Mentors invite mentees
- Send reminders to invited users
- Assign mentors and mentees

How will we know we succeeded:

Customer | Customer Needs | Quality Driver | CTQ|
|-------|-------|--------|---------|
|Mentorship Program|  Increase Efficiency  | Automated Services |  Mentors and mentees are assigned automatically 100% of cases |  
| |    |  |  Reminders are treated automatically for 90% of cases, excluding only escalations |  
| |    | Transparency |  Invitations status are automatically tracked 100% of cases | 
| |  Increase Engagement  | Ownership |  Mentors invite mentees 100% of cases|  
Mentor and Mentees|  Improve User Experience  | Timely access | No wait time between sign up and access to steps |


Objective: Automate the assignment process so that the mentorship program is more efficient, and mentors have a higher engagement in the program by triggering invites.

Teams and Responsibilities: 
- Communication Team: Define the content of the invitations and reminders, and test the features in the tracking tool.
- Technology Team: Develop the features in the tracking tool.
- Coordination / Tech and Communication teams: Test the features in the tracking tool and share training material.

The plan for the development is to have deliverables every 15 days:
- Mentorship invites mentors: May 10
- Mentors invite mentees: May 24
- Send reminders: June 7
- Create video on how to use the tool: Jun 21



