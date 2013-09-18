---
title: Student Project - Haskell Library for Finance
layout: page
group: student projects
---
{% include JB/setup %}

This project is about constructing a modular library in Haskell for
pricing financial contracts and portfolios – either solely based on
so-called closed-form functions or also coupled with Monte Carlo
simulations. The main focus is to work on code structure and code
architecture to reach a proof-of-concept level. 

### Contact person

Jost Berthold (joint supervision with Sinan Gabel).

### Notes

The present value of a cash flow is basically found by discounting the
cash flow to the present, so a general structure should allow for e.g.
different discount functions and different cash flows. This may seem
simple but becomes more complicated when financial instruments allow for
e.g. optionality elements i.e. cash flows that are paid/received
contingent on particular events, and uncertainty is present in the
discounting function (i.e. the term structure of interest rates is
uncertain).

### Key topics

Functional programming, Haskell, Parallel computations. Finance, Valuation.

### Input

A (commercial) working pricing and financial library written in
Mathematica “Derivatives Expert IV for Mathematica”. The library has
accommodating examples, documentation and test files. A .pdf version of
the documentation can be found at
[http://ifs.dk/DerivativesExpert/DerivativesExpertManual.pdf](http://ifs.dk/DerivativesExpert/DerivativesExpertManual.pdf)

### Prerequisites

Capable of writing small and middle sized applications in Haskell (GHC).
Getting a basic understanding of some key financial concepts such as
cash flows and discounting functions during the course of the project.

