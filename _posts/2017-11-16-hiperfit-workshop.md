---
layout: post
title: "HIPERFIT Workshop"
category: news
tags: [workshop]
---
{% include JB/setup %}

### HIPERFIT Technical Workshop

<img alt="Workshop picture" align="right" hspace="10" width="400" src="/images/hco.jpg">

On October 16, 2017, HIPERFIT is hosting a workshop for HIPERFIT
[partners](/partners.html), [faculty](/people.html), and other people
interested in technical topics related to HIPERFIT activities. The
presentations will include presentations both by researchers external
to HIPERFIT and by HIPERFIT researchers themselves.

This event, together with the [HIPERFIT Summit held on November 17, 2017](http://hiperfit.dk/news/2017/11/17/hiperfit-summit), marks the end of the HIPERFIT research center, as we know
it. We will, continue to operate under the name of HIPERFIT, but
funding for a number of the research projects are ending, which, of
course, opens up avenues to new opportunities.

### The Venue

[DIKU, Aud 3, HCØ](http://www.diku.dk/), Universitetsparken 5, DK-2100 Copenhagen.

### Schedule November 16, 2017

<img alt="Workshop picture" align="right" hspace="10" width="400" src="/images/Salen.jpg">

<dl class='event'>
<dt>08:55</dt><dd><b>Welcome (Fritz Henglein, DIKU)</b></dd>

<dt>09:00</dt><dd><b>Partial Evaluation and Life-Insurance on GPUs</b></dd>
<dt>09:00</dt><dd><a href='#mycroft'>Object-oriented partial evaluation and the expression problem</a> <i>(Alan Mycroft, U. of Cambridge)</i></dd>
<dt>09:30</dt><dd><a href='#sestoft'>Domain-specific languages and GPGPUs in life insurance and pensions</a> <i>(Peter Sestoft, ITU)</i></dd>

<dt>10:00</dt><dd><b>Coffee Break</b></dd>

<dt>10:30</dt><dd><b>Finance</b></dd>
<dt>10:30</dt><dd><a href='#poulsen'>Special FX</a> <i>(Rolf Poulsen, MATH)</i></dd>
<dt>11:00</dt><dd><a href='#nordfang'>Household finance</a> <i>(Maj-Britt Nordfang, MATH)</i></dd>
<dt>11:30</dt><dd><a href='#benth'>Modelling stochastic volatility in forward markets</a> <i>(Fred Esben Benth, U. of Oslo)</i></dd>

<dt>12:00</dt><dd><b>Lunch</b></dd>

<dt>13:00</dt><dd><b>Streaming and Formalisation</b></dd>
<dt>13:00</dt><dd><a href='#filinski'>Streaming data-parallelism</a> <i>(Andrzej Filinski, DIKU)</i></dd>
<dt>13:30</dt><dd><a href='#biboudis'>Streaming</a> <i>(Aggelos Biboudis, École Polytechnique Fédérale de Lausanne)</i></dd>
<dt>14:00</dt><dd><a href='#annenkov'>Nominal techniques in Coq</a> <i>(Danil Annenkov, DIKU)</i></dd>

<dt>14:30</dt><dd><b>Coffee Break</b></dd>

<dt>15:00</dt><dd><b>Data-parallel Programming</b></dd>
<dt>15:00</dt><dd><a href='#henriksen'>Design and implementation of the Futhark programming language</a> <i>(Troels Henriksen, DIKU)</i></dd>
<dt>15:30</dt><dd><a href='#oancea'>TBD</a> <i>(Cosmin Oancea, DIKU)</i></dd>
<dt>16:00</dt><dd><a href='#elsman'>APL on GPUs--a progress report with a touch of machine learning</a> <i>(Martin Elsman, DIKU)</i></dd>

<dt>16:30</dt><dd><b>Mini Coffee Break</b></dd>

<dt>16:45</dt><dd><b>Blockchain Technology</b></dd>
<dt>16:45</dt><dd><a href='#ross'>Automated execution of financial contracts on blockchain</a> <i>(Omri Ross, DIKU)</i></dd>

<dt>17:15</dt><dd><b>Closing Remarks (Fritz Henglein, DIKU)</b></dd>


<dt>17:20</dt><dd><b>Chat and Snacks</b></dd>


</dl>

### Abstracts for Talks on November 16, 2017

#### 09:00-10:00 &nbsp;Partial Evaluation and Life-Insurance on GPUs

<a name='mycroft'></a>__Object-oriented partial evaluation and the expression problem__ _(Alan Mycroft, U. of Cambridge)_

Object-oriented and functional languages rest on differing foundations and the 'expression problem'
captures the idea that their inter-translation ('transpilation') is non-modular; this suggests
that automated transpilation is likely to be ad-hoc or clumsy.

We show this to be false.
By creating a partial evaluator for a pure Java-like language with a focus on class specialisation
and applying it to an interpreter for an ML-like language we show that
the seemingly idiomatic transformation from sum types to a class hierarchy arises naturally.

In common with many partial-evaluation tools, our initial translation is untyped, but we
also show how slightly richer analysis can produce a typed translation
which is close to what a human might produce.

<a name='sestoft'></a>__Domain-specific languages and GPGPUs in life insurance and pensions__ _(Peter Sestoft, ITU)_

The pension and life insurance industry works with a very long-term financial contracts where payments depend on the life state of the insured individual(s).  We present a domain-specific language called the Actulus Modelling Language for Products (AML-P) for describing the payment streams of life insurance and pension contracts, and the envisioned uses of this language, including the computation of net present value, future cashflows and so on. The latter quantities can be estimated by numerical solution of (Thiele) differential equations, and we highlight the computational flexibility obtained by using a domain-specific language to separate specification and implementations. This reflects work done in the Actulus project 2011-2016, a collaboration between Edlund A/S, Copenhagen University and the IT University of Copenhagen. We also sketch some ideas for further development.

#### 10:30-12:00 &nbsp;Finance

<a name='poulsen'></a>__Special FX__ _(Rolf Poulsen, MATH)_

TBA.

<a name='nordfang'></a>__Household finance__ _(Maj-Britt Nordfang, MATH)_

TBA.

<a name='benth'></a>__Modelling stochastic volatility in forward markets__ _(Fred Esben Benth, U. of Oslo)_

TBA.

#### 13:00-14:30 &nbsp;Streaming and Formalisation

<a name='filinski'></a>__Streaming data-parallelism__ _(Andrzej Filinski, DIKU)_

TBA.

<a name='biboudis'></a>__Streaming__ _(Aggelos Biboudis, École Polytechnique Fédérale de Lausanne)_

TBA.

<a name='annenkov'></a>__Nominal techniques in Coq__ _(Danil Annenkov, DIKU)_

TBA.

#### 15:00-16:30 &nbsp;Data-parallel Programming

<a name='henriksen'></a>__Design and implementation of the Futhark programming language__ _(Troels Henriksen, DIKU)_

Futhark is a data-parallel programming language under development at HIPERFIT. The language supports nested data-parallelism and features an optimising compiler under rabit development. This presentation gives a status update on recent Futhark development, with a particular focus on generation of efficient OpenCL GPU kernels and the steps automatically taken by the Futhark compiler to ensure fusion and efficient memory accesses. In the presentation, we will discuss various tradeoffs of the code generation, and how a new versioning technique can defer to runtime the decision between different parallelisation strategies.

<a name='oancea'></a>__TBD__ _(Cosmin Oancea, DIKU)_

TBA.

<a name='elsman'></a>__APL on GPUs--a progress report with a touch of machine learning__ _(Martin Elsman, DIKU)_

We give a status report of the APL->TAIL->Futhark compiler, which compiles a subset of APL into code executable on GPUs. The compiler handles quite a number of APL functions and operators and is, for the subset of APL it supports, highly compatible with code written for Dyalog APL. Besides reporting on the performance of a number of APL benchmarks, we demonstrate, by example, how the APL compiler tool chain can be used to teach efficiently a neural network to recognise handwritten digits.

#### 16:45-17:15 &nbsp;Blockchain Technology

<a name='ross'></a>__Automated execution of financial contracts on blockchain__ _(Omri Ross, DIKU)_

In this presentation we outline how certain financial contracts can be managed and executed automatically on the Ethereum block-chain system. The system is based on a domain-specific language for financial contracts that is capable of expressing complex multi-party derivatives and is conducive to automated execution. We propose an architecture for separating contractual terms from contract execution. A contract engine encapsulates the syntax and semantics of financial contracts without actively performing contractual actions; such actions are handled by user-definable contract managers that administer strategies for the execution of contracts. Hosting contracts and contract managers on a distributed ledger, side-by-side with digital assets, facilitates automated settlement of commitments without the need for an intermediary. We discuss how the proposed technology may change the way financial institutions, regulators, and individuals interact in a financial system based on distributed ledgers.
