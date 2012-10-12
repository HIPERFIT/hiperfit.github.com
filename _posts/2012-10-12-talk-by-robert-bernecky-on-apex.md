---
layout: post
title: "Talk by Robert Bernecky on APEX"
category: news
tags: [Bernecky, APEX, SaC, APL]
---
{% include JB/setup %}

Robert Bernecky is visiting DIKU on October 22, 2012. Robert will give
a [COPLAS](www.coplas.org)/HIPERFIT talk on compilation techniques in
[APEX](http://www.snakeisland.com/apexup.htm), a compiler from APL to
[SaC](http://www.sac-home.org/). An abstract for the talk is given
below.

---

## Talk title: The Three Beaars
### Basically, Every Array Allocation Reduces Speed

### Robert Bernecky
### Snake Island Research Inc

### Monday October 22, 10:30am-11:30am
### DIKU Meeting Room A/B

## Abstract

Functional array language compiler and interpreter designers try to
reduce the number of arrays created during application execution,
because the negative impact of arrays on performance is so dramatic.
Just as The Three Bears had different requirements for their own
satisfaction, so do differing array shapes have different requirements
for their elimination. The problem itself is a bear: scalar operations
are the baby bear, typified here by dynamic programming and the
Floyd-Warshall algorithm; operations on small arrays, such as
numerically intense computations on complex arrays, is the mama bear;
operations on large arrays, typified by acoustic signal processing, is
the papa bear.  We compare interpreted to compiled APL performance for
several applications with different array shapes, and give an overview
of the various optimizations that enable those speedups, in both
serial and parallel contexts.

## Biography

Robert Bernecky has designed and developed APL systems since 1971.
While at I.P. Sharp Associates Limited, he was one of the people
responsible for the design and development of SHARP APL, a system that
set the standard for performance of large-scale APL systems.  He has
authored papers on language design, algorithm design, and interpreter
performance.

Bernecky is the CEO of Snake Island Research Inc, a consulting and
research firm headquartered in Toronto.

Bernecky developed APEX -- the APL Parallel Executor -- a high-
performance, retargetable APL compiler for serial and parallel
computers.

Bernecky holds a BA in philosophy from SUNY at Buffalo, an MSc in
Computer Science from the University of Toronto, and is trying to
finish his PhD before his PhD finishes him.  He is a member of ACM and
IEEE.
