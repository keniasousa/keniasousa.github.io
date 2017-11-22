---
layout: post
title: "What is the difference between flow charts and BPMN?"
date: 2014-10-01 16:57:26 +0200
categories: business business process modeling
---

I’ve been working with different projects and when we start modelling business processes, I’ve heard people calling them flowcharts. But, why are they calling processes flow charts? They are much more than just flow charts. How do I tell them that? OK, let me start from the foundation.

<b>What is a flow chart?</b> A flow chart is a type of diagram that graphically represents a process.  Hum, I’m also using diagrams to graphically represent processes.

<b>And am I doing flow charts?</b> When I’m modelling processes at a high-level (<a href="http://brsilver.com/three-levels-of-process-modeling-with-bpmn" onclick="javascript:pageTracker._trackPageview('/outbound/article/brsilver.com');" target="_blank">descriptive modelling</a>) and communicating it across the organisation, I’m definitely taking advantage of flowcharting. But I am using another notation, not flow charts. I use BPMN, (Business Process Model and Notation), a standard notation for business process modelling.

<b>What am I doing differently?</b> In flow charts, there are no set of agreed symbols. There are certainly commonly used symbols, but each one is free to create diagrams the way they see fit. Now, modelling business process with BPMN, I’m not worried that each model I come across in the organisation is using its own set of symbols (drawn in Visio, for instance). That, for one, makes it easier to compare models done across the organisation.

Here is an example of a business process using BPMN at a descriptive level:

<img src="/images/posts/bpm-analysis-initiate-project.png" class="bpm-analysis-initiate-project" alt="BPM Initiate Project">

<b>But am I going beyond flow charts?</b> First, with BPMN, I use more elements than those in a high-level flow chart (descriptive layer). I include more complex business process patterns, such as those with exceptions, decisions and events. With these models, I can create, among other things, detailed requirements for IT development. Second, with Aris Business Architect/Designer or another BPMS (Business Process Management Suite), I take advantage of a modelling repository, where I can reuse activities in different processes. Third, with enterprise architecture, I consider other organisational aspects beyond ordering of activities, such as related systems, resources allocation, indicators, etc.

<b>Anything else?</b> Flow charts have not evolved in terms of the notation, while BPMN is a notation defined by a group composed of companies highly engaged with the evolution of business process modelling. Using a standard like BPMN, you have a set of rules that are the foundation for modelling business process models understandable by a wider audience, rather than ad-hoc flow charts that lack an agreed set of modelling rules.
