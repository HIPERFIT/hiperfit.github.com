---
layout: post
title: "PhD Defence: Frederik Meisner Madsen"
category: news
tags: [talk, Frederik Meisner Madsen, phd defence]
---
{% include JB/setup %}

_Title:_ Streaming for Functional Data-Parallel Languages

_Presenter:_ Frederik Meisner Madsen, PhD. Student, DIKU/University of Copenhagen

_Time:_ Thursday, December 15, 2016, 13:15

_Place:_ Room Aud 05, HCØ, Universitetsparken 5, 2100 Copenhagen Ø

_Committee:_

- Assocociate Professor Martin Elsman (chairman), DIKU, University of Copenhagen
- Professor John Reppy, Department of Computer Science, University of Chicago, USA
- Professor Mary Sheeran, Department of Computer Science and Engineering, Chalmers University of Technology, Sweden

_Thesis (revised):_ [pdf](/pdf/meisner_madsen_thesis_revised.pdf)

## Abstract

In this thesis, we investigate streaming as a general solution to the
space inefficiency commonly found in functional data-parallel
programming languages. The data-parallel paradigm maps well to
parallel SIMD-style hardware. However, the traditional fully
materializing execution strategy, and the limited memory in these
architectures, severely constrains the data sets that can be
processed. Moreover, the language-integrated cost semantics for nested
data parallelism pioneered by NESL depends on a parallelism-flattening
execution strategy that only exacerbates the problem. This is because
flattening necessitates all sub-computations to materialize at the
same time. For example, naive n by n matrix multiplication requires
n^3 space in NESL because the algorithm contains n^3 independent
scalar multiplications. For large values of n, this is completely
unacceptable.

We address the problem by extending two existing data-parallel
languages: NESL and Accelerate. In the extensions we map bulk
operations to data-parallel streams that can evaluate fully
sequential, fully parallel or anything in between. By a dataflow,
piecewise parallel execution strategy, the runtime system can adjust
to any target machine without any changes in the specification. We
expose streams as sequences in the frontend languages to provide the
programmer with high-level information and control over streamable and
non-streamable computations. In particular, we can extend NESL's
intuitive and high-level work–depth model for time complexity with
similarly intuitive and high-level model for space complexity that
guarantees streamability.

Our implementations are backed by empirical evidence. For Streaming
Accelerate we demonstrate performance on par with Accelerate without
streams for a series of benchmark including the PageRank algorithm and
a MD5 dictionary attack algorithm. For Streaming NESL we show that for
several examples of simple, but not trivially parallelizable,
text-processing tasks, we obtain single-core performance on par with
off-the-shelf GNU Coreutils code, and near-linear speedups for
multiple cores.

_Notice:_ For an electronic copy of the thesis, please contact [phdadmin@di.ku.dk](phdadmin@di.ku.dk).

## Biography

Frederik Meisner Madsen is a PhD student at DIKU/University of Copenhagen
under supervision of Associate Professor Andrzej Filinski, DIKU.

_Host:_ DIKU and HIPERFIT (Associate Professor Andrzej Filinski)