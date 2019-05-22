---
id: 412
title: Accepting Nominations for Thunderbird 3.0a1/3.0 blockers
date: 2008-04-08T13:12:09+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2008/04/08/accepting-nominations-for-thunderbird-30a130-blockers/
permalink: /?p=412
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "412"
categories:
  - Mozilla
  - Open Source
  - Thunderbird
---
Mozilla project planning, for those not in the know, happens primarily through bugzilla entries, which include bugs, feature requests, work items, everything. It may not be the best way to organize things that aren&#8217;t really software defects, but it&#8217;s what we have, and somehow it works out ok.

As a case in point, the way releases get planned (what should be in which release) is through flags &#8212; bugs can be nominated for a release (by anyone), and then a group of people with a good overall perspective on the release (called &#8220;release drivers&#8221;) either accept a nomination or reject it &#8212; or redirect it to another release. Furthermore there are bugs that are considered _blocking_, while others are considered _wanted_. The former are the bugs that we&#8217;d delay a release in order to get them fixed, while the latter are nice-to-haves, but they wouldn&#8217;t block a release.

It&#8217;s a remarkably distributed process, with discussions about which bugs should be addressed and why distributed across the bugs. We then use bugzilla queries to get a holistic picture of the release, which gets particularly important close to the end-game. Over time, I think we can build better mechanisms, but the bird in the hand&#8230;

Importantly, release planning starts with _people nominating bugs_ for either &#8216;wanted&#8217; or &#8216;blocking&#8217; status. We currently have flags in place for two releases: Thunderbird 3.0a1, and Thunderbird 3. The former is imminent, the latter not so much.

For 3.0a1, our release goal is first and foremost to actually do a release, which will exercise a bunch of muscles and mechanisms which have not been exercised in a while. Nominations for 3.0a1 should focus on bugs which significantly impact the ability of alpha users to give feedback on the product. Common crashers, bugs causing data loss, and significant usability problems are the most obvious candidates. We&#8217;re not being feature-driven for this early alpha, so don&#8217;t bother nominating new features for this release.

For 3.0, we&#8217;re definitely willing to consider all kinds of bugs. These will help us scope the extent of work needed, but also help us get a broader, &#8220;crowd-sourced&#8221; picture of the state of the product &#8212; what, among the thousands of contributed ideas and bug reports, impacts the most people. The easiest way to express &#8220;support&#8221; for a bug is simply to vote on it. Don&#8217;t add comments to the bug if you&#8217;re not contributing new information beyond your support &#8212; that makes the bugs harder to read, hence harder to fix. Instead, vote on your favorites. (I know voting on bugs is far from ideal &#8212; but it&#8217;s better than any other current alternative)

To nominate a bug, you need to be logged in to bugzilla, and you should set the appropriate flag (under the CC area) to ?. Only drivers are allowed to set + or &#8211; flags, so please don&#8217;t.

For more information, see [the wiki](http://wiki.mozilla.org/Thunderbird:Release_Driving).