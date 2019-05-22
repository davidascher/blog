---
id: 372
title: 'Thoughts on Thunderbird&#8217;s Evolution'
date: 2008-01-03T17:55:16+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2008/01/03/thoughts-on-thunderbirds-evolution/
permalink: /?p=372
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "372"
categories:
  - MailCo
  - Mozilla
  - Thunderbird
---
Aside from all of the organizational stuff I&#8217;m doing like recruiting (more news soon I hope), dealing with the incorporation papers, budgeting, etc., I&#8217;ve been spending a lot of time thinking about Thunderbird&#8217;s evolution.

Specifically, how should we, as a project, figure out what to work on?

Some of my thinking about this hasn&#8217;t changed since I joined, but many of the details have, in reaction to talking to people on IRC, on the newsgroup, and, significantly, by watching a lot of bugmail.

First, a reality check. Thunderbird exists, today, and works, today, for large numbers of users, large numbers of use cases, against a variety of servers, in a huge array of different environments, from individual home users to massive organizational deployments. That&#8217;s a precious asset which I don&#8217;t want to either ignore or disrupt. So for example, any plans for Thunderbird evolution which start with &#8220;first, start over&#8221;, or &#8220;first, remove feature X&#8221; aren&#8217;t likely to go far.

Furthermore, there is an incredible store of community knowledge about known issues, good features to add, known architectural challenges, etc., which I&#8217;m slowly absorbing. And there is existing momentum there, with bugs being worked on daily, which I most certainly don&#8217;t want to stop. In the shortest term, all I&#8217;m likely to suggest are small course changes, although they&#8217;ll all be motivated by bigger picture motivations.

As an example of that kind of small influence, a little story: Mark Banner has been working on the Address Book for a long time. Joshua Cranmer, a more recent contributor, started to help out with a long-standing bug to convert the address book store from the &#8220;idiosyncratic&#8221; Mork database to the shiny new SQLite database now available. My contribution to that effort was to suggest in IRC that it&#8217;d be good to start with some unit tests, as changing backends without a test suite struck me as risky. A few days later, Mark had the beginnings of a test suite ready, that Joshua can use to move faster with the conversion. The bigger theme there is clearly that I believe we should build enough infrastructure such as test suites and test farms so that we can take on architectural changes with more confidence. That&#8217;s a theme you can expect to hear again. Much of the work that MailCo can do in the short term will be to help with setting up a context which is favorable to product evolution, so that people outside of MailCo find working on Thunderbird as rewarding an experience as possible. There are a surprising number of people who have tried to contribute to Thunderbird over the years, but there was no one with resources and the overall vantage point to help them help the project. (A related effort which I&#8217;m hoping to launch soon is to make it much, much easier for people to build, distribute, and install Thunderbird Extensions.)

There&#8217;s more to leading a project than making work safer or easier, though. Many people on the project would be happy to help move the project forward, if they only had a clear picture of where the project was going. Knowing about that long-term direction also makes it easier to figure out which of the existing feature enhancement requests (numbering over 1300 in bugzilla alone) fit in with the long-term vision for the project.

There&#8217;s a clear need for a long term vision, from which we can build a roadmap, taking into consideration the platform roadmap in particular. From that document we should be able to specify release goals, and then prioritize work items, identify areas needing contributor involvement, etc.

My approach to identifying this long term vision has been two-pronged. There are macro-level, contextual drivers, and there are micro-level, operational constraints. Understanding the current state of the project, is crucial to identifying what&#8217;s doable with a small paid staff and a lot of code, users, bugs, etc. On the flip side, the societal and market trends help us figure out where it&#8217;s _worth_ trying to take the project. For example, instant messaging use is now pervasive. Newsgroup usage is declining. All other things being equal (and they never are), I&#8217;m more likely to encourage IM integration than newsgroup tweaks. But it&#8217;s a balance, because we may have (as we do) existing code and contributors who care about NNTP (such as the aforementioned Joshua!), and I&#8217;m not about to stop them from fixing bugs!

Other high-level points which influence me and will influence the long-term vision:

  * Mozilla is unique in that among all of the &#8220;vendors&#8221; of messaging technology, it is the only organization driven by the public benefit. This should allow us to meet the user&#8217;s needs _directly_, without having to get distracted by exit strategies, analysts, etc. It also makes it easier to recruit volunteers!
  * Thunderbird has a unique position in the market due to its relationship with Firefox, the larger trends regarding open source adoption, and its technology base. The Mozilla platform&#8217;s extensibility capabilities are unparalleled, and this gives Thunderbird huge potential for fitting in &#8220;niches&#8221; that are hard for others to reach. 
  * The world of messaging has changed radically in the last decade, and not always for the better, from the user&#8217;s perspective. With increasing volume, spam, and diversity in communication modes, interacting via computers is getting more stressful, not less. From a product management perspective, there is &#8220;customer pain,&#8221; which means that there are problems to be solved. That&#8217;s a good thing!

In some ways, then, I&#8217;m forming a picture in my head which has a faraway, slightly fuzzy picture, of the Thunderbird that could be. And I&#8217;m also learning a lot daily about the Thunderbird that is. Interpolation is then just a small matter of design, architecture, coding, testing, inspiration, perspiration, patches, reviews, tests, parties, t-shirts, arguments, celebrations, conflicts, and conversations &#8212; lots of conversations&#8230;