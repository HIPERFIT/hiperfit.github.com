---
layout: post
title: "PhD Defence: Troels Henriksen"
category: news
tags: [talk, Troels Henriksen, Futhark, phd defence]
---
{% include JB/setup %}

_Title:_ Design and Implementation of the Futhark Programming Language

_Thesis:_ To be published later (For an electronic copy of the thesis, please contact 'PhDadmin@di.ku.dk')

_Presenter:_ Troels Henriksen, PhD. Student, DIKU/University of Copenhagen

_Time:_ Wednesday, November 15, 2017, 13:15

_Place:_ HCØ, Auditorium 6, Universitetsparken 5, 2100 Copenhagen Ø

_Committee:_

- Associate Professor Torben Mogensen (Chairman), Department of Computer Science, University of Copenhagen, Denmark
- Professor Mary Sheeran, Chalmers University of Technology, Sweden
- Professor Alan Mycroft, University of Cambridge, United Kingdom

## Abstract

In this thesis we describe the design and implementation of Futhark, a small data-parallel purely functional array language that offers a machine-neutral programming model, and an optimising compiler that generates efficient OpenCL code for GPUs.  The overall philosophy is based on seeking a middle ground between functional and imperative approaches. The specific contributions are as follows:

First, we present a moderate flattening transformation aimed at enhancing the degree of parallelism, which is capable of exploiting easily accessible parallelism. Excess parallelism is efficiently sequentialised, while keeping access patterns intact, which then permits further locality-of-reference optimisations. We demonstrate this capability by showing instances of automatic loop tiling, as well as optimising memory access patterns.

Second, to support the flattening transformation, we present a lightweight system of size-dependent types that enables the compiler to reason symbolically about the size of arrays in the program, and that reuses general-purpose compiler optimisations to infer relationships between sizes.

Third, we furnish Futhark with novel parallel combinators capable of expressing efficient sequentialisation of excess parallelism, as well as their fusion rules.

Fourth, in order to express efficient programmer-written sequential code inside parallel constructs, we introduce support for safe in-place updates, with type system support to ensure referential transparency and equational reasoning.

Fifth, we perform an evaluation on 21 benchmarks that demonstrates the impact of the language and compiler features, and shows application-level performance that is in many cases competitive with hand-written GPU code.

Sixth, we make the Futhark compiler freely available with full source code and documentation, to serve both as a basis for further research into functional array programming, and as a useful tool for parallel programming in practise.

## Biography

Troels Henriksen is a PhD student at DIKU/University of Copenhagen
under supervision of Professor Fritz Henglein, DIKU and (co-supervisor) Assistant Professor Cosmin Oancea, DIKU.

_Host:_ DIKU and HIPERFIT