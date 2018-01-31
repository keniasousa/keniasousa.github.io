---
layout: post
title: "Business Process Overview"
date: 2018-01-31 23:55:21 +0200
categories: business process
---

When starting to work with a new process,
you try to grasp everything as you read procedures and listen attentively to
people when they talk about their tasks.
But getting an understanding is a challenge
because procedures are detailed and links between them
are unclear. Also, some people work so intricately on their tasks that it is hard
to get an outline.

So, how can I help people create a process that is clear from the first look?

<!-- more -->

One effective approach is not to overload people with too many details at first. Rather, to provide
gradual refinements that represent complementary ways to see processes.
I have applied a layered approach that starts with the overview of processes and then decomposes
them by adding more details to help people gain information in a series of layers.

### Which Processes run here?

Before you start looking at any given process, you first need to know
what the company does.
One first common concept coming to mind is the one of Added Value Chains:
a set of activities a company does to create products or services.

From [Porter's generic value chain][value-added-chain]{:target="_blank"},
I created a diagram listing key processes.

<img src="/images/posts/overview.png" alt="Value-Added-Chain">

This value added chain lists some primary and support processes of a company.
It doesn't explain too much, but it gives context.

What does it mean to give context? Say you work with preparing calls for tenders, evaluating proposals and managing contracts. For you, that is at the heart of your daily tasks and it is key to the functioning of the enterprise. When you do procurement in the construction industry, once the contract is signed, for a construction project to be successful there are many other considerations, such as the logistics in transporting material from the fabrication to the project site in a timely manner. This is where context helps, it puts one part into perspective considering the entire structure and shows the importance of interrelations for everything to work.

### Which Activities do they do?

To move on with my reasoning, I will focus on the procurement process.

To start, I identified the main activities in a flow. At this stage, it is still
a high level list of activities to give a common
understanding of the process.

When you look at this diagram, it seems simple but the reality is that not
everyone has this knowledge. Even though it is basic, it provides a shared and
common understanding, limits scope and deepens the context for analyses.

<img src="/images/posts/bp-overview.png" alt="Activities">

### Which systems support the process?

Let's pause going in further details for this process and talk about information systems.

<a href="/images/posts/ArchiMate-BP-Sys.png" target="_blank"><img src="/images/posts/ArchiMate-BP-Sys.png" alt="ArchiMate"></a>

To determine an IT portfolio, I create a comprehensive list of the systems the company uses.
When aiming for business-IT alignment, a key step is to link systems to
processes at this high level in order to identify the purpose of
each system.

<a href="/images/posts/bp-overview-systems.png" target="_blank"><img src="/images/posts/bp-overview-systems.png" alt="ArchiMate"></a>

### Who participates?

Interactions between people is key to the success of any process. Acknowledging that there are other people in the process, that my behavior influences them and consequently the result produced is a first step to broaden your point of view.

This is a simple conversation diagram that shows only two participants and the messages they exchange. You can see which flows require communication with people outside the organization, such as asking for tender offers. You also see that the evaluation of offers happen within the organization since only the result is notified to the contractor. To go further, you could create a variation to show how the legal and financial departments and external experts communicate during offer evaluation.

### More details

It was good to have this overview, but I needed to add one more level of activities
because what was within each process was not clear for everyone.

At this stage of adding details to the processes, the procedures were very useful
to identify the main activities.

Here is an example of adding one more level of activity for one of the sub-processes.

<a href="/images/posts/bp-overview-sub-process.png" target="_blank">
<img src="/images/posts/bp-overview-sub-process.png" alt="SubProcesses"></a>

One interesting strategy when adding details to your process is to select a view
depending on the situation. For instance, if you have a meeting to discuss the
"Planning" process, use this image. If you need to discuss how to deal with contracts,
you could expand the last three sub-processes. The idea is not to overload people
with so many information that they would get distracted and overwhelmed. The goal
is to make it simple, to show details only when they are needed.

Any other detail you may feel compelled to present early on should deserve further
analysis. What we have to keep in mind at this stage is that any deeper investigation
is only possible if you start with this basic structure.

### Lessons learned

The main benefit from these diagrams was to create a collective knowledge.
As knowledge is shared, the impact can go further than you expect.
As a business analyst, I took these diagrams to every meeting and used them to clarify the context and
define the scope for requirements elicitation. When new people arrive in the
company or someone starts working with a new process, they use it to quickly
get a bird's-eye view. Policy writers used them to organize
the sequence of tasks in their procedures and interlink them to procedures of
other departments. Project managers used them to group and prioritize requirements.
Auditors used them as a guide so they don't forget any phase.
Senior managers finally saw which processes they had to focus on if they wanted
to satisfy their customers. With time, we could see these diagrams
on their office walls.

It is challenging to create an overview when a process is complex, procedures
are disconnected, and people do not have a shared understanding.
Despite the difficulties, it is especially important to create these diagrams.
When you create the overview of a process,
you help people create a mental model that helps them get a concrete grasp of the
reality that, otherwise, was dispersed and unknown.

[value-added-chain]: https://en.wikipedia.org/wiki/Value_chain
