---
id: 478
title: How should we manage autoconfiguration files?
date: 2009-01-20T17:37:26+00:00
author: David Ascher
layout: post
guid: http://ascher.ca/blog/?p=478
permalink: /?p=478
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "478"
categories:
  - Mozilla
  - Thunderbird
---
One of the features we&#8217;re working on for Thunderbird that I&#8217;ve mentioned before is the &#8220;autoconfiguration&#8221; setup, whereby when setting up an account, you type in your email address, and using the domain part (the part after the @ sign), Thunderbird tries to figure out what the right settings are. When it works, this is an amazing feature. This is not a new idea &#8212; in fact many mail programs have implemented in the past, including Exchange 2007 and the iPhone&#8217;s Mail program.

There are three ways of solving this problem: asking a central server for configuration files per domain, bundling some of those configuration files, and doing local network probing to look for likely domain names (mail.domain.com, imap.domain.com, etc.).

The central repository of configuration files has many advantages if we can figure out how to decentralize the provisioning of these configuration files, while remaining secure. In particular, it allows Thunderbird to &#8220;learn&#8221; about new domains or changed configurations as soon as those files are vetted, without having to wait for the next version of Thunderbird. Even with only a few configuration files, we should be able to cover the &#8220;short, fat, end&#8221; of the email domains &#8212; the top 200 domains for example probably cover 90% of home email users, which would be an amazing improvement for Thunderbird&#8217;s usability. (Gerv has already started [a project](http://wiki.mozilla.org/MailServerList) months ago to collect some of this information)

Local port probing is most useful in corporate environments. Either their small user base or corporate policies may deter them from submitting their configuration files in the central server. In this case, the challenge is to strike the right balance of efficiency vs. completeness. We certainly don&#8217;t want to probe hundreds of ports on a local domain in a desperate search for a mail server, but to assume that all mail servers are configured the same way is unrealistic. A hybrid of the Exchange 2007 [autodiscover](http://technet.microsoft.com/en-us/library/bb232838.aspx) model and the Mail.app configuration hostname-guessing model is likely optimal for this part of the market.

Side note: I could imagine an add-on that would bundle the configuration files and get updated periodically for those users who want to avoid leaking any data.

We welcome input on how we should manage these configuration files. The feature hasn&#8217;t landed yet, so it&#8217;s still very possible to influence this process. From my perspective there are a few key characteristics that should drive our process:

0) Reusing existing processes when possible makes life easier.

1) User experience is the goal. The point of this feature is to let as many people end up with a well-configured Thunderbird as easily as possible. This is why we&#8217;re going after a hybrid approach, trying to cover as many different environments with a single user experience.

2) This problem is not Thunderbird-specific. The data we&#8217;re looking for is not about how to configure Thunderbird, but how to configure IMAP/POP/SMTP email clients in general. If Mozilla can help solve the problem of email configuration in a safe, scalable, trusted way, then I&#8217;m fine with other email clients using it. I see this as potentially a very powerful public service that Mozilla can provide to email users everywhere.

3) We want to decentralize contributions of configuration files, but control the review processes, to facilitate end-user contributions and cover the long tail of domains, with a consistent policy especially with respect to validation.

In the short term, it feels like we could easily start with a variation on the processes we already use for code, with a security review overlay. In particular, I would suggest as an initial draft that:

&#8211; we have something equivalent to a module, which contains the published configuration files and processes around them  
&#8211; each configuration is reviewed by someone other than the configuration submitter (patch author)  
&#8211; each configuration needs to be validated by the reviewer against public documents published by the mail provider (ISP, university, etc.)  
&#8211; Mail administrators can file a bug, or contact the module owner directly if they want to report changes in their email setup or suggested changes.

We will probably want to figure out more sophisticated systems involving cooperation with mail administrators (using MX or DNS records, or signed emails, or &#8230;) in a later phase, but I don&#8217;t think we should gate being able to serve users of the largest domains (gmail, yahoo, major ISPs, universities). Walk, then run, should be our approach.

Similarly, there are possible futures where users could share configuration files with each other, but I don&#8217;t think we&#8217;re ready to tackle those securely yet.

We&#8217;ll figure out a way for those interested in submitting or reviewing configurations to sign up in a later round. At this point, we&#8217;re most keen on process-type feedback. Comment on [the bug](https://bugzilla.mozilla.org/show_bug.cgi?id=474520), or here, thanks!

PS: Whatever process we arrive at, we&#8217;ll then apply to the files we&#8217;ve been using in testing and the configuration data in Gerv&#8217;s spreadsheet, to make sure that all the data has gone through the right hoops.