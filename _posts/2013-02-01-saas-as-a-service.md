---
id: 738
title: SaaS as a Service?
date: 2013-02-01T16:08:47+00:00
author: David Ascher
layout: post
guid: http://blog.ascher.ca/?p=738
permalink: /?p=738
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "738"
categories:
  - Business
---
If you haven&#8217;t been paying attention (and really, most people shouldn&#8217;t), there&#8217;s what feels like a real trend where startups are breaking down common tasks for web & app development, and solving them through a software-as-a-service model. So, in no particular order, you can see

  * stripe doing payments 
  * disqus doing commenting 
  * firebase, pusher doing lightweight data & realtime updates 
  * newrelic is doing deep resource tracking 
  * geckoboard is doing dashboards
  * heroku is doing processs/service hosting, relying on a bevy of partners including many of the above for slices of value
  * …

There are lots and lots (and lots!) of new entrants that are following this paradigm, and from a developer&#8217;s point of view it&#8217;s both exciting and daunting. 

Exciting because in the right combination, these services can be combined to deliver incredible scale and agility even to very, very small teams. (I have a fantasy of someday figuring out how large a 10-person project can be. It&#8217;s pretty large).

Daunting as well, because while when they can work well together in an app, they really should be thought of as independently moving (and failing) parts. And you&#8217;re likely not going to understand them as well as you should, or as you would had you built them yourself.

Which leads me to a friday-afternoon prediction: that there will be, over the next few years, a few companies who become experts at solving the coordination problems that arise from assembling so many disparate slices of value into an offering (whether for developers, or clients, or internally). And I expect that this expertise may not be purely technological.

I&#8217;ve seen how deep one has to go to get a real understanding of the security and privacy implications of relying on a third party for handling user data; I&#8217;ve seen the horrendous chain of dependencies that emerge out of security vulnerabilities; I&#8217;ve gotten a glimpse at the regulatory issues which some (soon more) folks will have to face. Dealing with high availability, geo-distribution, etc. all result in systems whose complexity scales in scary ways.

This leads to two thoughts:

  * If I were a wise investor, I&#8217;d look for those folks who look like they&#8217;ll find ways to integrate value in coherent larger slices, or mitigate the pain. 
      * As a &#8220;product person&#8221;, I probably want to work on problems that require only a few slices, done well. </ul> 
        Said like that, I do get a &#8220;nothing new under the sun&#8221; feeling. Oh well, it&#8217;s Friday. MFBT.