---
id: 292
title: OpenID best practices
date: 2007-06-09T10:52:17+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "292"
categories:
  - General
---
Any recommendations for sites out there that I can study to see how to gracefully convert to OpenID from a non-OpenID based account system?

I just poked around [trenchmice](http://www.trenchmice.com/), and that&#8217;s a good way \_not\_ to do it. Specifically:

  * UI for logging in splits out signing in from registering at the beginning, whereas I think with an OpenID it&#8217;d be better to authenticate first and then create an account if needed. 
  * No support for iNames 
  * it&#8217;s a registration that requires a lot of sreg-data, including country, postal code, etc. 
  * even with the sreg data filled in, it didn&#8217;t like my canadian postal code. 

I&#8217;ve also noticed <pogo.com>, which is interesting in that they hide OpenID quite well, it being indicated primarily by a link next to the choice of userid that reads &#8220;Use my AOL or AIM screen name&#8221;. A tweak on that process might work better for us, although we&#8217;d want to be clear about the use of OpenID.

NB: We would naturally not require the creation of a third-party OpenID to login to our web properties &#8212; most likely, we&#8217;d become an OpenID provider and simply upgrade existing accounts to be OpenID accounts &#8212; letting users decide whether to user their ActiveState OpenID on other sites or vice versa.