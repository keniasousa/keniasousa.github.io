---
layout: post
title: "How to Roll Out Enterprise Architecture"
date: 2021-05-06 12:00:00 +0200
categories: lean, systems thinking, process improvement, customer, enterprise architecture 
---

![Network](/images/posts/connection.png)

Every company wants to give the best customer experience. But even when they offer usable applications, there are still broken links in that experience leaving their customers unsatisfied. How can we find what's wrong? Where do we start?

<!-- more -->

What happens sometimes is that each department has an efficient process but the gap lies in the communication between them. The reality is that companies already have some kind of representation of their processes, whether in text or in modeling tools. And when we try to connect the dots, we realize that each department uses different definitions and entities for the same meaning. For example, a participant of an education program wants to be identified as a person, not with different identifications whether this semester they are a student and the next they are a volunteer. 

So, before we are able to close the gap in the customer experience, we need to organize the people, processes and technology so that we are set up to create the best customer experience. An enterprise architecture creates a holistic view to increase transparency and makes it easier to identify the impact of changes across teams.

## Definition and Structure

There are different frameworks, tools and approaches for Enterprise Architecture and Business Architecture in they way they are structured. But in a nutshell, [Enterprise Architecture][ea-gartner] is usually seen as encompassing business architecture and it supports the enterprise to change and achieve the desired business vision. [Business Architecture][BA] primarily focuses on the business aspects and how they are linked. We can summarize them in domains and use them to define the structure of the organization:

1. **Business Architecture**: maps the business objectives, the business processes, the business functions, and the organization structure.

2. **Data Architecture**: defines data standards starting from business entities to the level of physical assets used in systems.

3. **Applications Architecture**: describes the application landscape that supports business processes, and how they interact with each other and with users.

## Linking the Views 

Each organization will define how these domains are connected and each business unit uses this so they understand each other and work in collaboration to achieve common goals.

You'll find I usually attempt to organize work in a series of steps to make it easier to follow so I can focus on the content. However, defining Enterprise Architecture is rather organic, it's more like making a puzzle. When we work on one piece, it points us to another one until we complete it. A few questions we can ask when we are defining the Enterprise Architecture are:

- **People**: are they supporting organizational goals, are the responsibilities reflected in the processes, are functions mapped to the organization structure, is the data shared between different functions, is terminology supporting good communication?

- **Processes**: do the activities help achieve the goals, have we identified how stakeholders, functions and business units collaborate, is there a common terminology across processes, is data accessible to understand, operate and improve processes?

- The **Technology**: which applications support key processes, which roles operate core applications, how does data flow across applications?

## Principles

It can seem overwhelming to take a systems thinking approach to Enterprise Architecture because it makes us think of defining how all parts interrelate to each other as part of the larger context they belong to. We can't help but think of documenting all aspects of our business and their relationships. One approach to help is to start small and operate through iterative cycles.

We can follow four principles:

1. **Simplicity**: _Prioritize focused on customers_

    According to the [Nature Human Behaviour Journal][Nature], as I learned from [Liane Davey][liane-davey], people have a bias that adding more things is strategic. But given the choice, the percentage of people choosing simplification strategies increases, which is good news to advocate for simplicity.

2. **Customer-centered**: _Observe what's happening to highlight problems_

    Understanding exactly what customers are going through helps understand limitations. The point is to base it on actual observation to get an accurate view of the situation. In lean, the Japanese word _Gemba_ is used to represent that we go in the actual place where the work is happening so we are able to understand the impact of the problem.

3. **Systems Thinking**: _Look at the overall picture and rely on relationships to help see the impact of changes_

    Business is an interconnected network with complex and dynamic interactions. Our goal is to see how changes in one place impact other areas and learn how to look beyond where the problem is occurring since it can be influenced by other areas.

4. **Lean**: _Iteratively test ways to solve problems in practice_

    Going through any change can be difficult but we can simplify this journey by embracing uncertainty and learning as we go. We don't know what we'll find out after we make improvements. That is the reason for experimenting and refining in practice in an iterative cycle so everyone learns by doing.

## Beyond the Surface

In some ways, Enterprise Architecture seems similar to weather forecasting to me:

- It needs a standard vocabulary describing key elements

- It needs to be broadcasted so people are aware and can take proper action

- There are many aspects that influence it and we need a scientific approach to make sense of it

- It needs to be measured to determine the success rate

- It assumes we take a holistic view, looking beyond just one location. Interesting to learn that it was only after the invention of the electric telegraph in the early 19th century that [weather forecasting][weather-forecasting] improved accuracy because it allowed reports from a wider region to be received and influence other areas almost instantaneously.

Enterprise Architecture is sometimes seen as a heavy approach when people try to focus on upfront modeling, on a paper exercise without trying it in practice and forget about the relationships between the domains. But what's worse for leaders is to face avoidable problems had we understood how our businesses are connected. Enterprise Architecture is seen as strategic for [change and innovation][ea-innovation] since it supports contextualized decision-making when we are faced with so many changes, especially as we are seeing it in society, businesses and customers.

How can all this help with the customer experience? To give the best customer experience a lot of things have to be aligned and work well behind the scenes. Everyone, every application and every product interacting with customers get prepared so they know what to do or how to operate when this time comes. But we cannot forget about the work that comes before and after that interaction. Again, they are all connected, the people using the technology and operating processes and their customers are part of the flow. When we change one of them, it could have an impact somewhere else and these links help us know where to look so we maintain it balanced. A transparent, connected and stable flow behind the scenes sets us up for successful customer experiences.

There are certainly other disciplines, approaches and techniques to explore. Teams have to choose the best approach, tools or a combination of those to support them in this journey. But as a foundation, it's important that team members are aligned. So when they need to decide which path to take, they know everyone will be based on the same set of principles.

[BA]: https://www.omg.org/bawg/business_architecture_overview.htm

[weather-forecasting]: https://www.bbc.com/news/magazine-32483678 

[Nature]: https://www.nature.com/articles/s41586-021-03380-y

[liane-davey]: https://www.lianedavey.com/why-youre-so-busy-and-how-to-ruthlessly-prioritize/

[ea-gartner]: https://www.gartner.com/en/information-technology/glossary/enterprise-architecture-ea 

[ea-innovation]: https://www.gartner.com/smarterwithgartner/enterprise-architecture-enables-digital-innovation/