---
layout: post
title:  "Growing Through Freemium"
date:   2016-03-18 16:57:51
---

<b>Background</b>

As I outlined in my <a href="http://nickgottlieb.com/2016/03/05/growth-at-a-startup/">last post</a>, the first big pricing change we made while I was at CircleCI was to implement a simple pricing model where the first container cost $19/month and each additional container was $50/month. 

Immediately after making this change our growth focus shifted to upgrades. I created a metric called upgrade velocity (number of months a customer has been using the service divided by the number of additional containers they have purchased) and ran a lot of experiments aimed at driving this number. Many of these were focused on encouraging users to take advantage of certain features that not only allowed them to get more value out of the product, but also allowed them to utilize more containers.

Once certain strategies had been validated and implemented, and the upgrade velocity increased significantly, we turned our attention to strategies that would put more users in to the top of the funnel. One high-impact strategy for doing this was to give the first container away for free, doing away with our 14-day free trial model and moving to a freemium pricing model.

<b>What were the concerns?</b>

There are of course concerns and risks with giving away your product for free. For us, the first concern was the potential revenue that we would lose from both current and future customers.

We began by taking a look at the potential revenue impact on future users. Of course if we  charge $0/month rather than $19/month for the the first container, we're going to be making a lot less money, but  we wanted to get an idea of what the impact would be 6-months in to a customer's life cycle. 

Say we were signing up 100 new users per month, and that by switching to a freemium model we would be able to sign up 300 new users per month (we actually did run a freemium test on our site and were able to increase sign ups by almost 3X). We knew from looking at our historical data that the average customer's upgrade velocity (number of months since sign up divided by number of additional containers purchased) is .5 over the first 6 months. So if we look 6 months down the road, the average customer who signed up for one container will be using 4. Here is an equation that helped us compare potential revenue 6 months from now:
 

sign ups * (initial monthly spend + ((6 * upgrade velocity) * 50)) =  cohort revenue in month 6

100 * ($19+(3*50)) = 16,900

300 * ($0+(3*50)) = 45,000

 
While this particular equation is simplified and glosses over things like customer churn, users vs. accounts, and the difference in the types of users a free product might attract, it did serve as a good heuristic. It showed that if we could maintain anywhere near the same upgrade velocity for our freemium customers as had had previously the overall revenue growth would be substantial.

The second number we were concerned with was the revenue lost from current customers. We believed strongly in fair pricing, and we certainly didn't want to charge existing customers more than new customers, but if we stopped charging all of our current customers for their first container we would lose a significant amount of revenue (number of paying customers multiplied by $19/month).

Instead of doing this, we tested out an alternative. We gave a small subset of paying customers an additional container for free, so their current monthly spend would remain the same but they would have an additional container. They had the option of manually lowering their plan by one container (and getting $19/month off their bill), but only ~15% of customers actually did that. It seemed that the majority of customers got more than a $19/month value from that extra container! While this would result in a hit to our margins it was a much smaller hit to our revenue and we decided it was our best option.

The last cost that we were concerned with, and the most difficult to test, was the cost of supporting a lot more customers, many of whom would not be paying. At this point in our scaling efforts we were already having significant problems with support, and there was real internal anxiety about potentially exacerbating this with freemium. We eventually came to a compromise: we would hire two support engineers to help alleviate the additional support load and we would have a contingency plan to limit support for free customers if the load became unbearable. 

<b>Results</b>

Once the decision was made, the code was shipped, and the <a href="https://circleci.com/blog/continuous-integration-and-deployment-on-circleci-just-got-better-now-its-free/
" target="_blank">announcement was made</a>, we began to watch the data. For the most part, things went as we expected. We had <b>a lot</b> more sign-ups, a lot more people in support, and within a couple months a lot more revenue. We did have one interesting and completely unexpected cost: there was a group of users that began using our free containers to mine bitcoin. It took our engineering team a couple of weeks to realize exactly what was going on, and once they did they were able to quickly put a stop to it, but it goes to show that there will always be unanticipated consequence to any product decision. 




