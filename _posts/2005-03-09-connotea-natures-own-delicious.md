---
id: 94
title: 'Connotea: del.icio.us for scientists'
date: 2005-03-09T01:31:01+00:00
author: David Ascher
layout: post


enclosure:
  - |
    http://thestranger.com/audio/jefferson_starbucks.mp3
    3584120
    audio/mpeg
  - |
    http://thestranger.com/audio/jefferson_starbucks.mp3
    3584120
    audio/mpeg
    
    
restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "94"
categories:
  - Blogging
  - Computing
  - Publishing
  - Science
  - Social Software
  - Web
---
Doing a little digging on the topic of my last post, I was poking around nature.com, and found [connotea](http://www.connotea.org/), which [is described](http://www.connotea.org/about) as a derivative of [del.icio.us](http://del.icio.us). It is apparently similar to an independent effort called [CiteULike](http://www.citeulike.org/).

At first, it seems like an awful lot of duplication &#8212; the core is basically a clone of del.icio.us. The biggest difference seems to be that it seems to think of URLs as handles to actual bibliographic entries, which are extracted at bookmarking time from the pages being bookmarked, and the bibliographic handle is the &#8220;primary key&#8221; (I wonder what happens if two URLs point to the same biblio entry). The analysis works on a few major sites so far, including [pubmed](www.pubmed.com) and Amazon. Having the bibliographic data then lets them do integration with citation management software (like EndNote). If enough of one&#8217;s sources are found online, then I can certainly see that as being a useful tool &#8212; I spent way too much time entering LaTeX bibliographies over the years.

But is the new feature &#8220;worth&#8221; having a _segregated_ social bookmarking service (and data pool) just for scientists?

First, will it work? Assuming that the system is bootstrapped, my guess is: probably. The social aspect of del.icio.us, i.e. the tag-sharing, link-exploring and folksonomy-building will probably work just fine in a &#8220;vertical&#8221; community such as scientists or lawyers (assuming a high enough degree of participation). The profession-specific shared bookmarking service could very well make folksonomy development go a tad faster, within well-defined communities with a shared jargon (although I feel that jargon semantics don&#8217;t carry across subfields, with one field&#8217;s definition of a term quite at odds with another&#8217;s). [Paul Kedrosky](http://paul.kedrosky.com/archives/001085.html) will be happy to see another vertical search concept (if he doesn&#8217;t know about it already!).

Apart from the duplication of effort, which is only theoretically bad, one obvious downside of the verticalization of the tool is that people doing interdisciplinary work (e.g. scientific lawyers, aka patent lawyers) will probably suffer from the compartmentalization of the meta-data &#8212; but they&#8217;re used to it by now.

Most interesting to me is the notion that the folks at Nature may have figured out a possible new feature/concept for systems like del.icio.us. Maybe it&#8217;s worth considering the possibilities that follow from doing more in-depth analysis of the &#8220;stuff&#8221; being bookmarked, and extracting the key parts of the content of interest, as opposed to focusing (as technologists would naturally do) on the &#8220;simple bit&#8221;, i.e. the URL. After all, the URL isn&#8217;t what&#8217;s interesting &#8212; it&#8217;s the stuff in the page that is.

As an example, this morning I bookmarked the [page on gawker](http://www.gawker.com/news/media/advertising/starbucks-siren-call-of-the-damned-034705.php) that was my introduction to [the Starbucks corporate anthem](http://thestranger.com/audio/jefferson_starbucks.mp3) (warning, it&#8217;s depressing as hell). I bookmarked the page because &#8220;it was there&#8221; &#8212; but it would be nice for the system to know that what&#8217;s key about that page is the link to the MP3 file &#8212; not just the words that Gawker uses to introduce it. If others have bookmarked another page that happens to include the same link, del.icio.us wouldn&#8217;t let me know about it. A version of something like Connotea that knew about link structures might.

As my kids say, very instering.