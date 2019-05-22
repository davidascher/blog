---
id: 491
title: Thunderbird 3 beta 2
date: 2009-02-26T12:13:27+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/?p=491
permalink: /?p=491
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "491"
categories:
  - Mozilla
  - MozillaMessaging
  - Software
  - Thunderbird
  - Web
---
On the road to Thunderbird 3, another milestone &#8212; this time, [Thunderbird 3 beta 2](http://www.mozillamessaging.com/en-US/thunderbird/3.0b2/).

[<img src="http://farm4.static.flickr.com/3555/3311116652_0968db2ecc.jpg" alt="illustration" width="500" height="176" />](http://www.flickr.com/photos/davidascher/3311116652/ "illustration by David Ascher, on Flickr")

### Why do beta releases?

Beta releases are funny things. They serve a few purposes. The first is to make sure that we periodically stabilize the code base, as without periodic &#8216;cooling&#8217;, it&#8217;s hard to get a handle on the quality of a piece of software. Betas also serve as deadlines, which are magical motivators for some people. Some of us will spend way too many hours staying up late in the night in order to &#8220;make a deadline&#8221;.

Betas for open source software are even more odd in that people interested in staying _very_ involved with the project can use nightly builds, which are updated every day. I&#8217;ve been using nightly builds of Thunderbird for over a year, as have several thousand other users. As a user of nightlies as much as a project coordinator, by the time the beta is released to a wider audience, all the excitement is historical.

Another fascinating aspect of beta releases is that, because we know there will be another release, and because the purpose of the beta is to get a broader set of testers to shake out edge cases, we try to be conservative about slipping in major features at the last minute, as the odds of those features being polished in time are never what we hope they&#8217;ll be. So we routinely delay feature additions until the next cycle, to avoid dragging the beta validation process out. It&#8217;s an unpleasant, but unavoidable part of optimizing releases.

If we do our job right there, then by the time the beta ships, the features that have landed are free of major bugs. We of course can&#8217;t know that until we get feedback from the beta.

### What&#8217;s in this release?

The most striking part of the release is the sheer volume of bug fixes. It&#8217;s not sexy work, it&#8217;s often the hardest work, but it&#8217;s very important. [This list](http://www.rumblingedge.com/2009/02/26/thunderbird-3-beta-2-released/) (of bug fixes and feature work, but mostly bug fixes) is impressive.

Of the features that have landed, I want to talk about two that many users could easily ignore: archiving, and the activity manager.

The archive feature is straightforwardly borrowed from GMail&#8217;s archive feature, which we think is great. The idea is that figuring out exactly which folder each message should be filed is a process that can take a lot of time and effort &#8212; something that wasn&#8217;t a real problem in the early days of email, but which becomes a real time sink with thousands of messages. With a good enough search engine, it&#8217;s easier for many users to simply &#8220;archive&#8221; the message (doesn&#8217;t really matter where), get it out of the way, and then rely on the search capability to find the message again.

In this beta, we&#8217;re half-way there. The archive feature is there if you want it, but you can also use the standard &#8220;file in a folder&#8221; method. Thanks to work we did before beta2, the archiving is fast, putting messages in per-month folders at the click of a buttton or a keystroke. The new fast global search hasn&#8217;t landed yet, but even our &#8220;old&#8221; cross-folder search mechanism has gotten a lot better.

I already love the feature &#8212; being able to select messages I don&#8217;t need to worry about anymore, hit &#8216;A&#8217; and be done with them, saves me a lot of time and mental effort

The second feature worth highlighting is also not fully deployed, but already useful. The Activity Manager was [born out of a recognition](http://clarkbw.net/blog/2008/06/04/activity-is-the-new-download/) that Thunderbird 2 is pretty bad at telling you what it&#8217;s doing. It says a lot of things, it says them fairly loudly, but they&#8217;re rarely the things you want to know. We&#8217;re building infrastructure that will let the various bits of Thunderbird be much more helpful in describing what&#8217;s going on (through a log of notable events), what went wrong (non-intrusive but notable alerts), and how it&#8217;s progressing at long-running tasks (with more context than just a single progress bar). Teaching software that wasn&#8217;t designed with a notification mechanism or philosophy in mind how to be polite and informative is a slow and arduous task, but we&#8217;re making good progress. In Thunderbird 3b2, there&#8217;s an Activity Manager window, which for now will just report on message moves, copies and deletes, and IMAP auto-syncing. Now that the framework is in place, we should be able to have a lot more informative messages when you need them, and reduce the number of dialog boxes (especially the ones you can&#8217;t do anything about!).

One of the fascinating aspects of the activity manager is that it&#8217;s giving even those of us who know how the software works on a detailed level a better handle on important global aspects. For example, the activity manager showed me that the autosync function can and should be much more aggressive, so that more of your email is already downloaded before you need it.

Other features you may notice:

  * Much more useful Growl notifications on OS X
  * Keyboard shortcuts for quick tab navigation
  * Better looking forwarded mail
  * Fewer dialog boxes

### What&#8217;s next?

The next beta release is our last scheduled beta. As such, we&#8217;re thinking of it as the last milestone to introduce Big New Features. Furthermore, we&#8217;re hoping to be even better behaved this cycle and land features as early in the process as possible. Upcoming features which we hope will be available in a nightly build soon include:

  * the new global search function, leveraging tabs
  * cleaning up the message header area further
  * &#8220;pop tarts&#8221; to complement the activity manager
  * the beginning of some theming work (prettier icons, etc.)

And then, of course, there will be unplanned bright ideas which show up out of nowhere. Life wouldn&#8217;t be fun without those.

[Try out the beta](http://www.mozillamessaging.com/en-US/thunderbird/3.0b2/), file bugs, send feedback!

PS: the illustration at the top is from a brand spankin&#8217; [new website for Mozilla Messaging](http://www.mozillamessaging.com). We&#8217;ve changed the site to make it the primary destination for Thunderbird users, riffing on the look of other Mozilla websites, and yet quite distinct. I find the illustrations in particular a lot of fun, and I&#8217;m very proud of the team that built it.  [Rafael Ebron](http://rebron.org/) ran the project with the [SpreadThunderbird team](http://spreadthunderbird.com/), with designs from [The Royal Order](http://theroyalorder.com/), and implementation from [silver orange](http://www.silverorange.com/). A very nice job, thanks to all who contributed!  The new site also allows us to build localized sites, which will be amazing.