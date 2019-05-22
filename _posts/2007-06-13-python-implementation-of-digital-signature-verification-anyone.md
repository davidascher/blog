---
id: 297
title: Python implementation of digital signature verification anyone? UPDATED
date: 2007-06-13T17:08:00+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "297"
categories:
  - General
---
Hey, Lazyweb, what&#8217;s the status of Python libraries to do Diffie-Hellman digital signature verification?

UPDATE: The lazyweb didn&#8217;t help (Boris, geez.), but patience with Google did point me to:

  *  [m2crypto](http://chandlerproject.org/bin/view/Projects/MeTooCrypto), which has a rich interface to the openssl code, include DH
  * turns out the openid libs already package a [DH wrapper](http://www.openidenabled.com/resources/darcsweb?r=python-openid;a=headblob;f=/openid/dh.py) as well