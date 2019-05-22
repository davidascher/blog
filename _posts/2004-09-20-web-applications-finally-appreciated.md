---
id: 752
title: Web applications finally appreciated
date: 2004-09-20T04:00:00+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "7"
categories:
  - General
---
> First-time visitor: &#8220;Hi, my name is David, and for years I didn&#8217;t really understand the power of web apps.&#8221;

> Support group participants, in concert: &#8220;Hello, David&#8221;

There, now I&#8217;ve said it&#8212;I am finally starting to understand what people have been getting so excited about for the last decade. That&#8217;s oversimplifying, of course, but I am more and more appreciating how the web is changing the rules.

A few factors that are shaping my current thinking are Gmail, bloglines, and Paul Graham&#8217;s Hackers and Painters.

#### Web apps are valuable because they&#8217;re public 

Like many techies, I&#8217;ve been playing around with [gmail](http://gmail.google.com) (yes, I periodically have invites left over), mostly to read new mailing list traffic. It&#8217;s, not surprisingly, quite good at some things (finding old mail, structuring conversations, user interface), and surprisingly bad at others (i.e. prioritizing email for the sake of efficient slogging through _new_ mail, e.g. by understanding the different types of emails). Mostly, though, it&#8217;s a very Googlish app because it redefines cool by throwing away decades of groupthink around the value of eye candy. Kudos to them for that. (I have lots of other thoughts about Gmail that I&#8217;ll defer to another post).

I&#8217;ve also become a fan of the blog aggregator [bloglines](http://www.bloglines.com). Gmail and bloglines both are fascinating because their value is (so far) tied to their living in the &#8216;public web&#8217;. Not only does their scalability make them interesting from a business point of view, not only are they remarkably simple systems (just &#8216;good ideas&#8217;!), not only are they better than desktop apps because they&#8217;re accessible from anywhere, but they have fascinating additional potential if they get to exploit [Metcalfe&#8217;s law](http://en.wikipedia.org/wiki/Metcalfe%27s_Law). Bloglines already achieves some of this by suggesting blogs I may want to read based on my reading list and correlations with other subscribers&#8217; interests. Gmail, thus far, is bound by the constraint that email is email is email, even though communication between gmail accounts could be much richer than the &#8216;standard&#8217;. I&#8217;m fully expecting Google to do much more with gmail, google groups and blogger than they&#8217;ve done thus far&#8212;and to capture the power of the masses before the power of the fiefdoms that are corporations, based on their track record.

Tagging along the acknowledgement that for these apps at least &#8216;the power is _in_ the web&#8217; is the realization that it&#8217;s difficult for me to see how systems like gmail and bloglines could mesh with firewall-bound modes of operation. I can&#8217;t have work email on gmail. I can&#8217;t read internal blogs with bloglines. As long as that&#8217;s true, web apps will always have to live _alongside_ similar apps that live inside the firewall (either on desktops or on internal websites). Frustrating to say the least, given that I don&#8217;t see how firewalls (or more generally the notion of private data) are going to go away anytime soon. I think I&#8217;m noticing this now because I never really cared to integrate &#8220;internal&#8221; data sources with Amazon, ebay, online radio, newspapers or any of the other &#8220;old&#8221; web sites that are part of my life. When it comes to email, blogs, and bookmarking services like del.icio.us, I&#8217;m finding that there is a fundamental tension between the need for some privacy and the public, with no clear answer in sight.

#### Publishing of web apps as a fundamentally different software publication model

