---
layout: post
title: "MSc Thesis defence on Multireduce and Multiscan on Modern GPUs"
category: news
tags: [Marco Eilers]
---
{% include JB/setup %}

MSc thesis defense by Marco Eilers.

__Time:__ Friday, 11 April 2014, 14:00-15:00.

__Place:__ Auditorium "Lille UP1", Universitetsparken 1.

#### Abstract

With the introduction of platforms like CUDA and OpenCL, the superior
computing power of modern GPUs compared to CPUs is used more and more
often to accelerate general purpose computations. The multireduce and
multiscan operations, generalizations of the ordinary reduce and scan,
have immediate applications for common algorithmic problems and show
potential to be used as simple, deterministic building blocks for
parallel algorithms.

We first discuss sequential CPU algorithms for both of these
operations, focusing especially on problems resulting from poor use of
various caches, and point out ways to solve them.  For GPUs, we
systematically examine three main groups of algorithms: parallel
adaptations of the sequential algorithm, GPU adaptations of existing
PRAM algorithms, and sort-based conversions to simpler problems. For
each of these possibilities, we discuss how the GPU memory hierarchy
can be used for best performance, and which additional algorithmic
improvements can be made for operators which are commutative as well
as associative.

We conclude that multireduce can be implemented efficiently on GPUs
and can therefore be recommended as a parallel primitive, whereas the
multiscan cannot. For histogramming, a special case of multireduce,
our algorithmic improvements for the multireduce can be used to
achieve a 40% speedup over the best existing algorithm.

__Supervisor:__ Andrzej Filinski

__External examiner:__ Peter Sestoft, ITU