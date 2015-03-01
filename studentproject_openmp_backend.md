---
title: Student Project - OpenMP backend for a data-parallel functional programming language
layout: page
group: studentprojects
---
{% include JB/setup %}

As part of its research into parallel functional programming, HIPERFIT
has developed a programming language, Futhark, and an optimising
compiler.  This project is about developing a compiler backend that
generates code using [OpenMP](http://en.wikipedia.org/wiki/OpenMP) to
achieve multi-core CPU parallelism.

### Contact person

[Cosmin Oancea](people.html) (or [Troels Henriksen](people.html)).

### Notes

The Futhark compiler already supports a range of both high- and
low-level optimisations, ranging from loop fusion, over bounds check
elimination, to memory allocation optimisations.  However, as of this
writing, the only extant code generation backend generates sequential
C code, which is then compiled to final machine code using a C
compiler.  While work is ongoing on development of a parallel GPU
backend, using OpenMP to obtain parallel multicore CPU code could
provide good speedup for many applications, at a rather modest
development cost.

The most direct approach in this project would be to extend the
current C code generator to generate OpenMP parallelism annotations.
However, some work will also be necessary on the intermediate steps in
the compiler to ensure that the parallel invariants from the original
data-parallel functional code are maintained throughout the entire
compiler pipeline.

### Key topics

Functional programming, Haskell, code generation

### Input

A description of Futhark is available in Troels's master thesis
["Exploiting Functional Invariants to Optimise Parallelism: a dataflow
approach"](/pdf/TroelsMSc.pdf) (although note that Futhark is called
L0 in this document).

The [Futhark compiler is available on
Github](https://github.com/HIPERFIT/futhark).

### Prerequisites

The Futhark compiler is implemented in Haskell, and some experience
working with Haskell or another functional programming language is
recommended.  Also recommended is understanding of basic compiler
technology (equivalent to taking DIKUs compiler course and enjoying
it).
