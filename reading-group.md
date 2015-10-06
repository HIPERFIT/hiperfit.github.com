---
title: HIPERFIT Reading group
layout: page
---

## Description

This page documents the activities of the HIPERFIT reading group,
which was initiated in April 2015. We meet on tuesdays from 13:00 to
15:00 (approx.) following the schedule below. The schedule will be
updated continuously.

### Time usage

The reading group will run for 23 times, with an expected time usage
around 8 hours for each session (including preparation), which will
total 184 hours, which should correspond to 7.5 ECTS.

### Topics
We will be reading papers in several topics in the core area of
HIPERFIT, namely functional programming languages for financial IT.

 * Programming language design for parallel programming
 * Type systems for array based languages (e.g. dependent types)
 * high-performance computing optimizations and algorithms.
 * Automatic/algorithmic differentiation
 * Finance and monte-carlo simulation

### Participants
 * Troels Henriksen (Ph.D. student)
 * Danil Annenkov (Ph.D. student)
 * Frederik Meisner Madsen (Ph.D. student)
 * Martin Dybdal (Ph.D. student)
 * Andrzej Filinski (Supervisor)
 * Martin Elsman (Supervisor)
 * Cosmin Oancea (Supervisor)

Other HIPERFIT faculty and students are welcome to participate in the
meetings on voluntary basis.


##Schedule (2015)

### Type systems for array languages
 * April 7th QUBE (Discussion lead by Martin Elsman and Martin Dybdal)
   * "QUBE - Dependently typed array programs don't go wrong" (JLAP, 2009) - <http://www.sciencedirect.com/science/article/pii/S1567832609000411>
   * "QUBE - Array Programming With Dependent Types" (Ph.D. dissertation) - <http://www.students.informatik.uni-luebeck.de/zhb/ediss1099.pdf>
 * April 14th (Discussion lead by Danil Annenkov)
   * "From Contracts Towards Dependent Types: Proofs by Partial Evaluation" - <http://link.springer.com/chapter/10.1007%2F978-3-540-85373-2_15>
 * April 21st (Discussion lead by Martin Dybdal)
   * "An Array-oriented language with Static Rank Polymorphism" - <http://dx.doi.org/10.1007/978-3-642-54833-8_3>
 * April 28th
   * "Dependent Types in Practical Programming" - http://www.cs.bu.edu/~hwxi/academic/papers/popl99.pdf

### Program optimisation (preliminary plan)
 * May 5th (Discussion lead by Troels Henriksen)
   * "A framework for enhancing data reuse via associative reordering" - <http://dl.acm.org/citation.cfm?id=2594342>
 * May 12th (Discussion lead by Frederik)
   * "Optimising Purely Functional GPU Programs" (skip Section 3) - <http://www.cse.unsw.edu.au/~tmcdonell/papers/acc-optim-icfp2013.pdf>
   * "Embedding Foreign Code" - <https://www.cse.unsw.edu.au/~chak/papers/acc-ffi.pdf>

   * Skim: "High-Performance Code Generation for Stencil Computations on GPU Architectures" <http://www.cs.ucla.edu/~pouchet/doc/ics-article.12.pdf>
 * May 19th
   * Cancelled
 * May 26th
   * "Automatic Parallelization in the Polytope Model" <http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.39.3581>

 * June 2nd (Discussion lead by Martin Elsman)
   * "Region-based memory management for GPU programming languages: enabling rich data structures on a spartan host" <http://dl.acm.org/citation.cfm?id=2660244>

 * August 25th
   * SaC JFP paper - <http://dl.acm.org/citation.cfm?id=967501>

 * October 13th

   * [A provable time and space efficient implementation of NESL](http://dl.acm.org/citation.cfm?id=232650)


### Finance / Automatic Differentiation

 * September 15th
 
   * Esben Bistrup Halvorsen. "Calculating Key Ratios for Financial Products using Automatic Differentiation and Monte Carlo Simulation" - http://hiperfit.dk/pdf/ad_esben.pdf - Martin Elsman

   * White-paper: Structured products desks join the AAD revolution - <http://www.fincad.com/sites/default/files/wysiwyg/Structured%20products%20desks%20join%20the%20AAD%20revolution.pdf>

 * September 22th (Jumping a way from finance for one week)

   * Draft-paper: "A Haskell EDSL for Nested Data-parallel Design-space exploration on GPUs" <http://www.cse.chalmers.se/edu/year/2014/course/DAT280_Parallel_Functional_Programming/exploration-draft-Obsidian.pdf>

   * And their own reflections: <http://www.cse.chalmers.se/edu/course/DAT280_Parallel_Functional_Programming/LectureGPU115.pdf>

 * September 29th (Back with some more Finance)

   * "Valuing American Options by Simulation: A Simple Least Approach" (Longstaff and Schwartz): <https://people.math.ethz.ch/~hjfurrer/teaching/LongstaffSchwartzAmericanOptionsLeastSquareMonteCarlo.pdf>


## Suggestions

If you add a topic, please include your name

### Finance, automatic differentiation, Monte-Carlo simulations etc.

 * "Parallel random numbers: as easy as 1, 2, 3" - http://dx.doi.org/10.1145/2063384.2063405 - Martin Dybdal

 * Andreas Griewank, Andrea Walther, "Evaluating Derivatives: Principles and Techniques of Algorithmic Differentiation" -- det er en bog; jeg har den på mit kontor (fra KUBIS). - Fritz Henglein

 * ("Specialising Simulator Generators for High-Performance Monte-Carlo Methods" - http://dx.doi.org/10.1007/978-3-540-77442-6_9 - Martin Dybdal)

### High-performance computing

 * "Rodinia: A benchmark suite for heterogeneous computing" - http://dx.doi.org/10.1109/IISWC.2009.5306797 - Martin Dybdal

 * "A characterization of the Rodinia benchmark suite with comparison to contemporary CMP workloads" - http://dx.doi.org/10.1109/IISWC.2010.5650274 - Martin Dybdal

 * "Software Pipelined Execution of Stream Programs on GPUs" - http://dx.doi.org/10.1109/CGO.2009.20 - Martin Dybdal

 * Obsidian

### Optimisation

Trying to stick to something that has general value, rather than one-off hacks - Troels

 * "Effective Automatic Data Allocation for Parallelization of Affine Loop Nests" - http://www.csa.iisc.ernet.in/TR/2014/2/tech-report.pdf - Troels Henriksen

 * "Metrics and Models for Reordering Transformations" - http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.83.6624 - Troels Henriksen

 * "Automatic Generation of Peephole Superoptimizers" - http://embedded.cse.iitd.ac.in/~sbansal/pubs/asplos06.pdf (maybe also Massalin, 1987) - Martin Dybdal

## Other topics:

 * [Automatically Improving Accuracy for Floating Point Expressions](http://delivery.acm.org/10.1145/2740000/2737959/p1-panchekha.pdf)

 * Flattening, NESL, VCODE
 * CUDA PTX
 * Something on the architecture of Xeon Phi? - Martin Dybdal
 * Hierarchical cost-models - Martin Dybdal
 * "Fission" / Bohrium

## Decided not to read

 *  "pocl: A Performance-Portable OpenCL Implementation" - http://link.springer.com/article/10.1007/s10766-014-0320-y
