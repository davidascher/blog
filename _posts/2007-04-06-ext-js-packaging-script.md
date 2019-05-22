---
id: 250
title: Ext JS Packaging script
date: 2007-04-06T17:34:02+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/2007/04/06/ext-js-packaging-script/
permalink: /?p=250
tags:
  - ""
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "250"
categories:
  - General
---
I&#8217;ve been having fun working w/ (among others), the <a target="_blank" title="ExtJS" href="http://www.extjs.com" rel="noopener noreferrer">ExtJS</a> library (ext.js.com).  In fact, I&#8217;m a paid customer, meaning I get access to the SVN tree, which can come in handy. However, the SVN tree doesn&#8217;t include the packaged files needed for easy use, as those are currently built as part of the release process by the Ext JS team through a baroque process involving a Windows-only program.  While there are plans to provide tools to customers to make custom builds available on demand, that&#8217;s not there yet.  To make my own life easier in the interim, I wrote <a target="_blank" title="build_ext_packages.py" href="http://ascher.ca/build_ext_packages.py" rel="noopener noreferrer">a script</a> that I run from the root of the svn tree and creates the packaged files.  If you want to work off of the head, it&#8217;s handy.