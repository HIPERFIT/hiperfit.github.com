---
layout: post
title: "PhD Defence: Martin Dybdal"
category: news
tags: [talk, Martin Dybdal, phd defence]
---
{% include JB/setup %}

_Title:_ Array abstractions for GPU Programming

_Thesis:_ To be published later (For an electronic copy of the thesis, please contact 'PhDadmin@di.ku.dk')

_Presenter:_ Martin Dybdal, PhD. Student, DIKU/University of Copenhagen

_Time:_ Wednesday, August 9, 2017, 13:15

_Place:_ HCØ, Auditorium 10, Universitetsparken 5, 2100 Copenhagen Ø

_Committee:_

- Associate Professor Andrzej Filinski (chairman), Department of Computer Science, University of Copenhagen, Denmark
- Associate Professor Gabriele Keller, University of New South Wales, Australia
- Professor Peter Sestoft, IT University of Copenhagen, Denmark

## Abstract

The shift towards massively parallel hardware platforms for high-performance computing tasks has introduced a need for improved programming models that facilitate ease of reasoning for both users and compiler optimization.

A promising direction is the field of functional data-parallel programming, for which functional invariants can be utilized by optimizing compilers to perform large program transformations automatically. However, the previous work in this area allow users only limited ability to reason about the performance of algorithms. For this reason, such languages have yet to see wide industrial adoption.

We present two programming languages that attempt at both supporting industrial applications and providing reasoning tools for hierarchical data-parallel architectures, such as GPUs.

First, we present TAIL, an array based intermediate language and compiler framework for compiling a large subset of APL, a language which have been used in the financial industry for decades. The TAIL language is a typed functional intermediate language that allows compilation to data-parallel platforms, thereby providing high-performance at the fingertips of APL programmers.

Second, we present FCL, a purely functional data-parallel language, that allows for expressing data-parallel algorithms in a fashion where users at a low-level can reason about data-movement through the memory hierarchy and control fusion will and will not happen. We demonstrate through a number of micro benchmarks that FCL compiles to efficient GPU code.

## Biography

Martin Dybdal is a PhD student at DIKU/University of Copenhagen
under supervision of Associate Professor Martin Elsman, DIKU.

_Host:_ DIKU and HIPERFIT (Assoc. Prof. Martin Elsman)