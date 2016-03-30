---
layout: post
title:  "SaaS Pricing as a Growth Lever"
date:   2016-03-11 16:57:51
---


**Starting Point**

In 2014 the company I was managing growth for, CircleCI, offered a classic 3-tiered pricing model. Our pricing page looked something like this:

<img src="{{ site.baseurl }}/assets/img/pricing-sketch.png">

It's not important to understand how our product works, just that it's a SaaS service that helps software developers ship their products faster. To do this we sell containers, which are used on software projects, and parallelism is a feature that allows containers to be used in different ways. 


The original goal when this model was designed was to allow people to self-select in to the most expensive plan that they were willing to pay for. A team with multiple projects didn't cost us more, but we figured they were getting more value from the product and hence were willing to pay more. This is a classic pricing structure for SaaS products and you see it all the time.

This pricing model seemed to be serving us well, we were growing at a very healthy rate, but we regularly had people come in to support who were confused by it. They were mostly confused by how upgrades (i.e. purchasing more containers) affected their plan. Could they purchase additional containers with the solo plan? If they did would they get access to multiple projects and parallelism? Did they need to switch plans before adding containers? These were questions that we got more and more often as we expanded our customer base. 

Having empaty for your users means thinking about their complete experience with your product, not just the core features that deliver value to them. The purchasing experience is an often overlooked but extrememly important part of any product, especially for SaaS products. Your product can solve a serious problem, be delightful to use, and extrememly valuable to the user, but if the purchasing experience is poor you will have more dissastisified users paying you less money. There was clearly a product growth opportunity here so I decided to totally reevaluate our pricing model.


**Reevaluating**

I started by taking a dive in to both our customer data and customer support conversations (both of which were stored in <a href="https://www.intercom.io" target="_blank">Intercom</a>). The first thing I discovered was that most of our best customers weren't actually getting any value from being able to use containers on multiple projects. In fact, almost all of our highest paying customers had large monolithic application that consisted of only a single project.

The second thing I discovered was that we generated much more revenue from upgrades than we did from initial signups, and the use of our parallelism feature tended to dramatically drive these upgrades. As soon as customers started to use parallelism they would purchase additional containers at a rate of over 2X what customers who weren't using parallelism would (which makes sense because parallelism makes it easier to use multiple containers at once). 

These two discoveries made it clear that using the number of projects and parallelism as pricing mechanisms was wrong. It also made it clear that driving the use of parallelism should be a growth goal, and the first easy step is doing that was to make it free.

The new pricing we released was very simple: the first container is $19/month and each container after that is $50/month. We still offered a couple starting points but they all followed the same simple formula. Below is what our new pricing looked like and <a href="http://blog.circleci.com/simple-and-transparent-pricing/" target="_blank">this is the announcement we made to our customers</a>. 

<img src="{{ site.baseurl }}/assets/img/pricing.png">

The new pricing resulted in an increase in sign ups and an even bigger increase in additional containers purchased.  

One question this pricing model begs is 'why is the first container only $19 while all additional ones are $50?' The answer is that we wanted to make it easier for users to start using the product so that they could start purchasing containers. Why not just give the first container away for free then? Well that's eventually exactly what we did and what my next post is about.

