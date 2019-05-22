---
id: 223
title: 'Yahoo&#8217;s UI library and the like'
date: 2006-11-17T15:44:48+00:00
author: David Ascher
layout: post


tags:
  - ""
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "223"
categories:
  - General
---
I&#8217;ve always had mixed feelings about Yahoo!.

I liked them in the earliest of days, when it was just a little directory of stuff on the www (as I remember calling it). I got fairly turned off when it became hugely successful, because of its &#8220;vibrant&#8221; esthetic and extremely commercial focus (ads everywhere!). I was curious when they acquired one of my favorite companies, Ludicorp/Flickr. I was scared when I saw Terry Semel present at Web 2.0, and he made it so clear what they saw as their role as an advertising company. I was impressed when I understood the diversity and richness of their business model (selling nikes for virtual avatars in online games? wow/sigh). I&#8217;ve somehow always felt slightly funny about their developer network promoting talks at technical conferences (not sure why!). When they bought good companies, the people behind them seemed to disappear behind the firewall. So, overall, wary.

This last little while I&#8217;ve been very impressed with what they&#8217;re doing on the web development front. Their [YUI library](http://developer.yahoo.com/yui/) is _nice_. Publishing and maintaining CSS stylesheets to help cross-browser design is a thoughtful touch. Their [cheatsheets](http://developer.yahoo.com/yui/#cheatsheets) are an elegant combination of thoughtful content, smart page layout, and beautiful design (I immediately printed them and pasted them into my new notebook, only to have them be made obsolete the next day with a new release&#8230;). Their design patterns collection is a Good Thing for the web. I&#8217;m looking forward to playing with YUI more.

I had a hard time admitting how good YUI was because of cognitive dissonance &#8212; For a while now I&#8217;ve been a fan & promoter of the Dojo Toolkit, which was the first toolkit I ran into which took both JavaScript and software engineering seriously. Dojo&#8217;s scope is bigger than YUI&#8217;s current scope, but it suffers from a lot of the usual challenges of open source projects: engineering is valued more than polish, there&#8217;s not enough attention paid to graphic design, and it&#8217;s tough to do effective product & project management when all you have are volunteers. There are still bits of Dojo that YUI doesn&#8217;t seem to compete with, such as the dojo.storage offline storage wonder, the undo management infrastructure, the exciting-if-it-really-works dojo.gfx graphics layer. Still, it must be disheartening for the Dojo folks to compete head-to-head with a company with the resources of Yahoo.

Luckily, as a user, neither I nor anyone else needs to pick one or the other (plug: Komodo 4 will ship with built-in support for both, among others!). With some caveats, it should be possible to cherry-pick the bits from these or other toolkits (yes, I know, prototype.js-based toolkits don&#8217;t play well with others often).

Now if someone could figure out how to make flash plugins play well with the event system, we&#8217;d really be onto something&#8230;