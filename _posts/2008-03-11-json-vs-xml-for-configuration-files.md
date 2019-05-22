---
id: 398
title: JSON vs. XML for configuration files?
date: 2008-03-11T16:55:17+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2008/03/11/json-vs-xml-for-configuration-files/
permalink: /?p=398
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "398"
categories:
  - Mozilla
  - Open Source
  - Programming Languages
  - Software
  - Thunderbird
---
One of the topics we&#8217;re discussing in Thunderbird dev land involves how to distribute configuration files for Thunderbird, so that if you&#8217;re part of a group (users of large ISPs, enterprise users, gmail users, whatever), that the &#8220;right&#8221; default configuration can be picked up as automagically as possible.

There&#8217;s lots behind that effort, but there&#8217;s one point of debate which I thought I&#8217;d throw out here explicitly to get input from people outside the Thunderbird community. Thunderbird can easily support either an XML dialect, or JSON files. There&#8217;s a feeling that the formats are isomorphic, and that figuring out which syntax ends up being a tooling issue, in particular for unknown third parties who might want to also implement parsing of these files. Some people believe that XML, being more mature, is more likely to be parseable by various software packages &#8220;out there&#8221;. Others believe that JSON is a better fit, because it&#8217;s lighter weight, more mashable, etc.

Are there good best practices that people have developed as to when to use which markup language?

Comments here, please. Keep it civil and constructive, please!