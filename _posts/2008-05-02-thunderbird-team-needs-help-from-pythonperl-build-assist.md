---
id: 420
title: Thunderbird team needs help from Python/Perl build engineer
date: 2008-05-02T17:07:30+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2008/05/02/thunderbird-team-needs-help-from-pythonperl-build-assist/
permalink: /?p=420
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "420"
categories:
  - Mozilla
  - Open Source
  - Python
---
If you&#8217;re a Thunderbird fan but not interested in fixing some of the nasty C++ problems we tackle in the product, you could still be very, very helpful if you can help us with a little Python/Perl build problems.

Specifically, Mozilla has a great system called &#8220;try servers&#8221; where one can submit patches against the tree, and the build system runs builds on Linux, Mac and Windows, using those patches, then serves those builds for testing. This is really helpful to figure out if proposed patches solve specific problems, especially when the developers aren&#8217;t able to reproduce the bugs, but testers can. It works great for Firefox development right now.

The only problem is that there&#8217;s a little bit of patching needed to the try server code itself to make it able to work with other targets besides Firefox, as described in [bug 431375](https://bugzilla.mozilla.org/show_bug.cgi?id=431375). [Ben Hearsum](http://blog.mozilla.com/bhearsum/archives/25), a build guy from Mozilla, is happy to help someone figure out those patches, but he doesn&#8217;t have time to make it happen right now.

From what i can tell, required skills include comfort with CVS and Linux, Python, Perl, and some build engineering common sense.

Thanks in advance!