---
id: 577
title: Maturation of the hosting provider market
date: 2010-10-04T21:47:04+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "577"
categories:
  - Computing
---
I&#8217;ve been considering switching hosting providers for a little while, as my current provider, while cheap, has been slower and slower, making me think that they&#8217;re not managing their hosts super well.  And I figured it&#8217;d be good to get a feel for how that part of the market has evolved.

A tweet and some link-following later, I&#8217;ve come to a few tentative conclusions:

First, like everything else in the computer world, the capacities have gone up, but the price points haven&#8217;t changed drastically in the years since I setup ascher.ca.  The dirt-cheap providers are a few dollars cheaper than before (e.g. [Laughing Squid](http://laughingsquid.us/)), but most low-end VPS offerings are $15-20/month &#8212; they&#8217;re just bigger defaults than before.

Second, there&#8217;s clearly interesting competition to reach out to l33t developers.  [Dreamhost](http://www.dreamhost.com), [Media Temple (aka (mt))](http://www.mediatemple.net), [Slicehost](http://slicehost.com), etc. have been around for a while, and they seem to be doing fine, with many positive reviews to be found. All of these providers claim to be developers building a company for other developers, and their success clearly depends on that being a believable story.

Third, running your own VM is still a complicated business, requiring knowledge of Linux (absolutely no mention of any other OS, btw), configuration, system administration, security, etc.  That&#8217;s been true forever, and I&#8217;m seeing some interesting attempts by some to differentiate in what must be a horrible race-to-the-bottom margin-cutting segment.  In particular, I noticed:

  * Linode highlights their community, their library of useful docs, and their [StackScripts](http://www.linode.com/stackscripts/), which could help automate setting up services on stock OSes (although I&#8217;d really want to see some security reviews on those scripts, which could easily p0wn the gullible).
  * [No.de](https://no.de/) (from our friends at Joyent) isn&#8217;t a general purpose VPS, but has evolved the Smart platform into a node-led system which also includes various [databases](http://wiki.joyent.com/node:faq). I&#8217;ve played with no.de a bit, and automated deployment via-git-push could get really addictive.
  * Webbynode has a command-line rapid application deployment tool, which clearly has a Rails history, but is branching out into Django and [Node](http://guides.webbynode.com/articles/rapidapps/nodejs.html).  They also have an interesting github integration model where you point it to a github repo for both source and configuration of a package.

Overall, it&#8217;s good to see some innovation higher up in the stack.  I haven&#8217;t decided who&#8217;ll get my account yet, but I&#8217;m likely to spend a few more dollars and subsidize someone who&#8217;s focusing on making my life easier, not just racing to the bottom.