[<img class="book" vspace="5" hspace="5" border="1" align="right" src="http://store1.yimg.com/I/paulgraham_1809_27074" />](http://www.paulgraham.com/hackpaint.html)

One of the best parts of Paul Graham&#8217;s [new book](http://www.paulgraham.com/hackpaint.html) was the chapter in which Paul explains how much more sane he finds publishing software that lives on a server you (the publisher) run compared to shipping bits to customers. The biggest appeal from an end-user point of view (which in the end is all that _should_ matter) is the fact that the application can change progressively when the code is ready, because there are no major releases. Gmail changes periodically, and sometimes I notice, sometimes I don&#8217;t. As long as the changes are subtle and for the better, my user experience is nothing but good. Another consequence of web application architectures is that, due to the simpler modes of interaction with the software (the browser), automated testing & QA is more easily achieved, thereby putting fewer steps between the conception of a feature and its delivery to customers.

The alternative model (employed by most publishers of &#8220;downloadable bits&#8221;) consists of releases which go through typically slow QA cycles, have associated marketing rollout plans, more or less rigid schedules, known bugs, patch releases, etc. Central to that is that releases are expensive (even if they&#8217;re cheap for the publisher, customers still need to upgrade, and they never all do). Some silver linings have been found in that state of affairs: &#8220;major&#8221; releases are often seen as valuable because they provide stable definitions of what&#8217;s in the product, which in turn makes it easier to define the value of the product, document it, _discuss_ it, etc. It&#8217;s also true that marketers like occasions to make a splash, salespeople like occasions to talk to customers, and developers like to know that they&#8217;re &#8220;done!&#8221; (at least for now).

Note that most open source software projects follow this model, so it&#8217;s not just &#8220;marketing folks&#8221; who think this way. Open source communities bicker for months about what should go in a release, and users would be quite befuddled if there was no way of knowing &#8220;which version of Python you&#8217;re running&#8221;.

Which is better? Paul clearly believes the web-based, continual release model is better. Me, I&#8217;m not sure.

Speaking as a developer, I&#8217;m torn&#8212;continuous release is a goal most engineering teams strive for constantly&#8212;yet sometimes evolving an app through continual working stages is just too hard (and managing parallel development branches is often even harder).

As a manager, my mind reels at the agility that a continual release _to the customer_ requires of _every bit of the operation_, from the doc writer (the doc plan is &#8220;what changed yesterday?&#8221;) to the sales people to the bug triage process (last week&#8217;s bugs may not be reproducible, but is that because they&#8217;re really gone?). At the same time, the appeal of reducing organizational and individual release stress is significant.

Speaking as someone who has to understand the impact of effort on revenue, I&#8217;m also torn. The two different models clearly imply different ways of monitoring the state of the business&#8212;in one case, one gets to judge releases by relatively coarse metrics such as upgrade rates, size of revenue &#8220;spikes&#8221; tied to launches, etc; in the other, one relies on day-to-day measurement of the efficiency of the online &#8220;machine&#8221;. I can imagine scenarios where it becomes very hard to know whether changes in the apparent health of the business are due to code changes, graphics changes, or the fact that it&#8217;s Friday.

As a user interface wonk, one of the concerns that comes to mind with the &#8216;constant evolution&#8217; model is that if an app works &#8220;differently&#8221; every day, it can becomes harder for the user to gain comfort with it. I suspect that the model that Paul argues for works great for technically savvy, &#8220;high-end&#8221; users, but would be harder to get past &#8220;mom & pop&#8221;. Google&#8217;s search engine has changed veeerry sloooowly. Then again, it&#8217;s much too easy to underestimate the ability of people to adapt to change. I wonder if eBay evolved as rapidly as Paul&#8217;s online store generator did, even matching for &#8216;maturity&#8217; of the apps.

<ins>Update: I&#8217;m not the only one to think that: see <a href="http://allinthehead.com/retro/225/">Drew McLellan</a>&#8216;s post on the topic.</ins>

Regardless, I&#8217;m grateful to Paul for making the point so clearly and helping frame my thinking. These bits of information, combined with the cumulative effects of hearing Tim O&#8217;Reilly [speak](http://conferences.oreillynet.com/cs/os2004/view/e_sess/5515) about the [changing face of the software ecosystem](http://tim.oreilly.com/opensource/paradigmshift_0504.html) for years, are finally starting to affect my world view. It feels good.