---
layout: post
title: "Talk by Amos Robinson on Fusion"
category: news
tags: [visit, talk, fusion, Amos Robinson]
---
{% include JB/setup %}

__Fusing Filters with Integer Linear Programming__

Amos Robinson, University of New South Wales, Sydney, Australia.

Time and location: August 26, 12:15-13:00. The APL meeting room, DIKU, Universitetsparken 5, Building B, 2100 Copenhagen Ø.

To attend the talk, please signup by email to Martin Elsman (mael at di.ku.dk).

__Abstract:__

The key to compiling functional, collection oriented array programs
into efficient code is to minimise memory traffic. Greedily fusing
array operations together can reduce some memory traffic, but finding
the fusion clustering that produces the least amount of memory traffic
turns out to be NP-hard.  Integer linear programming (ILP) can be used
to solve NP-hard problems, by finding the minimal solution for a given
cost metric. Previous work has used ILP to find fusion clusterings for
certain graphs, however these approaches cannot handle size-changing
operations such as filter. In this talk, I will show how size-changing
operations differ, and how we have extended previous work to support
such operations.

__Bio:__

Amos Robinson is a PhD student at University of New South Wales,
Sydney, Australia. His focus is on optimisation and fusion in purely
functional programming languages such as Haskell. He was also the
winner of the inaugural Sydney Coq Fight, a theorem proving
tournament.
