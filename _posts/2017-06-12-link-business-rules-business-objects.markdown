---
layout: post
title: "How to link Business Rules with Business Objects"
date: 2017-06-12 10:39:07 +0200
categories: business business process business rules enterprise architecture enterprise systems it
---

As I look into linking the business layer with other perspectives in enterprise architecture, the following question came to me: “How do I link business rules with business processes, business objects and even with data objects?”

Inspired by <a href="https://www.linkedin.com/pulse/modelling-business-rules-using-archimate-language-antonio-plais?trk=v-feed&amp;lipi=urn%3Ali%3Apage%3Ad_flagship3_feed%3B5D%2B5txRDXKvj4rf1vbtlDw%3D%3D" onclick="javascript:pageTracker._trackPageview('/outbound/article/www.linkedin.com');" target="_blank">this article from Antonio Plais</a> on business rules,  I have looked in depth into <a href="http://www.opengroup.org/subjectareas/enterprise/archimate-overview" onclick="javascript:pageTracker._trackPageview('/outbound/article/www.opengroup.org');" target="_blank">ArchiMate Enterprise Architecture Modeling Language</a> (<a href="http://pubs.opengroup.org/architecture/archimate3-doc/" onclick="javascript:pageTracker._trackPageview('/outbound/article/pubs.opengroup.org');" target="_blank">ArchiMate 3.0 specification</a>). I illustrate what I have learned by relating elements from three different layers from Enterprise Architecture, namely, Business Layer, Motivation Layer and Application Layer. The following diagram shows an overall view of element types in these layers using <a href="http://www.sparxsystems.com/products/ea/index.html" onclick="javascript:pageTracker._trackPageview('/outbound/article/www.sparxsystems.com');" target="_blank">Sparx Systems’ Enterprise Architect</a>:

<!-- more -->

<a href="http://usi4biz.com/2017/06/12/how-to-link-business-rules-with-business-objects/business-layer-overall/" rel="attachment wp-att-750">![business-layer-overall.png](/images/posts/business-layer-overall.png)</a>

### <strong>Business Layer</strong>

Let’s start by defining the business processes and the related business objects. The relationship from a Business Process to a Business Object are:

<ul>
<li>access: a type of dependency relationship that indicates that a process acts upon (e.g. read, update, delete) an object.</li>
<li>association: an unspecified relationship between any two elements.</li>
</ul>
The following diagram shows the Business Layer with the Business Process ‘Create Recipe’ that creates the ‘Recipe’ business object using the access relationship.

<a href="http://usi4biz.com/2017/06/12/how-to-link-business-rules-with-business-objects/business-layer/" rel="attachment wp-att-743">![business-layer.png](/images/posts/business-layer.png)</a>

### <strong>Motivation Layer</strong>

The Motivation layer in ArchiMate represents the reasons that guide the solution. Adding motivational concepts from this layer, I use a Requirement element to represent business requirements.

The possible relationships from a business process, business object or data object to a requirement are:

<ul>
<li>realisation: a structural relationship that indicates that one element plays a critical role in the operation of another element.</li>
<li>influence: a type of dependency relationship that indicates that a element affects the other element (e.g. positively, negatively).</li>
<li>association: an unspecified relationship between any two elements.</li>
</ul>
On the other hand, the relationship possible from a requirement to a business process, business object or data object is <em>association</em>.

From these options, I selected <em>realisation</em> due to its stronger meaning to demonstrate that one element realises the other, in this case, a business process realises a requirement. The others relationships were not selected because association is generic and influence is the weakest type of dependency. The ArchiMate specification mentions: “For weaker types of contribution to the realization of an element, the influence relationship should be used” (section 5.1.4. Realisation relationship). In addition, the <i>influence</i> was created to link motivational elements, specific to Archimate, which are not in UML. Thus, the realisation seems the best suit for this case.

The following diagram shows the business process ‘Create Recipe’ and the business object ‘Recipe’ realising the requirement ‘Possibility to update portions’.

<a href="http://usi4biz.com/2017/06/12/how-to-link-business-rules-with-business-objects/business-layer-cs/" rel="attachment wp-att-747">![business-layer-cs.png](/images/posts/business-layer-cs.png)</a>

According to ArchiMate, a <strong>business rule is a specialisation of a requirement</strong>. There is no specific element to represent business rules in ArchiMate. But, we could use the same element as from requirement. However, in a context where there are already business rules, a businessRule element can be used to make an specialisation of the requirement element.

<a href="http://usi4biz.com/2017/06/12/how-to-link-business-rules-with-business-objects/business-layer-brule-cs/" rel="attachment wp-att-748">![business-layer-brule-cs.png](/images/posts/business-layer-brule-cs.png)</a>

### <strong>Application Layer</strong>

Going to the application layer, the relationship between data object (application layer) and business object  (business layer) is <i>realisation</i>.

Considering a business rule as a specialisation of a requirement, the relationship of a data object to the business rule is a <em>realisation</em>, following the same reasoning for relationships towards requirements.

The data object ‘Recipe’ realises the business object ‘Recipe’ and the business rule ‘Update portion of ingredients’. The user can increase, decrease portions and reset to original portion.

<a href="http://usi4biz.com/2017/06/12/how-to-link-business-rules-with-business-objects/business-layer-brule-busobj-cs/" rel="attachment wp-att-749">![business-layer-brule-busobj-cs.png](/images/posts/business-layer-brule-busobj-cs.png)</a>

 
