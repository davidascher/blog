---
id: 696
title: Can federation be made glossy?
date: 2012-01-07T00:10:21+00:00
author: David Ascher
layout: post


restapi_import_id:
  - 5780561eab8f6
original_post_id:
  - "696"
categories:
  - Uncategorized
---
Over on twitter, I got into a weird pseudo-argument about federation and user experience.  This is the kind of topic for which Twitter conversations are particularly ill suited, so I&#8217;m &#8220;taking it to the blog&#8221;.

The simplest way of explaining the topic is as a clash of superficial values between two cultures of software design, both of which I subscribe to, and my internal struggle to try and reconcile them.

### The Technocratic View

Engineers, developers, open source advocates, &#8216;internet architects&#8217;, and &#8220;people like that&#8221; value web architectures which are not just federated (multiple cooperating parties) but decentralized and open, ideally to an extreme point.  According to this viewpoint, it should be possible for an individual (or individual organization) to host, and control (deeply) a full peer of the network. Furthermore, the internet has been possible because not only can people take implementations of software and modify them locally (cf. Free & Open Source software), but  also to have radically different implementations of these software systems, and let them compete in the &#8220;market&#8221;.  This system is what I&#8217;ll call the technocratic approach &#8212; open standards, software systems that can be modified at the edges, and a competitive market for systems which can compete on everything: features, performance, cost, ergonomics, esthetics, etc.

This, to be clear, is the approach that has led to the global success of the internet in general, but in the realm of communications, to email in particular.  Most email recipients can&#8217;t tell whether it was sent on the network by one of the mega-nodes (aol, yahoo, microsoft, google, etc.) or a tiny little server running email just for that one person.  It&#8217;s trendy to diss email these days, but without email none of the more recent stuff would have happened, so, some respect please!  Even in a contemporary context, there are deep advantages to this kind of architecture,  especially when it comes to issues of control over people&#8217;s right to communicate securely.

This radical decentralization is not problem-free, though &#8212; it makes identifying spam and other bad actors incredibly hard, and it makes &#8220;upgrading&#8221; basically impossible to do system-wide, because there&#8217;s no way to get everyone to either guarantee a new capability, or, equally hard, give up on a previously-supported behavior.  As the size of the network grows, it gets more and more rigid, which is why email, SMS, etc. all are basically functionally frozen systems.  Small groups can agree to layer on new features (e.g. encrypted emails), but it&#8217;s impossible to &#8216;upgrade email&#8217;.

In this world, decentralization is assumed; there&#8217;s a social norm to follow standards; technocrats are in charge, which helps open source approaches compete.  As the network scales, the rate of change of the standard inevitably slows (as the aggregate human and capital costs of changes become enormous).

### Design-led software creation

The other belief system to which I subscribe is that to make software for humans, one needs to deeply understand human needs, and those are radically different than digital computing systems.  In particular, disciplines like various aspects of design, user experience, psychology, consumer behaviors, and economics are as critical to the actual adoption by normals as those of software & systems engineering.  Many organizations have figured this out, Apple being the current archetype &#8212; Apple systems routinely inspire real passion from normals &#8212; they&#8217;re systems that people love to use, that make people feel good.  And so everyone tries to copy the Apple approach as best they can, trying to design experiences that can be described as shiny, glossy, sexy.  Thanks to Apple, we&#8217;re now all competing for the best designers & user researchers, looking for engineers who get design and designers who can motivate engineers.  This, in my view, is a very good thing.

However, Apple&#8217;s success has come bundled with an approach to system designed which is antithetical to some of the foundational principles of the internet.  In particular, forgetting its Apple ][ roots, modern Apple systems are exceedingly closed (I can&#8217;t even replace the battery or storage device in my latest laptop!).  Apple has asserted that, from a design point of view, open systems lead to worse experiences.  That&#8217;s why iOS devices are customizable in very limited prescribed ways (oh, I know, let&#8217;s call them Apps).  That&#8217;s why the App Store guidelines are there &#8212; to &#8220;guarantee the best user experience possible&#8221;.  And it is indeed the case that it&#8217;s easier to _control_ the outcome if you have a more closed system.  Which, bluntly, makes me sad.  Because this point, which is easiest to make by referencing Apple, is at the root of the stunning success of centralized communication systems in the 21st century.  Facebook and Twitter, to take two examples, have succeeded in part because by picking a centralized architecture, they&#8217;ve been able to sidestep huge architectural challenges, and gain huge design control.  And people have loved them to bits for it.  As much as technocrats think they rule Google, Google+ is centralized, and I would be (happily!) surprised to see Google+ adopt any meaningful decentralization just for these reasons (and the expected financial outcomes from a successful centralized outcome).

### The conventional framing

Everything I say above is fairly cliché.  One one side the technocratic approach, which argues that decentralization, open systems, open source, standards are the only ethical way to build communication systems.  On the other, design experience which has shown that closed, centralized systems have such incredible competitive advantage in terms of driving consumer behavior, that even