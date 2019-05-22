---
id: 350
title: Gmail enables IMAP
date: 2007-10-23T21:49:32+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "350"
categories:
  - Gmail
  - Google
  - Mozilla
---
It&#8217;s nice to see that Gmail now supports (at least for some accounts) [IMAP access](http://mail.google.com/support/bin/answer.py?ctx=%67mail&hl=en&answer=75726). It will make talking to it from the iPhone much nicer &#8212; as I mentioned last week, IMAP is just a much better protocol.

It seems that they&#8217;re mapping labels to IMAP folders, which is an natural but non-trivial idea, as multiple labels can be assigned to a single email, but AFAIK IMAP doesn&#8217;t have the concept of a single email message in multiple folders. Also, the labels are per-conversation, not per-email, so the metaphors don&#8217;t line up perfectly. I wonder what happens to conversational labels if one uses IMAP to move a single email across folders&#8230;