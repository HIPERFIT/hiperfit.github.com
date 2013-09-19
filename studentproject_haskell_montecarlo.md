---
title: Student Project - Parallel Monte Carlo Simulations in Haskell
layout: page
group: studentprojects
---
{% include JB/setup %}

This project is about constructing a Monte Carlo simulation library in
Haskell. The library should be structured to allow for different
statistical distributions (e.g. the Gaussian normal and log-normal) and
for parallel execution. Consideration should be given to parallel
calculations such that each thread generates random numbers that are
independent from the other threads' calculations. The generator should
be deterministic if given the same initialisation i.e. given the same
so-called seed value - in other words given a certain seed value the
generator simulates the same pseudo-random numbers.

### Contact person

[Jost Berthold](people.html) (joint supervision with Sinan Gabel)

### Notes

An estimate of an expected value of a function F can be obtained by
generating/simulating values from the desired statistical distribution,
and finding the mean of F applied to those values. This provides
relatively easy access to valuing financial contracts.

A random walk can be created by recursively summing pseudo-random numbers.

Its use can vary widely but test cases will be directed towards valuing
financial contracts.

### Key topics

Functional programming, Haskell, Parallel computations.

Monte Carlo method (statistics), pseudo-random uniformly distributed
numbers (reals, integers), Seed value (for the random generator).

Finance, Valuation.

### Input

A (commercial) working Monte Carlo (non-parallel) simulation library
written in Mathematica “Derivatives Expert IV for Mathematica”
(relevant part is module/package 18). The library has accommodating
examples, documentation and test files. A .pdf version of the
documentation can be found at
[http://ifs.dk/DerivativesExpert/DerivativesExpertManual.pdf](http://ifs.dk/DerivativesExpert/DerivativesExpertManual.pdf);
see pages 309-326.

Gentle, J. E. Random Number Generation and Monte Carlo Methods, 2nd ed.
Springer-Verlag, 2003.

http://en.wikipedia.org/wiki/Monte_Carlo_method

### Prerequisites

Capable of writing small and middle sized applications in Haskell (GHC).
Understand basic statistics.