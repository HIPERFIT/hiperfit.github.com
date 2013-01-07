---
layout: post
title: "HIPERFIT seminar in February postponed"
category: news
tags: [clouds, pricing]
---
{% include JB/setup %}

It is time to inform about our HIPERFIT seminar in February. However,
you still have more than one week, as we are again postponing the
seminar by one week.

The seminar will be held on **Tuesday, February 10, 3pm**
(moved by one week) in Mødelokale A/B at DIKU. It features two talks
by faculty members:

- Marcos Vaz Salles: _Making Time-stepped Applications Tick in the Cloud_

- Cosmin Oancea, Jost Berthold: _On Real-World Pricing Code and its
  Parallelisation_

The first talk reports Marcos' joint work with Cornell fellows
(presented at SoCC 2011). The second talk is work in progress on
essentials of, and insights into, real-world pricing code using a
Monte-Carlo method. Abstracts are included below. We hope you will
enjoy the talks!

Best regards from HIPERFIT

## Abstracts

### Marcos Vaz Salles: _Making Time-stepped Applications Tick in the Cloud_

Scientists are currently evaluating the cloud as a new platform. Many
important scientific applications, however, perform poorly in the
cloud. These applications proceed in highly parallel discrete
time-steps or "ticks" using logical synchronization barriers at tick
boundaries. We observe that network jitter in the cloud can severely
increase the time required for communication in these applications,
significantly increasing overall running time. In this paper, we
propose a general parallel framework to process time-stepped
applications in the cloud. Our framework exposes a high-level,
data-centric programming model which represents application state as
tables and dependencies between states as queries over these
tables. We design a jitter-tolerant runtime that uses these data
dependencies to absorb latency spikes by (1) carefully scheduling
computation and (2) replicating data and computation. Our data-driven
approach is transparent to the scientist and requires little
additional code. Our experiments show that our methods improve
performance up to a factor of three for several typical time-stepped
applications.

### Cosmin Oancea, Jost Berthold: _On Real-World Pricing Code and its Parallelisation_

HIPERFIT's main mandate is to investigate language and compiler
technology to allow financial software to be (i) elegantly and readily
written and (ii) effectively optimized to exploit hardware
parallelism. In this context, we report our insights from work in
progress: evaluating a reasonably-complex kernel of a partner's
financial library, comprising about 6200 lines of low level C.

First, we experiment with parallelization solutions in the C-language
domain and show that speed-ups as high as 22x and 34x can be achieved
on a commodity GPU (Quadro2000M), for double and single precision
floats, respectively. Second, we distinguish two main sources of
optimizations: (i) classical transformations that adapt the memory
usage to the hardware parameters, and (ii) the higher-level ones that
exploit algorithmic invariants, which need to be synthesized at
interface level. Finally, to support this higher-level perspective, we
are in the process of rewriting the library in a higher-level language
(Haskell) with good support for mathematical abstraction, higher-order
functions, modularity and code reuse. Not surprisingly, the
functional approach makes the data-parallel nature of the computation
much more evident than the original C version.

We expect that the C-Haskell performance gap can be substantially
reduced by using modern libraries for data-parallelism in our -- so
far sequential -- code. Furthermore, our results indicate that the
optimizations that were identified in the C code carry over to the
Haskell domain and can even be partially automated (by means of
rewrite rules). Our work in progress on extensions and optimizations
is an important step towards a more generic codebase and
domain-specific abstractions of pricing code.