---
title: Workshop Progamme - Functional High-Performance Computing (FHPC'13)
layout: page
---
{% include JB/setup %}

<div class="item-text dynamic-text">
 <div>

<h1>FHPC 2013 Workshop Schedule and Paper Abstracts</h1>

<style>.session {width:770px; border-top: solid black 3px;font-size:larger;clear:both;font-variant:small-caps;font-weight:bold;padding-left:20pt;padding-right:10pt;padding-top:10pt}</style>
<style>.title {font-style:italic;font-weight:bold;padding:3pt}</style>
<style>.authors {padding:3pt}</style>
<style>.abstract {font-size:smaller;width:800px;border:solid black 1px;padding:3pt}</style>
<style>.paper {width:800px;border-left:none;border-right:none;border-top: solid black 1px;padding:2pt}</style>
<!-- <style>.abstract:last-child {border-bottom: solid black 1px;padding:3pt}</style> 
<style>.paper:last-child {border-bottom: solid black 1px;padding:2pt}</style>-->

<div class="session">9:00 - 10:30 &mdash; Runtime Techniques for Declarative Parallel Programming</div>

<div class="paper"><span class="authors">Matthew Fluet.</span><br/>
<span class="title">The Manticore Project</span>(invited talk)</div>

<div class="paper"><span class="authors">Sylvain Henry. </span><br/><span class="title">ViperVM: a Runtime System for Parallel Functional High-Performance Computing on Heterogeneous Architectures</span></div>
<div class="abstract"><b>Abstract: </b>The current trend in high-performance computing is to use heterogeneous architectures (i.e. multi-core with accelerators such as GPUs or Xeon Phi) because they offer very good performance over energy consumption ratios. Programming these architectures is notoriously hard, hence their use is still somewhat restricted to parallel programming experts. The situation is improving with frameworks using high-level programming models to generate efficient computation kernels for these new accelerator architectures. However, an orthogonal issue is to efficiently manage memory and kernel scheduling especially on architectures containing multiple accelerators. Task graph based runtime systems have been a first step towards efficiently automatizing these tasks. However they introduce new challenges of their own such as task granularity adaptation that cannot be easily automatized.<br/>
In this paper, we present ViperVM, a runtime system that takes advantage of parallel functional programming to extend task graph based runtime systems and offer new optimization opportunities. The main concept is to replace dynamically created task graphs with pures functional programs. Some functions used in programs are associated to kernels (written in OpenCL, CUDA\ldots). The runtime system performs parallel reduction of these programs and it automatically schedules kernels on available accelerators. An advantage of this model is that it is easy to substitute a kernel execution with an equivalent functional expression in pure functional programs. Hence this mechanism can be used to perform granularity adaptation by replacing big tasks with equivalent expressions involving smaller ones.</div>

<div class="session">11:00 - 12:30 &mdash; Parallel Programming Models and Application Classes</div>

<div class="paper"><span class="authors"><span>Frederik M. Madsen and Andrzej Filinski</span>. </span><br/>
<span class="title">Towards a Streaming Model for Nested Data Parallelism</span></div>
<div class="abstract"><b>Abstract: </b>The language-integrated cost semantics for nested data parallelism pioneered by NESL provides an intuitive, high-level model for predicting performance and scalability of parallel algorithms with reasonable accuracy. However, this predictability, obtained through a uniform, parallelism-flattening execution strategy, comes at the price of potentially prohibitive space usage in the common case of computations with an excess of available parallelism, such as matrix multiplication.<br/>
We present a simple nested data-parallel functional language and associated cost semantics that retains NESL's intuitive work--depth model for time complexity, but also allows highly parallel computations to be expressed in a space-efficient way, in the sense that memory usage on a single (or a few) processors is of the same order as for a sequential formulation of the algorithm, and in general scales smoothly with the actually realized degree of parallelism, not the potential parallelism.<br/>
The refined semantics is based on distinguishing formally between fully materialized _vectors_ and potentially ephemeral _sequences_ of values, with the latter being bulk-processable in a streaming fashion.  This semantics is directly compatible with previously proposed piecewise execution models for nested data parallelism, but allows the expected space usage to be reasoned about directly at the source-language level.<br/>
The language definition and implementation are still very much work in progress, but we do present some preliminary examples and timings, suggesting that the streaming model has practical potential. </div>

<div class="paper"><span class="authors"><span>Qi Wang, Meixian Chen, Yu Liu and Zhenjiang Hu</span>. </span><br/>
<span class="title">Towards Systematic Parallel Programming of Graph Problems via Tree Decomposition and Tree Parallelism</span></div>
<div class="abstract"><b>Abstract: </b>Many graph optimization problems, such as the Maximum Weighted Independent Set problem, are NP-hard. For large scale graphs that have billions of edges or vertices, these problems are hard to be computed directly even using popular data-intensive frameworks like MapReduce or Pregel that are deployed on large computer-clusters, because of the extremely high computational complexity. On the other hand, many studies have shown the existence of polynomial time algorithms on graphs with bounded treewidth, which makes it possible to solve these problems on large graphs. However, the algorithms are usually difficult to be understood or parallelized.<br/>
In this paper, we propose a novel programming framework which provides a user-friendly programming interface and automatic in-black-box parallelization. The programming interface, which is a simple and straightforward abstraction called Generate-Test-Aggregate (GTA for short), is used to describe a set of graph problems. We propose to derive bottom-up dynamic programming algorithms on tree decompositions from the user-specified GTA algorithms, and further transform the bottom-up algorithms to parallel ones which run in a divide-and-conquer manner on a list of subtrees. Besides, balanced tree partition strategies are discussed for efficient parallel computing. Our preliminary experimental results on the Maximum Weighted Independent Set problem demonstrate the practical viability of our approaches.</div>

<div class="paper"><span class="authors"><span>Josef Svenningsson, Joel Svensson and Mary Sheeran</span>. </span><br/>
<span class="title">Counting and Occurrence sort for GPUs using an Embedded Language</span></div>
<div class="abstract"><b>Abstract: </b>This paper investigates two sorting algorithms: counting sort and a variation, occurrence sort,  which also removes duplicate elements,  and examines their suitability for running on the GPU. The duplicate  removing variation turns out to have a natural functional, data-parallel implementation which makes it particularly interesting for GPUs. <br/>
The algorithms are implemented in Obsidian, a high-level domain specific language for GPU programming.<br/>
Measurements show that our implementations in many cases outperform the sorting algorithm provided by the library Thrust. Furthermore, occurrence sort is another factor of two faster than ordinary counting sort. We conclude that counting sort is an important contender when considering sorting algorithms for the GPU, and that  occurrence sort is highly preferable when applicable. We also show  that Obsidian can produce very competitive code.</div>

<div class="session">13:30 - 14:30 &mdash; Optimizing Compilation of Functional Programs</div>

<div class="paper"><span class="authors"><span>Troels Henriksen and Cosmin E. Oancea</span>. </span><br/>
<span class="title">A T2 Graph-Reduction Approach To Fusion</span></div>
<div class="abstract"><b>Abstract: </b>Fusion is one of the most important code transformations as it  has the potential to substantially optimize both the memory hierarchy  time overhead and (sometimes asymptotically) the space requirement.<br/>
In imperative languages, the legality of loop-fusion is typically  verified by dependency analysis on arrays applied at loop-nest level. Such analysis, however, has often been labeled as ``heroic effort'' and, if at all, is supported only in its simplest and most conservative form in industrial compilers.<br/>
In functional languages, fusion is naturally and more easily derived as a producer-consumer relation between program constructs that expose a richer, higher-order algebra of program invariants,  such as the map-reduce list homomorphisms.<br/>
Related implementations in the functional context typically  apply fusion only when the to-be-fused producer is used exactly once, i.e., in the consumer.   This guarantees that the transformation is conservative: the resulting program does not duplicate computation.<br/>
We show that the above restriction is more conservative than needed, and present a structural-analysis algorithm, inspired from the T1-T2 transformation for reducible data flow, that enables fusion even in some cases when the producer is used  in different consumers AND without duplicating computation.<br/>
We report an implementation of the fusion algorithm for a  functional-core language, named L0, which is intended  to support nested parallelism across regular multi-dimensional arrays.   We succinctly describe L0's semantics and the compiler infrastructure  on which the fusion transformation relies, and present compiler-generated  statistics related to the success of fusion analysis on a set  of six benchmarks.</div>

<div class="paper"><span class="authors"><span>Artjoms Sinkarovs and Sven-Bodo Scholz</span>. </span><br/>
<span class="title">Sematics-Preserving Data Layout Transformations for Improved Vectorisation</span></div>
<div class="abstract"><b>Abstract: </b>Data-Layouts that are favourable from an algorithmic perspective often are less suitable for vectorisation, i.e., for an effective use of modern processor's vector instructions.<br/>
This paper presents work on a compiler driven approach towards automatically  transforming data layouts into a form that is suitable for vectorisation. In particular, we present a program transformation for a first-order functional array programming language that systematically modifies they layouts of all data structures.<br/>
At the same time, the transformation also adjusts the code that operates on these structures so that the overall computation remains unchanged. We define a correctness criterion for layout modifying program transformations and we show that our transformation abides to this criterion. </div>

<div class="session">14:30 - 15:30 &mdash; Libraries for Parallel Functional Programming</div>

<div class="paper"><span class="authors"><span>Lindsey Kuper and Ryan R. Newton</span>. </span><br/>
<span class="title">LVars: Lattice-based Data Structures for Deterministic Parallelism</span></div>
<div class="abstract"><b>Abstract: </b>Programs written using a deterministic-by-construction model of   parallel computation are guaranteed to always produce the same   observable results, offering programmers freedom from subtle,   hard-to-reproduce nondeterministic bugs that are the scourge of   parallel software.  We present a new model for   deterministic-by-construction parallel programming that generalizes   existing single-assignment models to allow multiple assignments that   are monotonically increasing with respect to a user-specified   partial order.  Our model achieves determinism by using a novel   shared data structure that allows only monotonic writes and   "threshold" reads that block until a lower bound is reached.  We   give a proof of determinism and a prototype implementation for our   model and describe how to extend it to support a limited form of   nondeterminism that admits failures but never wrong answers.</div>

<div class="paper"><span class="authors"><span>Mauro Blanco, Pablo Perdomo, Pablo Ezzatti, Alberto Pardo and Marcos Viera</span>. </span><br/>
<span class="title">Towards a functional run-time for dense NLA domain</span></div>
<div class="abstract"><b>Abstract: </b>We investigate the use of functional programming to develop a numerical linear algebra run-time; i.e. a framework where the solvers can be adapted easily  to different contexts and task parallelism can be attained (semi-) automatically. We follow a bottom up strategy, where the first step is the design and implementation  of a framework layer, composed by a functional version of BLAS routines.  Using this framework, we implement a functional version of Cholesky factorization, which serves as a proof of concept to evaluate the flexibility and performance of our approach.</div>

<div class="session">16:00 - 17:30 &mdash; Data Parallelism</div>

<div class="paper"><span class="authors">Manuel Chakravarty.</span><br/>
<span class="title">Data Parallelism in Haskell</span>(invited talk)</div>

<div class="paper"><span class="authors">Panel: </span><br/>
<span class="title">Data Parallelism and GPU Computing</span></div>

 </div>
</div>
