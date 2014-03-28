---
title: Student Projects
layout: page
group: navigation
---
{% include JB/setup %}

This page lists a series of suggested student projects within
HIPERFIT. For more information about the possibilities, please talk to
the appropriate contact persons.

### Optimization of a Haskell Automatic Differentiation Library

Esben Halvorsen describes in his MSc project [Calculating Key Ratios
for Financial Products using Automatic Differentiation and Monte Carlo
Simulation](http://hiperfit.dk/pdf/ad_esben.pdf), how to construct a
Haskell framework for Automatic Differention (AD), which turns out to
be useful for calculating "the greeks" (key ratios) for financial
products. The framework has been implemented in Haskell and the
project report outlines a series of possibilities for optimizations,
including an improved representation of arrays. This project is about
investigating the possibilities for optimization of the AD framework,
possibly for pricing and calculating greeks on parallel hardware.

Supervisor: [Martin Elsman](http://www.elsman.com)

### APL parsing in Haskell

APL is an array programming language from the 60's, which turns out to
have interesting language constructs for programming with arrays for
parallel hardware. Although APL is nowadays not widely adopted as the
programming language of choice for large corporations, APL is still
used in industry, for instance, in the danish company (and HIPERFIT
partner) [SimCorp](www.simcorp.com), which has large parts of their
code base written in APL. This project is about designing and
constructing an APL-parser in Haskell. For inspiration, a parser for
APL, written in Standard ML, is [available at
github](https://github.com/melsman/aplparse).

Supervisor: [Martin Elsman](http://www.elsman.com)

### Project: Bohrium Backend for L0

As part of its research into parallel functional programming, HIPERFIT
has developed L0, a simple purely functional data-parallel language
intended as an intermediate representation.  At the same time, the
high-performance computing group has developed Bohrium, a vectorised
bytecode system enabling parallel execution on GPUs, clusters and
other parallel platforms.  This project is about constructing a
Bohrium backend for the L0 compiler, bridging the two projects.

Contact person: [Cosmin Oancea](people.html) (or [Troels Henriksen](people.html)).

[more >>](studentproject_l0_bohrium_backend.html).

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
