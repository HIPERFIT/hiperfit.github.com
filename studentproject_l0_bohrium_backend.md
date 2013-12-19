---
title: Student Project - Bohrium backend for L0
layout: page
group: studentprojects
---
{% include JB/setup %}

As part of its research into parallel functional programming, HIPERFIT
has developed L0, a simple purely functional data-parallel language
intended as an intermediate representation.  At the same time, the
high-performance computing group has developed Bohrium, a vectorised
bytecode system enabling parallel execution on GPUs, clusters and
other parallel platforms.  This project is about constructing a
Bohrium backend for the L0 compiler, bridging the two projects.

### Contact person

[Cosmin Oancea](people.html) (or [Troels Henriksen](people.html)).

### Notes

The current L0 compiler performs various high-level optimisations
(such as fusion, hoisting and constant-folding), but the only finished
backend generates rather naive sequential C code.  Rather than
duplicating the work done by the Bohrium developers, we would like to
leverage their results, as well as take advantage of current and
future low-level optimisations done by Bohrium.

In L0, all bulk operations on data is performed via so-called
"second-order array combinators" (SOACs), such as `map`, `reduce` or
`scan`, with a great deal of flexibility in their function arguments.
A single Bohrium instruction can only express a simple bulk
computation (such as adding two arrays), and a significant part of the
project will thus be developing ways to decompose a complex `map` into
simpler vectorised operations.

An embryonic, incomplete version of the backend has already been
developed, and is suggested (but not required) as a starting point.

### Key topics

Functional programming, Haskell, Compilers, High-performance computing.

### Input

A description of L0 is available in the paper ["A T2 Graph-Reduction
Approach To Fusion"](pdf/fhpc13_troels.pdf).  The paper ["Bohrium:
Unmodified NumPy Code on CPU, GPU, and Cluster"](pdf/Bohrium.pdf) is
an introduction to Bohrium.

The [code for Bohrium is available on
Bitbucket](https://bitbucket.org/bohrium/bohrium) and [documentation
as well](http://bohrium.bitbucket.org/developers/index.html), and we
hope to make the L0 compiler available as well.

### Prerequisites

Capable of writing small and middle sized applications in Haskell
(GHC), as well as a moderate understanding of C.  Understanding of
basic compiler technology (equivalent to taking DIKUs compiler course
and enjoying it).
