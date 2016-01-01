---
title: Student Projects
layout: page
group: navigation
---
{% include JB/setup %}

This page lists a series of suggested student projects within
HIPERFIT. For more information about the possibilities, please talk to
the appropriate contact persons.

### Bachelor Projects

Please consult [the project announcement](/news/2015/08/25/bachelor-projects/) and the [bachelor project teaser slides](/pdf/HIPERFIT_PROTOTYPE_2015.pdf).

Contact persons: [Danil Annenkov](people.html) or [Martin Elsman](people.html).

### Project: Compile-time memory allocation in Futhark

As part of its research into parallel functional programming, HIPERFIT
has developed a programming language, Futhark, and an optimising
compiler targeting GPGPU.  During the later stages of the compilation
pipeline, the Futhark compiler will insert explicit memory allocations
in the program being compiled, and add annotations indicating in which
memory a given array is stored.  This decoupling of arrays from memory
permits memory-level optimisations, such as hoisting allocations out
of inner loops.

This project is about moving further with optimisations on this
representation.  Specifically, we conjecture that an algorithm similar
to register allocation can be devised which would allow different
arrays to be located in the same memory block, as long as the arrays
are never live at the same time.  This optimisation will not only
reduce total memory usage in the generated code, but also reduce the
number of memory copy operations.

This project is a good fit for a bachelor's project.  It involves a
good bit of both hacking and clever algorithmic thinking, and the
effect of the work can be directly measured in reduced memory load and
increased performance.  It is also a good way to get involved with
compiler work.

Contact person: [Cosmin Oancea](people.html) or [Troels Henriksen](people.html).

### Project: Map-Scan loop fusion in Futhark

*Loop fusion* is an optimisation technique that combines several loops
into one, which can result in less space usage, as intermediary arrays
need no longer be constructed, as well as result in tighter code.
This project is about improving the fusion capabilities in Futhark, a
DIKU-developed data-parallel purely functional language aimed at
high-performance GPGPU code.

When generating GPGPU code for reductions, it has been observed that
the optimal structure is often one where every thread first performs
sequential reduction on a chunk of the input, followed by parallel
reduction where the threads combine their work.  The function used for
the sequential phase does not have to respect the usual properties
required for parallel reductions (notably associativity), which can be
exploited to permit aggressive fusion into the sequential phase.  We
believe that the same technique could also be applied to parallel
scans.

This project is a good entry point for getting into compiler hacking.
It is suitable for both bachelor's projects and ad-hoc 7.5 ECTS
projects.

Contact person: [Cosmin Oancea](people.html) or [Troels Henriksen](people.html).

### Project: Efficient Histogram Computation on GPGPUs

The code below shows an example of histogram computation:
function "f" computes based on the current index and 
input-array element several (key,value) pairs such as
the sum of values is 1. The (key,value) pairs are used
to update the histogram.  

    do i=0, N-1
        (key1,key2,val1,val2) = f(i, a[i]);
        h[key1] += val1;
        h[key2] += val2; // where val1+val2 = 1.0
    enddo


The project is about doing this computation efficiently on GPUs.

Contact person: [Cosmin Oancea](people.html) or [Troels Henriksen](people.html).

### Project: Adding Function-Level Shape/Invariant Annotatations in Futhark

As part of its research into parallel functional programming, HIPERFIT
has developed a programming language, Futhark, and an optimising
compiler.  This project is about allowing the user to annotate, at function
level, algebraic invariants between integer parameters, which for example, 
may allow the compiler to accurately determine array shapes, and further
on to hoist allocations outside of recurrences.  Just to get an idea, an
annotated function can possibly look like:

    fun [([int,k1], char, [bool,k2]), k3]
        myFun(int M, int N, [[real, k4],M] arr)
                where { k1 < k2, 
                        k3 in k2*k1 + N ... M,
                        k4 < M + N,
                        M >= MAX(2*N,0),
                        arr in N ... M-1 } = 
        body of function

where k1, k2, k3, k4 are existentially qualified under the constraints
appearing in the where clause.


Contact person: [Cosmin Oancea](people.html) or [Troels Henriksen](people.html).


### Project: OpenMP backend for data-parallel functional programming language

As part of its research into parallel functional programming, HIPERFIT
has developed a programming language, Futhark, and an optimising
compiler.  This project is about developing a compiler backend that
generates code using [OpenMP](http://en.wikipedia.org/wiki/OpenMP) to
achieve multi-core CPU parallelism.

Contact person: [Cosmin Oancea](people.html) (or [Troels Henriksen](people.html)).


### Project: Optimization of a Haskell Automatic Differentiation Library

Esben Halvorsen describes in his MSc project [Calculating Key Ratios
for Financial Products using Automatic Differentiation and Monte Carlo
Simulation](/pdf/ad_esben.pdf), how to construct a
Haskell framework for Automatic Differention (AD), which turns out to
be useful for calculating "the greeks" (key ratios) for financial
products. The framework has been implemented in Haskell and the
project report outlines a series of possibilities for optimizations,
including an improved representation of arrays. This project is about
investigating the possibilities for optimization of the AD framework,
possibly for pricing and calculating greeks on parallel hardware.

Supervisor: [Martin Elsman](http://www.elsman.com)

### Project: APL parsing in Haskell

APL is an array programming language from the 60's, which turns out to
have interesting language constructs for programming with arrays for
parallel hardware. Although APL is nowadays not widely adopted as the
programming language of choice for large corporations, APL is still
used in industry, for instance, in the danish company (and HIPERFIT
partner) [SimCorp](http://www.simcorp.com), which has large parts of their
code base written in APL. This project is about designing and
constructing an APL-parser in Haskell. For inspiration, a parser for
APL, written in Standard ML, is [available at
github](https://github.com/melsman/aplparse).

Supervisor: [Martin Elsman](http://www.elsman.com)
