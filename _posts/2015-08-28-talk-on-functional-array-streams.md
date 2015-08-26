---
layout: post
title: "Talk on Functional Array Streams"
category: news
tags: [talk]
---
{% include JB/setup %}

## HIPERFIT Talk: Functional Array Streams

_Presenter:_ Frederik Meisner Madsen, PhD student, DIKU/University of Copenhagen

_Time:_ Friday August 28, 2015, 13-14

_Place:_ The APL Meeting Room (DIKU, HCØ, Universitetsparken 5; room 01-0-029)

## Abstract:

Regular array languages for high performance computing based on
aggregate operations provide a convenient parallel programming model,
which enables the generation of efficient code for SIMD architectures,
such as GPUs. However, the data sets that can be processed with
current implementations are severely constrained by the limited amount
of main memory available in these architectures.

In this paper, we propose an extension of the embedded array language
Accelerate with a notion of sequences, resulting in a two level
hierarchy which allows the programmer to specify a partitioning
strategy which facilitates automatic resource allocation. Depending on
the available memory, the runtime system processes the overall data
set in streams of chunks appropriate to the hardware parameters.

In this paper, we present the language design for the sequence
operations, as well as the compilation and runtime support, and
demonstrate with a set of benchmarks the feasibility of this approach.

## Biography

Frederik Meisner Madsen is a PhD student at the HIPERFIT research
center where he is involved in programming language
research. Particular areas of interest include functional array
languages, nested data-parallelism and streaming.

_Host:_ Martin Elsman