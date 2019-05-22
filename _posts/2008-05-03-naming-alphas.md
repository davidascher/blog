---
id: 421
title: Naming alphas
date: 2008-05-03T13:35:07+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "421"
categories:
  - Mozilla
  - MozillaMessaging
  - Thunderbird
---
Software production is a lot like sausage factories. The end result is nice, but peeking behind the factory walls isn&#8217;t always pretty (cue [scene](http://mightygodking.com/index.php/2008/03/03/tintin-in-america-the-abbreviated-conclusion/) from Tintin in America).

It&#8217;s been educational to go through the process of picking nominations for the next alpha release, understanding the interactions between Gecko changes and the impact on Thunderbird, and more. We&#8217;re getting there, though, as soon as we can figure out a couple of last issue. But then there&#8217;s the issue of &#8220;public perception&#8221;, in particular what we should _call_ this next release. Because names are loaded, and version numbers even more so.

So what is the point of doing this next release? There are lots of somewhat conflicting goals:

  * Because it&#8217;s time: it&#8217;s been a long time since there was any non-security release of Thunderbird, and that&#8217;s always dangerous. Software that&#8217;s not used by people outside the inner circle tends to have hidden flaws that get harder to fix with time. So it&#8217;s important to release something, _anything_.
  * Because we&#8217;re on trunk: Thunderbird development has been going on on the &#8220;trunk&#8221; of Mozilla for several months now, and as a result a lot of changes motivated by both the evolution of the platform and Firefox 3 have impacted Thunderbird. It&#8217;s good to get feedback on the consequences of those changes, whether that&#8217;s cool new features like the Add-on manager or core changes like the changes in the widgetry on the mac.
  * Because it&#8217;s a new team. The Thunderbird 2.0.0.x releases you&#8217;ve seen over the last few months have all been done by the Mozilla Corporation engineers who have those processes ironed out. Some of us on the Mozilla Messaging side are new to making Mozilla releases, and it&#8217;s certainly better for everyone if we work out the kinks in releases doing early releases rather than &#8220;important&#8221; releases. At the same time, having a new team means that we can challenge some of the old ways, and consider doing things differently because the environment is different.
  * Because we want to release often: Both Dan Mosedale and I really want us to move to a more agile development model, where releases aren&#8217;t that hard, and where we can experiment with changes without huge impact on the QA process. That&#8217;s going to be hard, and involve investments in all parts of the pipeline, from build automation (Rick&#8217;s on that), to unit test coverage (Mark&#8217;s on that), to rethinking how we do QA (Gary and Wayne are on that). But getting there also means understanding, documenting, and streamlining the release process.
  * To re-engage with the add-on developer community: there&#8217;s lots of work to do to make sure that when 3.0 is ready, the add-on community has been part of that process, so that their extensions can be ported to the new codebase. Having a release that they can target that is based on trunk is a good first step there (finishing and documenting STEEL is another big step in that direction).

Note that there&#8217;s a big reason to release which _isn&#8217;t_ mentioned above, and that&#8217;s &#8220;to get feedback on the big changes in the next major release of the product&#8221;. And that&#8217;s because none of the big changes that we&#8217;re hoping to have in Thunderbird 3 are in this build. So for most users, I expect that the differences between this next release and Thunderbird 2.0.0.14 are going to feel pretty minor. Which is how it should be at this stage.

However, given how long it&#8217;s been since there&#8217;s been a feature release, it&#8217;s likely that if we label this release &#8220;Thunderbird 3.0a1&#8221;, that we&#8217;ll both get complaints about how little has changed since Thunderbird 2, as well as give the impression that we&#8217;re close to nailing down Thunderbird 3, neither of which are true.

Furthermore, we really do mean that it&#8217;s an alpha release. There are no guarantees, there will be minimal testing, and it&#8217;s possible it will eat up all your mail (although unlikely =). So calling it Thunderbird _anything_ is likely to confuse people who don&#8217;t follow Mozilla closely.

Given all that, I&#8217;m thinking that this next release should be called **Shredder a1**, with Shredder (Rick Tessner&#8217;s brainstorm) being to Thunderbird what Minefield is to Firefox. We probably won&#8217;t have the word Shredder in the product for a1, but hopefully for a2.

Thoughts?