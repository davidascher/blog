---
id: 425
title: Thunderbird 2.0.0.14 and SSL certificates
date: 2008-05-12T18:03:28+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2008/05/12/thunderbird-20014-and-ssl-certificates/
permalink: /?p=425
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "425"
categories:
  - Mozilla
  - MozillaMessaging
  - Thunderbird
---
Thunderbird 2.0.0.14 was recently released to the world: yet another security release for Thunderbird. Yay, and thanks to all involved! All was well, until news came in through a bug report that one of those included updates is problematic for some users.

Specifically, as part of making Firefox 2.0.0.14, we made a change in how the underlying platform handles SSL certificates. That change was made to increase the privacy of people visiting certain web pages, as documented in [this advisory](http://www.mozilla.org/security/announce/2008/mfsa2008-17.html).

The problem is that the switch (asking users to confirm that they want to identify themselves with a certificate) makes sense for web pages, but it doesn&#8217;t make sense as implemented for email transactions. There&#8217;s a lot more detail in [the relevant bug](https://bugzilla.mozilla.org/show_bug.cgi?id=431819).

Luckily, this problem likely doesn&#8217;t affect the vast majority of Thunderbird users. It only affects users who are issued a certificate to secure the communication with the mail server, rather than relying on passwords. With the 2.0.0.14 release, those users end up being asked to confirm the use of the certificate on every connection, which gets to be annoying.

Most of the users affected are likely in large organizations, as they are the ones who tend to issue their own certificates. Luckily, those organizations also often do their own QA before a deployment, so in all likelihood few people will be exposed to the bug.

Getting a fixed Thunderbird 2.0.0.15 out is planned, but we&#8217;re trying to figure out how to prioritize this release relative to the other releases.

In the meantime, there is a simple workaround that can be applied per user ([revert a preference setting](https://bugzilla.mozilla.org/show_bug.cgi?id=431819#c48)), or, for those deployments using [autoconfig](http://developer.mozilla.org/en/docs/MCD,_Mission_Control_Desktop_AKA_AutoConfig), by tweaking the central configuration file.

We could also release a XPI add-on to fix the preference, but that may or many not be easier &#8212; feedback welcome.

I&#8217;d love to hear from administrators of large Thunderbird installations in particular, as this bug highlighted for me several of the challenges we have in making sure that our processes are aligned with those of large deployments.

I&#8217;m also thinking that we need to setup better communication channels with people deploying large installations of Thunderbird (email lists, different blogs, etc.). If you&#8217;re involved in large-scale deployments of Thunderbird, email me and let me know your thoughts.