---
id: 416
title: 'Hamburg: Thunderbird, Calendar, Accessibility, CouchDB?'
date: 2008-04-21T08:54:31+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "416"
categories:
  - Calendaring
  - CouchDB
  - Mozilla
  - Open Source
  - Thunderbird
---
In day 3 of a Calendar meeting face-to-face, we had a few deviations from the core of the main topics (Lightning, Sunbird, Thunderbird integration), with two cool side-trips.

First, [Marco Zehe](http://www.marcozehe.de/) came to talk about the state of accessibility in Thunderbird and Calendar. The take-away message to me was that accessibility for &#8220;trunk&#8221; (Thunderbird 3, etc.) is pretty good, thanks to all the work done at the platform level. There are some outstanding issues, which we agreed to consider as blocking Thunderbird 3, but it&#8217;s one of those areas where the next version of Thunderbird will be significantly better than the current one for a subset of users.

Second, at my instigation, [Jan Lenhardt](http://jan.prima.de/) gave a talk about [CouchDB](http://couchdb.org/), which was nicely off topic but thought-provoking. The coolest bit is that about an hour after the end of Jan&#8217;s talk, Philipp Kewisch, Calendar hacker extraordinaire, and author of the [GData add-on for Calendar](http://wiki.mozilla.org/Calendar:GDATA_Provider), had whipped up a proof-of-concept CouchDB provider for Lightning, meaning that calendar data (events, etc.) can be stored in a couchdb repository.

Kudos to the CouchDB and Calendar teams for building systems that clearly are easy to extend, and to HTTP/REST and JSON for providing great building blocks.