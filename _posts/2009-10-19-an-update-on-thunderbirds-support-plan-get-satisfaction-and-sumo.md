---
id: 540
title: 'An update on Thunderbird&#8217;s support plan, Get Satisfaction and SUMO'
date: 2009-10-19T12:37:06+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/?p=538
permalink: /?p=540
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "540"
categories:
  - Mozilla
  - Thunderbird
---
[<img class="alignright" title="Avanti Marque (by drdad on Flickr)" src="http://farm4.static.flickr.com/3423/3945259239_931c37e078_m.jpg" alt="" width="240" height="180" />](http://www.flickr.com/photos/jonkleinman/3945259239)Since my last blog post about a position being available for support, I&#8217;m pleased to announce (belatedly) that we&#8217;ve hired Roland Tanglao to lead Mozilla Messaging support. It&#8217;s not obvious being the only person on staff supporting millions of users around the world!  In order to learn how Thunderbird support is currently happening, he&#8217;s been busy immersing himself in that world.

Success for anything user-facing on the scale of Mozilla Thunderbird requires scalable approaches.  One person, no matter how well qualified and efficient, can&#8217;t help everyone who may have issues (especially as many people come to us with questions that are really about their mail provider).  So we need to look to systems and communities to help us help users.

## Get Satisfaction

The first system that we&#8217;ve committed to is [Get Satisfaction](http://getsatisfaction.com/mozilla_messaging/), an online website which is designed from the ground up for peer-to-peer support.  You go there to ask a question, and maybe you also help someone else who has a question you know the answer to.  The &#8220;take a penny, leave a penny&#8221; model.

There are two things that stand out for me with Get Satisfaction: their user experience, and their APIs:

Get Satisfaction clearly thought long and hard about what the user experience of a support site should be like, and it shows: Threads are categorized as being ideas, problems, and praise, and problems and idea threads can be marked appropriately when either there&#8217;s an solid answer of some sort, or to track the evolution of ideas.  This provides people who want to dive into a support role with great dashboards, which makes dealing with a high volume much easier.  It also provides users a way to communicate their input & mood effectively, which is an important part of a support interaction.

The second aspect of Get Satisfaction that was particularly compelling to me was that they have built their system with HTTP APIs in mind from the beginning.  This means that we can integrate it into our own websites, or even in future versions of Thunderbird, without anyone needing to rework the database.  We&#8217;re just starting to figure out how to use these APIs, but I&#8217;m hopeful it will allow us to streamline support interactions considerably.

You can find out more about Roland&#8217;s thoughts about Get Satisfaction in his [blog post](http://blogs.mozillamessaging.com/roland/2009/09/30/get-satisfaction-25-months-in/).

## Knowledge Base

Even as we&#8217;re happy with the capabilities of Get Satisfaction, it&#8217;s clear we need to complement it with a knowledge base where we can build longer FAQs, helpful documents, etc. There, we got an unexpected assist from the Fennec (Mobile Firefox) project, as their need for a variant of [SUMO](http://support.mozilla.com/en-US/kb/) for Mobile users made it so that the SUMO project had to refactor and &#8220;productize&#8221; SUMO.  Having more than one installation of SUMO supported by the core SUMO team made me feel that our use cases were likely to be supported well, which is great &#8212; we try to leverage as much of the Firefox infrastructure as we can, as efficiently as we can.  Thanks Fennec!  (For now, we&#8217;ll stick with Get Satisfaction, and won&#8217;t be using the SUMO forums or the Live Chat features).

SUMO will allow us to build a scalable, localizable document store &#8212; it&#8217;s been proven to scale (handling 22 million hits a day for Firefox!), and has a built-in localization system.  Given that Thunderbird 3 will likely be published in 40 languages, ignoring localization isn&#8217;t a realistic option.  (I should point out that while GetSatisfaction is currently only in English, that team is keen to explore internationalization and localization).

For English users, [MozillaZine](http://forums.mozillazine.org/) is the obvious alternative to both Get Satisfaction and SUMO.  And indeed MozillaZine currently has lots of great content, and a bunch of people who provide great support.  Unfortunately, it also lacks a bunch of features (APIs and RSS feeds), has an interface which we can&#8217;t improve upon, and is English-only.  An interesting observation is that with people relying on search engines ever more, it&#8217;s not really a problem to have multiple sources of information about a product.  I expect MozillaZine will continue to thrive, and we&#8217;ll definitely continue to work with the all existing knowledge bases on the web and link to them appropriately.

## A web of communities

Going forward one of Roland&#8217;s tasks is to build or strengthen the bridges between Mozilla Messaging and the excellent Thunderbird related communities on the web. Mozillazine, of course, but also [geckozone](http://www.geckozone.org/) in France, and as many other support communities we can find.  Around the time of Thunderbird 3 launch (hopefully in November), Roland is planning some sort of worldwide support community online meeting. If you&#8217;re interested in participating, [contact Roland](http://blogs.mozillamessaging.com/roland/).

One of my hopes is that better organization of support communities can lead not just to happier users, but to a better product.  One of Roland&#8217;s duties is to provide feedback to the product development team on frequent or emerging issues faced by users, or areas of Thunderbird that particularly please people.  That&#8217;s not something he can summarize accurately by himself &#8212; he&#8217;ll need your help.

## Positive Feedback

Support is too often a one-way medium, with users complaining about problems.  That&#8217;s certainly an important function, but in a cooperative open source project, it&#8217;s equally critical that QA and developer contributors thank users for their input, and that users point out parts of the experience that they _like_, as positive feedback is the best motivator.  So take some time out and pick an open source project and generate some good karma!  For Thunderbird, it&#8217;s easy, go to [getsatisfaction](http://getsatisfaction.com/mozilla_messaging/) and click on &#8220;give praise&#8221;.  Roland will make sure that the people deserving of your praise get to see it.