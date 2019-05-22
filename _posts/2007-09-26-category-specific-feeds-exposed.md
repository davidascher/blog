---
id: 333
title: Category specific feeds exposed
date: 2007-09-26T23:35:07+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2007/09/26/category-specific-feeds-exposed/
permalink: /?p=333
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "333"
categories:
  - Blogging
---
After a little bit of struggling with PHP (it&#8217;s been a while), I&#8217;ve exposed category specific feeds. Specifically, if someone wants to keep track of my Mozilla-related posts, here&#8217;s [the feed](http://ascher.ca/blog/category/mozilla/feed/) (or the browser-oriented [archive page](http://ascher.ca/blog/category/Mozilla/)). Similarly for ActiveState stuff ([feed](http://ascher.ca/blog/category/activestate/feed/), [archive](http://ascher.ca/blog/category/activestate/)), etc.

I haven&#8217;t yet figured out what tweaks are needed to my WP templates to make the feed exposed in the category-specific archives be the category-specific feed. It doesn&#8217;t look simple, as the category archives is really just a specialized search.