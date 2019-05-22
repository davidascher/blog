---
id: 280
title: Priorities
date: 2007-05-16T22:38:36+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2007/05/16/priorities/
permalink: /?p=280
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "280"
categories:
  - Mozilla
---
The Mozilla world is abuzz with emotional statements about the fate of XULRunner, the technology stack Firefox is built on, in particular as a reaction to [Mitchell Baker&#8217;s post](http://weblogs.mozillazine.org/mitchell/archives/2007/05/xul_and_xulrunner_investment.html) on the topic, and [Chris Messina&#8217;s video rant](http://www.viddler.com/explore/factoryjoe/videos/1/).

[Gerv Markham](http://weblogs.mozillazine.org/gerv/archives/2007/05/dinner_with_chris_messina.html) has a great point I&#8217;d like to riff on:

> &#8230; there&#8217;s one misunderstanding that I think underlies a lot of what he [Chris Messina] said, which is that he suggested that we are paying too much attention to the browser instead of the platform. But that&#8217;s a false dichotomy &#8211; the browser (and the open web) is the platform. Others are far more qualified to comment on this than me, but which is more likely to succeed &#8211; if we go up against Silverlight, Flex and JavaFX with XUL, as just one more competitor in a group of single-vendor solutions, or if we go up against them with the Web &#8211; HTML5, JavaScript, CSS, canvas, SVG, Ogg and open standards? 

Whether &#8220;the open web is the platform&#8221; or &#8220;xulrunner is the platform&#8221; depends on what fight you&#8217;re in for. If your aim is primarily to build a platform for &#8220;rich internet applications&#8221;, then, sure, XULRunner (XR for short) could be turned into a &#8220;contender&#8221; of a platform. From a technical point of view, the XR stack is a pretty decent cross-browser development framework, in the sense that people can and do ship great apps built on that stack. People keep mentioning the recent entrants Joost and Songbird, but we&#8217;ve been [doing it](http://activestate.com/products/komodo_edit/features.plex) for for the larger half of a _decade_ (see [this](http://activestate.com/company/newsroom/press/2000_05_24_1) quaint release from eons past). It can be done. Today.

In terms of making XR a contender for a much broader class of users, I&#8217;m sure that the folks at Joost and Songbird would agree with me that there&#8217;s a lot of work to be done! To make XR as appealing for RIA developers as Flex/Apollo or Silverlight, you&#8217;d have to solve two very different classes of problems. The first are nice juicy coding challenges, like a faster runtime, a sexier graphics framework, etc. The second is that for an RIA platform to be compelling, it has to be _already installed on virtually all target systems_, automatically updated/patched, versioned properly, security-audited, well documented, etc. Those are hard problems which take years of slow market penetration, constant massive investment, and aggressive channel management to build. Macrodobe is there with the Flash installed base after years of taking one beach at a time, thanks to regular folks&#8217; passion for games and tolerance for ads. Microsoft is there thanks to, well, owning the dominant operating system. Mozilla is nowhere near that, and it won&#8217;t get there until Firefox is much more widely deployed than it currently is.

However. Even if the features were implemented, and the distribution challenge were solved&#8230; Making an RIA platform is not what&#8217;s driving Mozilla. That, as hard as it is, is too modest a goal. Mozilla has signed up for a bigger fight, described in the [Mozilla Manifesto](http://www.mozilla.org/about/mozilla-manifesto.html), which people don&#8217;t talk about as much as they should. I&#8217;ll repeat the Principles section here:

  1. The Internet is an integral part of modern life–a key component in education, communication, collaboration, business, entertainment and society as a whole.
  2. The Internet is a global public resource that must remain open and accessible.
  3. The Internet should enrich the lives of individual human beings.
  4. Individuals&#8217; security on the Internet is fundamental and cannot be treated as optional.
  5. Individuals must have the ability to shape their own experiences on the Internet.
  6. The effectiveness of the Internet as a public resource depends upon interoperability (protocols, data formats, content), innovation and decentralized participation worldwide.
  7. Free and open source software promotes the development of the Internet as a public resource.
  8. Transparent community-based processes promote participation, accountability, and trust.
  9. Commercial involvement in the development of the Internet brings many benefits; a balance between commercial goals and public benefit is critical.
 10. Magnifying the public benefit aspects of the Internet is an important goal, worthy of time, attention and commitment. 

Ensuring the health of these principles is Mozilla&#8217;s driving force. I like these principles. They concisely state why I have learned to care about the Internet and its human-readable face (the web) ever more deeply over the years.

Notice the absence of any mention of RIAs. Notice the number of times the Internet is mentioned.

This fight that Mozilla signed up for is not about fighting over the _profitable_ ivory tower of RIAs (as sexy and glossy as it is), but watching out for the much bigger, messier, and more _valuable_, Greater Web.

To win that fight, it&#8217;s not as important to come up with an offline model for XUL apps as it is to come up with an offline model for plain old web pages. It&#8217;s not as important to come up with glossy effects for dialogs as it is to enable the creation of web content that can be seen in a choice of standards compliant browsers competing for users. It&#8217;s not as important to optimize the runtime for XUL apps as it is to optimize the runtime for random web pages. Luckily, there will be overlap with the needs of RIA developers. In particular, getting Firefox ever more _out there_ will, over time, allow for a XUL-based RIA story.

Solving the RIA problem can make a company money. Solving the problems of internet apps, whether &#8220;rich&#8221; or poor, can change the world. Microsoft and Adobe in particular will make lots of money building out RIA platforms and selling them to intranet developers everywhere. But, hopefully, most people won&#8217;t be that affected. They&#8217;ll be too busy posting on Craigslist, editing Wikipedia, doing all kinds of technologically &#8220;simple&#8221; things which are actually changing the world, rather than getting sucked into caring about the Jenga-like ever-taller stack-o-technologies which keeps us geeks so enthralled and IT budgets humming.

As a developer/entrepreneur, I have a lot invested in Mozilla&#8217;s technology stack, and it may seem foolish to argue against making it the focus of Mozilla&#8217;s attention. Indeed, ActiveState puts time & effort towards ensuring the XULRunner technologies&#8217; long and healthy life. I&#8217;d even say that we&#8217;re likely to do even more in the future, as that platform is becoming richer and more popular all the time (no matter what today&#8217;s blogovibes may say). As a human, however, I have _a lot more_ invested in the decentralized, open, and competitive nature of the internet and the web. Firefox&#8217;s technology stack could come and go, and us geeks would adapt, rebuild, try something else. Were the essence of the web to go away, everyone would be much poorer for it.

PS: Like everything else on this blog, this is an (overly preachy, I know) expression of a personal point of view, nothing more.

PPS: the above isn&#8217;t really a PS since there&#8217;s no Scriptum to be Post. But you get the idea.