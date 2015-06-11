---
layout: post
title: "Talks on Streaming in Data Parallelism"
category: news
tags: [talk,seminar]
---
{% include JB/setup %}

## HIPERFIT Seminar Talks: Streaming in Data Parallelism

_Presenters:_ Andrzej Filinski (Associate Professor, DIKU) and Frederik Meisner Madsen (PhD Student, DIKU)

_Time:_ Tuesday, April 24, 15:00-16:00

_Place:_ Aud 07 (HCØ, Universitetsparken 5)

## Abstracts:

The presentation will consist of two shorter talks:

_Streaming NESL (speaker: Andrzej Filinski, associate professor, DIKU)_

Streaming NESL, under development in the HIPERFIT Center, is a
refinement of the nested data-parallel functional language NESL.  It
extends NESL's flattening-based implementation strategy and
language-integrated cost model for time (in the form of work and step
measures) to also achieve predictable (and optimistic) bounds for
space usage.  This is done by avoiding complete materialization of
intermediate vector-typed values that do not actually require random
access. Instead, such values are transparently materialized and
processed in "chunks", of size proportional to the available parallel
computing resources - from SIMD instructions on single-core CPUs to
large GPGPUs.

We give an overview of the status of the project, including a summary
of the source language and cost model, a sketch of the implementation
strategy in terms of a chunked-dataflow abstract machine (which may
also be relevant to other language-technology projects within
HIPERFIT), and an outline of some current challenges, both theoretical
and practical.

_Streaming Accelerate (speaker: Frederik Meisner Madsen, PhD student, DIKU)_

The relatively mature embedded language Accelerate brings the power of
hardware-accelerated, shape-polymorphic programming with regular
arrays to Haskell. Extending Accelerate with streaming functionality,
along the lines of our current research, will hypothetically improve
its usability and performance for many important use-cases. This talk
presents an extension to Accelerate that enables streaming by lifting
a non-trivial subset of the language from working on arrays to working
on sequences of arrays. The programmer obtains a sequence by slicing
an array into a sequence of sub-arrays, and may return to ordinary
Accelerate through reduction. Sequence expressions are evaluated
efficiently in fixed-size chunks by reusing memory and compiled
kernels, allowing sequences to scale in length without requiring
additional computing resources except computation time.