---
layout: post
title: "Talk on Compiling APL to Accelerate"
category: news
tags: [talk,seminar]
---
{% include JB/setup %}

## HIPERFIT Seminar Talk: Compiling APL to Accelerate through a Typed Array Intermediate Language

_Presenter:_ Michael Budde, MSc student, DIKU/University of Copenhagen

_Time:_ Tuesday June 9, 2015, 15-16

_Place:_ Aud 07 (HCØ, Universitetsparken 5)

## Abstract:

In this talk, we present an approach for compiling a rich subset of
APL into data-parallel programs that can be executed on GPUs. The
compiler is based on the APLTail compiler, which compiles APL programs
into a typed array intermediate language, called TAIL. We translate
TAIL programs into Haskell source code, employing Accelerate, a
Haskell-library for general purpose GPU-programming. We demonstrate
the feasibility of the approach by presenting some encouraging results
for a number of smaller benchmarks. We also outline some problems that
we need to overcome in order for the approach to result in competitive
code for larger benchmarks.

## Biography

Michael Budde is an MSc student at University of Copenhagen, DIKU. The
talk is based on joined work with Martin Dybdal and Martin Elsman,
DIKU. The work is presented at the [ARRAY'15 workshop](http://www.sable.mcgill.ca/array/) in Portland,
Oregon, later in June.

_Host:_ Martin Elsman