---
layout: post
title: "Business Process Overview"
date: 2017-12-14 23:55:21 +0200
categories: voluntary
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

<img src="/images/posts/VAC.png" alt="Value-Added-Chain">

This value added chain lists some primary and support processes of a company.
It doesn't explain too much, but at least it gives context.

### Which Activities do they do?

To move on with my reasoning, I will focus on the procurement process.

To start, I identified the main activities in a flow. At this stage, it is still
a high level list of activities to give a common
understanding of the process.

When you look at this diagram, it seems simple but the reality is that not
everyone has this knowledge. Even though it is basic, it provides a shared and
common understanding, limits scope and deepens the context for analyses.

### Who is involved?

When you see the process, you see activities, but none of them will be performed
without the process performers. Knowing the business roles assigned to business
process help identify which processes to focus on depending on the role you have
or on the actor you want to help.

<a href="/images/posts/BA-BP-macro-process-information-systems-stakeholders-procurement.png" target="_blank">
<img src="/images/posts/BA-BP-macro-process-information-systems-stakeholders-procurement.png" alt="Stakeholders"></a>

### Which systems support the process?

Let's pause going in further details for this process and talk about information systems.

I identified the supporting systems for each activity. Following [ArchiMate][archimate]{:target="_blank"},
I link two elements: business process with system software.

<a href="/images/posts/ArchiMate-BP-Sys.png" target="_blank"><img src="/images/posts/ArchiMate-BP-Sys.png" alt="ArchiMate"></a>

To determine an IT portfolio, I create a comprehensive list of the systems the company uses.
When aiming for business-IT alignment, a key step is to link systems to
processes at this high level in order to identify the purpose of
each system.

Some systems span across several processes and it is hard to quickly
identify its coverage. So, I created a relationship matrix to  
spot which processes are covered by each system.

<img src="/images/posts/Matrix-BP-Sys.png" alt="Matrix" target="_blank">

With this association, it is possible to detect if two or more systems serve the
same purpose. If this is the case, it deserves further analysis to identify if they offer similar
functionalities to avoid redundancy. Such a deep investigation is only possible if you start with this
basic structure.

### More details

It was good to have this overview, but I needed to add one more level of activities
because what was within each process was not clear for everyone.

At this stage of adding details to the processes, the procedures were very useful
to identify the main activities.

<a href="/images/posts/BA-BP-process-information-systems-procurement.png" target="_blank">
<img src="/images/posts/BA-BP-process-information-systems-procurement.png" alt="SubProcesses"></a>

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
[archimate]: http://www.archimate.nl/en/about_archimate/what_is_archimate.html
