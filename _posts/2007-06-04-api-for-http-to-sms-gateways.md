---
id: 287
title: API for HTTP to SMS gateways?
date: 2007-06-04T17:24:41+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "287"
categories:
  - General
---
It appears that every carrier has their own web to SMS gateway. Is there anyone maintaining an open source library that centralizes that knowledge, so that at the very least one could do:

`<br />
  send_sms(carrier_name, subscriber_number, sender, message)<br />
` 

(Note that I&#8217;m not asking for the `carrier_name` to be guessed.

I&#8217;ll take any reasonable language implementation.