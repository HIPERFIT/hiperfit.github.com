---
layout: post
title: "HIPERFIT Seminar on July 2, 2013"
category: news
tags: [fusion, seminar, Bohrium, Brian Vinter, Troels Henriksen]
---
{% include JB/setup %}

The HIPERFIT July 2013 seminar is planned for Tuesday, July 2 from
14:00 to 15:30 at the DIKU small auditorium (Lille Aud), where we will
have two presentations by [Troels Henriksen](/people.html) and [Brian Vinter](/people.html):

- __14:00-14:30. A T2 Graph-Reduction Approach To Fusion. (Troels Henriksen, HIPERFIT, DIKU).__

- __14:30-15:00. Topic to be announced. (Brian Vinter, HIPERFIT, NBI).__

- __15:00-15:30. A light refreshment, served by HIPERFIT.__

Abstracts for the talks follow below.

We look forward to see you at the seminar!

Best Regards,

Martin Elsman

HIPERFIT Center Manager

---

__A T2 Graph-Reduction Approach To Fusion__

Troels Henriksen, HIPERFIT, DIKU

14:00-14:30 July 2, 2013

The (DIKU) small auditorium at Universitetsparken 1 (UP1)

Fusion is one of the most important code transformations as it has the
potential to substantially optimize both the memory hierarchy time
overhead and (sometimes asymptotically) the space requirement. In
imperative languages, the legality of loop-fusion is typically
verified by dependency analysis on arrays applied at loop-nest
level. Such analysis, however, has often been labeled as "heroic
effort" and, if at all, is supported only in its simplest and most
conservative form in industrial compilers.  In functional languages,
fusion is naturally and more easily derived as a producer-consumer
relation between program constructs that expose a richer, higher-order
algebra of program invariants, such as the map-reduce list
homomorphisms.  Related implementations in the functional context
typically apply fusion only when the to-be-fused producer is used
exactly once, i.e., in the consumer. This guarantees that the
transformation is conservative: the resulting program does not
duplicate computation.  We show that the above restriction is more
conservative than needed, and present a structural-analysis algorithm,
inspired from the T1 -T2 transformation for reducible data flow, that
enables fusion even in some cases when the producer is used in
different consumers and without duplicating computation.  We report an
implementation of the fusion algorithm for a functional-core language,
named L0 , which is intended to support nested parallelism across
regular multi-dimensional arrays. We succinctly describe L0's
semantics and the compiler infrastructure on which the fusion
transformation relies.

*Troels Henriksen* is an MSc student at DIKU, employed in the HIPERFIT
 research center, and working on the implementation and design of the
 HIPERFIT parallel-functional programming language L.

