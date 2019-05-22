---
id: 374
title: Gateway drug for Thunderbird devs
date: 2008-01-04T13:13:42+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2008/01/04/gateway-drug-for-thunderbird-devs/
permalink: /?p=374
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "374"
categories:
  - Mozilla
  - Open Source
  - Thunderbird
---
If you&#8217;re keen to get involved with Thunderbird development but don&#8217;t know where to start, here&#8217;s a simple step which can 1) help you figure out all of the mechanics of doing work with Mozilla, and 2) move the project forward by addressing a fairly mechanical but still useful set of issues.

Joey Minta setup a [wiki page](http://wiki.mozilla.org/User:Jminta/Mail_XPCOMUtils) describing the overall task of converting Thunderbird to use XPCOMUtils, which is a new module available in Gecko 1.9 (which will be the foundation of Tunderbird 3). Converting Thunderbird to use it will simplify the code base and reduce startup time, with no downside identified so far, so it&#8217;s an easy patch to get reviewed.

To see an example of such a bug, patch, and review process, see [bug 410727](https://bugzilla.mozilla.org/show_bug.cgi?id=410727).

If you&#8217;ve never contributed Mozilla code before, it&#8217;s probably good to spend some time reading up on [developer.mozilla.org](http://developer.mozilla.org/en/docs/Developing_Mozilla), as well as reading up on [building](http://developer.mozilla.org/en/docs/Build_Documentation) Thunderbird.

If you want to talk to other Thunderbird developers as you&#8217;re working on a bug or patch, I suggest hanging out on #maildev on irc.mozilla.org.

Hope to see you there!