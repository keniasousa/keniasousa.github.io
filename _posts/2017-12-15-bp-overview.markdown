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

### Who is involved?

Knowing who to contact is a question that kept on popping up. Mainly, people wanted to know:
who is the project manager of this
tool? Who is the product manager or the product owner? To answer them all at once,
I created a variation of this diagram with key stakeholders.

<a href="/images/posts/BA-BP-macro-process-information-systems-stakeholders-procurement.png" target="_blank">
<img src="/images/posts/BA-BP-macro-process-information-systems-stakeholders-procurement.png" alt="Stakeholders"></a>

### More details

On my talks to different people, they were very willing to talk about their
own tasks, so grouping them as a list of activities per process in alignment to
the procedures was not difficult, but time consuming.

<a href="/images/posts/BA-BP-process-information-systems-procurement.png" target="_blank">
<img src="/images/posts/BA-BP-process-information-systems-procurement.png" alt="SubProcesses"></a>

### Lessons learned

As I started showing these overviews, people put them on their office walls and
referenced them whenever they needed it.

I started taking these diagrams to every meeting and kept on taking
notes about what people mentioned. I took them to meetings anytime
people had questions and started using them at the beginning of requirements
elicitation to clarify the context and define the scope of discussions.

When I started, people warned me that the process was complex.
But that is yet another reason for doing these diagrams especially when someone
new arrives in the company or starts working with this process. From several
feedbacks, they appreciate to quickly get a bird's-eye view.

Getting the end-to-end overview of a process is no easy task. When you arrive in
a new company and everyone confirms they have it all in their minds, it doesn’t
mean that everyone has the same collective knowledge. From my experience,
it has definitely been worth the effort creating a visual representation tailored
to their needs. Next time I do this, it will probably be different to adapt to the
company's culture, but I already have a framework to direct my questions towards
an overall understanding.

[value-added-chain]: https://en.wikipedia.org/wiki/Value_chain
[archimate]: http://www.archimate.nl/en/about_archimate/what_is_archimate.html
