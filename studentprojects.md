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

### Project: The HIPERFIT Portfolio Management Prototype

Please consult [the project background information](/pdf/HIPERFIT_PROTOTYPE_2016_ADDITIONAL_INFORMATION.pdf) and the [bachelor project teaser slides](/pdf/HIPERFIT_PROTOTYPE_2016.pdf).

Contact persons: [Danil Annenkov](people.html) or [Martin Elsman](people.html).

### Project: CUDA Backend for Futhark

As part of its research into parallel functional programming, HIPERFIT
has developed a programming language, Futhark, and an optimising
compiler targeting GPGPU.  Currently, the Futhark compiler generates
code using the OpenCL library.  Another popular library, CUDA, is more
widespread in scientific computing, and generated CUDA code may thus
be easier to integrate in existing systems.

This project is about writing a CUDA backend for the Futhark compiler.
Most of the optimisations are done at a higher level, and should be
reusable in the CUDA backend.  Performance of generated code should be
similar to that of the existing OpenCL backend, but we're open to
being surprised.

Contact person: [Cosmin Oancea](people.html) or [Troels Henriksen](people.html).

### Project: Compile-time Memory Allocation in Futhark

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

### Project: Adding Function-Level Shape/Invariant Annotations to Futhark

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


### Project: OpenMP Backend for a Data-Parallel Functional Programming Language

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
