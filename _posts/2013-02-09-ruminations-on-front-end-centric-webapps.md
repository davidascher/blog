---
id: 773
title: Ruminations on front end-centric webapps
date: 2013-02-09T16:08:19+00:00
author: David Ascher
layout: post
guid: http://blog.ascher.ca/?p=773
permalink: /?p=773
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "773"
categories:
  - Mozilla
  - Uncategorized
  - webmaker
---
I&#8217;ve been poking around [firebase](http://firebase.com/) & [meteor](http://meteor.com/), and [sparkleshare](http://sparkleshare.org/)+[github](http://github.com/) and [dropbox](http://dropbox.com)+[site44](http://site44.com/). I&#8217;m a bit disturbed (in a good way) by what feels to me like a sea change that&#8217;s happening there, and it seems to me that almost anyone thinking about web developers writ large needs to think hard about what this means for their roadmap.

In particular, a few brief thoughts:

I&#8217;ve been, for a while now, using sparkleshare + github pages with CNAME support as a way of making trivial static sites that are real. Sparkleshare is an open source git-syncing-to-filesystem client (with nice ergonomics and design, OMG!). With github-pages and CNAME support, this means that I save in my favorite text editor, and within \_seconds\_ the thing is live on the web. That&#8217;s a disruptive flow.

I&#8217;ve been coaching the [harp.io](http://harp.io/) team through [WebFWD](http://webfwd.org/), and they have a service which does similar things on top of Dropbox, including coffeescript/haml processing, CDN, load balancing, push-button deploy, screenshotting for multiple user agents, rollback, etc. In other words, you author your webapp locally on a dropbox folder, and they take care of high-quality, high performance hosting. There is no app-specific server-side logic (which means you need to either have static sites or integrate with hosted services for said features).

I recently ran into site44.com, which does a &#8216;cheap & cheerful&#8217; version of what harp.io does, with no push-button deploy/rollback, and much more like sparkleshare &#8212; instant deploy, with little management capabilities (but instant gratification).

Both harp.io and site44 use Dropbox for syncing, which is a _Big Idea_ in my opinion because setting up Dropbox is so much easier than setting up git credentials (what with SSH keys, etc.). Both assume that the user has write access to local files (which may be a problem in some retrograde environments like enterprises and schools, but which could be solved with web-based editors).

I finally bit the bullet and dig in again into Firebase. Firebase is effectively a key-value store, with Pubsub messaging of data changes. They&#8217;ve made some interesting progress in their security and auth models (they include persona support, which is cool). Firebase feels like it makes it trivial to add state and real-time behaviors to previously static sites. The API surface area is quite small, so it should be fairly easy to adopt.

I&#8217;m also looking again at Meteor. Since they first launched w/ both fanfare and a bit of ridicule due to overhype, they&#8217;ve cleaned up their act significantly: the license is now MIT, they&#8217;ve announced $11M in financing from tier-1 VCs, announced an enterprise business plan to complement their open source offering, and build a bunch of APIs. Meteor feels like a steeper learning curve, and another &#8220;at-bat&#8221; for reactive programming (a topic I&#8217;ve been interested in for a decade). 

Meteor feels like a solid foundation for a potential full-stack offering, and I like the open source option; Firebase feels like a really compelling basis for demoware and hacks. Regardless, syncing from filesystem to websites without thinking too hard about deployment is a huge benefit of front-end-driven sites.

Single-page apps feels to me like the conceptual next hurdle. Figuring out how to manage history and state management so that the app feels as dynamic as the best webapps, but has good URL support, etc., is an engineering challenge (see e.g. [history.js](https://github.com/balupton/history.js)). And it certainly challenges the old mental model of one URL -> one file which pulls down other resources. The newer model (especially on mobile, low-latency devices) needs to be one app -> many URLs, with one core application logic which pulls data-as-JSON and builds most state clientside (with serverside rendering as an optimization for high traffic or slow-CPU environments, as per airbnb&#8217;s post).

I&#8217;m not sure what this means for advanced [webmaker](http://webmaker.org/) skills. At the very least explaining some of the above to a broader audience is something we could do.