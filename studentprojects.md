---
title: Student Projects
layout: page
group: navigation
---
{% include JB/setup %}

This page lists a series of suggested student projects within
HIPERFIT. For more information about the possibilities, please talk to
the appropriate contact persons.

### Project: OpenMP backend for data-parallel functional programming language

As part of its research into parallel functional programming, HIPERFIT
has developed a programming language, Futhark, and an optimising
compiler.  This project is about developing a compiler backend that
generates code using [OpenMP](http://en.wikipedia.org/wiki/OpenMP) to
achieve multi-core CPU parallelism.

Contact person: [Cosmin Oancea](people.html) (or [Troels Henriksen](people.html)).

[more >>](studentproject_openmp_backend.html).

### Project: Structural Description Language

As part of its research into parallel functional programming, HIPERFIT
has developed a programming language, L0, and an optimising compiler.
This project is about designing and implementing a schema-like
description language for recursive syntax trees, then use it to write
tests that specify the desired high-level structure of the optimised
program.

Contact person: [Cosmin Oancea](people.html) (or [Troels Henriksen](people.html)).

[more >>](studentproject_structural_description_language.html).

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

### Project: Haskell Library for Finance

This project is about constructing a modular library in Haskell for
pricing financial contracts and portfolios – either solely based on
so-called closed-form functions or also coupled with Monte Carlo
simulations. The main focus is to work on code structure and code
architecture to reach a proof-of-concept level. 

Contact person: [Jost Berthold](people.html) (joint supervision with Sinan Gabel).

[more >>](studentproject_haskell_library_finance.html).

### Project: Parallel Monte Carlo Simulations in Haskell

This project is about constructing a Monte Carlo simulation library in
Haskell. The library should be structured to allow for different
statistical distributions (e.g. the Gaussian normal and log-normal) and
for parallel execution. Consideration should be given to parallel
calculations such that each thread generates random numbers that are
independent from the other threads' calculations. The generator should
be deterministic if given the same initialisation i.e. given the same
so-called seed value - in other words given a certain seed value the
generator simulates the same pseudo-random numbers.

Contact person: [Jost Berthold](people.html) (joint supervision with Sinan Gabel).

[more >>](studentproject_haskell_montecarlo.html).
