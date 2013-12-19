---
title: Student Projects
layout: page
group: navigation
---
{% include JB/setup %}

This page lists a series of suggested student projects within
HIPERFIT. For more information about the possibilities, please talk to
the appropriate contact persons.

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
