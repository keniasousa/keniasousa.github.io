---
layout: post
title:  "Analysis of an Infographic"
date:   2017-03-12 22:31:55 +0100
categories: python
---


[Alberto Cairo's work][Graphics_Lies_Misleading_Visuals] entitled "Reflections
on the Challenges and Pitfalls of Evidence-Driven Visual Communication" presents
three ways that graphics can mislead the reader, which can be used as mechanisms
to analyse and detect issues in our own visual graphics:

- Hiding relevant data to highlight what benefits us: "cherry-picked"
statistics, e.g. show the average to hide that sales were negative in a certain
moment.
- Displaying too much data to obscure reality: extreme and unnecessary
detail, e.g. showing details that would be better explored with interactive tools,
not on a printed page.
- Using graphic forms in inappropriate ways: distorting the data,  e.g. truncate
Y-axis, hide where X-axis begins, inconsistent intervals in one of the axis, etc.

With examples, the author shows that these mistakes do mislead audiences and
creators of data visuals should aim to eliminate or, at least, minimize them.

Inspired by this work, I selected an infographic to analyse it according to
Cairo's mechanisms. This visual infographic describes the impact of US  and
World consumption on the availability of natural resources. It aims to show how
long some natural resources would last if the World consumption continues at
today's rate (from April 2007). This is compared to how long they would last if
the World consumed at half the US consumption rate (from April 2007).

The visual was found in the following URL by searching for the keywords
"cool infographics": [How long will it last infographics][how-long-will-it-last].

![infographics](/images/posts/26051202.jpg)

With further searches, the source image from New Scientist (science magazine)
can be found at: [New Scientist][newscientist]. But the original article from the
2605 issue of May 2007 cannot be accessed without subscription to the magazine.

The intended audience of the visual can be a wide range of people, including
scientists, geologists, ecologists, economists, statisticians, entrepreneurs,
environmentalists, and anyone interested on earth's natural resources.
I believe the audience is as wide because the infographics was displayed in a
popular science magazine that is sold online or on retail outlets to the general
public.

The components that I've found misleading in the visual are organised by the
mechanisms presented by Alberto Cairo's work:

- Hiding relevant data to highlight what benefits us

The visual does not show the data on World population consumption rate, which is
used in the calculations of how many years are left for the resources in the
graph presented in the middle. Hiding this information can be misleading because
the decoder is led to understand that the World consumption is smaller than the
US consumption. If the visual also showed a bar graph of the World population
consumption per capita, similar to the one on the left, the decoder could better
compare these consumptions.

- Displaying too much data to obscure reality

There are five data visuals presented:

1) bar graph on the left with US annual consumption;
2) small table on the bottom next to the bar graph;
3) circle graph in the middle that has the key information of the infographics;
4) proportion of consumption met by recycled materials;
5) population on April 2007 on the bottom right.

Showing these five data visuals in one infographics is misleading because it can
confuse the decoder with unclear links between them. For instance, what is the
relationship between number of years left for a resource (graph 3 in the middle)
and its proportion of consumption met by recycled materials (4 on the right) ?  
Another example: What is the relationship between the table (table 2 on the bottom)
and graph 3 in the middle? Is the data from the same source? In the table, the
element "Hafnium" will be exhausted in around 10 years, but there is no figure
available in the chart in the middle.

- Using graphic forms in inappropriate ways (distorting the data)

The bar graph on the left with US annual consumption uses a different scale, which
multiplies units by 10. It can be understood that this scale was used because
there is a big discrepancy between the resources being compared. But, in any case,
this scale is misleading to the understanding of the decoder who may end up
understanding that the difference in consumption is smaller than it actually is.
In addition, I could not tell if the scale in the circle graph in the middle is
consistent since there is no labelling.

Looking further into the effects of visual embellishments on understanding of charts, a very interesting article from CHI was recommended to me on [Useful Junk][useful_junk]. In this article, the main state of the art is on Edward Tufte to eliminate embellishments and on Nigel Holmes to encourage them. The authors report on their experiment results, which shows that there is no difference in interpretation accuracy between embellished and minimalist charts. However, embellished charts actually improved memorability after a gap longer than twelve days.

From my experience, I am in favour of the idea that pictures a worth a thousand words. I have faced this usefulness in my daily work with business processes and even more with statistics charts. Linking back to Cairo's work, my perspective is that the advantages of embellishments will only be powerful if they are truthful to accurately inform their audiences.

[Graphics_Lies_Misleading_Visuals]: http://infovis.fh-potsdam.de/readings/Cairo2015.pdf

[how-long-will-it-last]: http://www.coolinfographics.com/blog/2009/4/29/how-long-will-it-last.html

[newscientist]: https://www.newscientist.com/data/images/archive/2605/26051202.jpg

[useful_junk]: http://hci.usask.ca/uploads/173-pap0297-bateman.pdf
