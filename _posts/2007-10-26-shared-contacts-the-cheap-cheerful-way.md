---
id: 355
title: 'Shared contacts, the cheap &#038; cheerful way'
date: 2007-10-26T17:22:19+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "355"
categories:
  - caldav
  - carddav
  - collaboration
  - groupdav
  - MailCo
  - Mozilla
  - Thunderbird
---
I&#8217;ve been meaning to write more about groupware and collaboration, and hopefully will find the time for a longer post on the topic, but here&#8217;s a bit of timely news. Ludovic Marcotte and friends have just released a combination of some of their previous extensions to Thunderbird and Lightning as something they call the [SOGo connector](http://www.inverse.ca/contributions/sogo_connector.html): it&#8217;s an extension to Thunderbird which, when combined with Lightning, provides features like remote address book through [CardDAV](http://ietfreport.isoc.org/idref/draft-daboo-carddav/) (sending vCards through CalDAV, AFAICT), and an informal protocol called [GroupDAV](http://www.groupdav.org/). While CardDAV is an extension to CalDAV which is an IETF spec, GroupDAV is currently an ad-hoc, simple protocol built to let clients interoperate with open source groupware servers, which probably explains both why it&#8217;s simple and why only a few servers (including [SOGo](http://www.inverse.ca/contributions/sogo.html), of course) support it.  
I still need some education as to what relevant standards have to say (even in non-final form) about shared contact lists. More on this topic later I&#8217;m sure.