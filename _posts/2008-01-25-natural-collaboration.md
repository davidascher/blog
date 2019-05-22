---
id: 381
title: Natural collaboration
date: 2008-01-25T17:13:17+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "381"
categories:
  - Mozilla
  - Thunderbird
---
There are projects with open source licenses, and there are open source projects.

It&#8217;s a distinction which I&#8217;ve known about intellectually for a long time, but which I&#8217;m just now starting to understand at a more emotional level.

In particular, I&#8217;ve talked to a bunch of people about some of the messy architectural issues that Thunderbird needs addressed to enable Cool New Features. Some of those people are somewhat cranky, sometimes bitter, often pessimistic, and undoubtedly excellent engineers, who look at the amount of work involved and shudder. At the same time, I&#8217;m recruiting engineers who I think will be able to undertake some of those &#8220;heavy lifting&#8221; jobs which, people often assume, no one who wasn&#8217;t paid to do it would want to do, because it&#8217;s &#8220;not sexy&#8221;.

Two such messy areas in the case of Thunderbird are the progressive, careful replacement of the Mork database backend with a SQLite based backend, and the removal of the use of RDF in areas where it proved not to be a poor technology choice in hindsight. Both of these are hard, high risk areas, with few people around who really understand all the details.

And yet.

Two volunteers, [Joshua Cranmer](http://quetzalcoatal.blogspot.com) and Joey Minta, both in school and doing this for reasons that they should probably explain themselves someday, are making good headway towards tackling these issues, building in Joshua&#8217;s case on a test framework put together by Mark Banner, also a volunteer, and in Joey&#8217;s case on an outline that David Bienvenu, one of the original Thunderbird developers, had generously written up.

It&#8217;s _so much fun_ to watch the dynamics of natural collaboration that can occur when people share a goal and enjoy working together, even if it&#8217;s all mediated by online messages. I look forward to a &#8220;Mailnews party&#8221; where we can meet face to face. Both of these projects will likely take a long time to work through, especially as we need to pay close attention to migrating user data, accomodating extension authors, and all the nitty gritty details that distinguish high quality software from demoware. But it&#8217;ll be a fun, collaborative project, so it&#8217;s fine!

In other news, I&#8217;ll be attending the [CalConnect Roundtable](http://www.calconnect.org/roundtable11.shtml) Feb 6-8, and plan on meeting at least some of the people behind the [Mozilla Calendar](http://www.mozilla.org/projects/calendar/) project and other calendar projects.