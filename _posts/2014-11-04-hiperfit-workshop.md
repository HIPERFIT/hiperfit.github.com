---
layout: post
title: "HIPERFIT Workshop"
category: news
tags: [workshop]
---
{% include JB/setup %}

<img width="200" alt="HIPERFIT logo" align="right" src="/images/hiperfit.jpg">

### 2014 HIPERFIT Workshop for Partners and Faculty

On December 10, 2014, HIPERFIT is hosting a workshop for HIPERFIT
partners and faculty. At the workshop, HIPERFIT faculty and PhD
students will present the latest developments in the various HIPERFIT
project developments. The workshop also offers [HIPERFIT partners](/partners.html) the
possibility to present opportunities for involving HIPERFIT
researchers in obstacles encountered by the partners with respect to
high-performance computational problems in the finance domain. A
separate session is therefore devoted to partners for presenting such
encounters in the finance industry.

### The Venue

[Kurhotel Skodsborg](http://www.skodsborg.dk/), Skodsborg Strandvej 139, 2942 Skodsborg (45585800)

### Schedule December 10, 2014

<dl class='event'>
<dt>08:30</dt><dd>Breakfast served</dd>
<dt>08:55</dt><dd>Welcome (Fritz Henglein)</dd>
<dt>09:00</dt><dd>Compiling for Parallel Computations (Chair: Ken Friis Larsen)
 <ul>
 <li><i><a href="/pdf/HIPERFIT_Dec2014_Henriksen.pdf">Futhark - An Array Language for Data-parallel Execution</a></i> (Troels Henriksen, DIKU)</li>
 <li><i><a href="/pdf/HIPERFIT_Dec2014_Madsen.pdf">Streaming Nested Data Parallelism</a></i> (Frederik Meisner Madsen, DIKU)</li>
 <li><i>Compiling APL for Data-Parallel Execution through a Typed Intermediate Language</i> (Martin Dybdal, DIKU)</li>
 </ul>
</dd>
<dt>10:15</dt><dd>Break</dd>
<dt>10:30</dt><dd>Industry Input (Chair: Fritz Henglein)
 <ul>
 <li><i><a href="/pdf/HIPERFIT_Dec2014_Clausen.pdf">The MC2 Challenge in Risk</a></i> (Carl Balslev Clausen, SimCorp)</li>
 <li><i>Big Data and Advanced Analytics in a Financial Institution</i> (Nadeem Gulzar, Danske Bank) <b><i>CANCELLED</i></b></li>
 <li><i>"Carry that Load" &mdash; Risk-minimization in Electricity Markets</i> (Martin Jönsson, IMF)</li>
 </ul>
</dd>
<dt>11:30</dt><dd>Break</dd>
<dt>11:45</dt><dd>Bohrium and Big-data (Chair: Brian Vinter)
 <ul>
 <li><i><a href="/pdf/HIPERFIT_Dec2014_Skovhede.pdf">Bohrium - Bridging High Performance and High Productivity</a></i> (Kenneth Skovhede, NBI)</li> 
 <li><i>Effective Interoperability</i> (Simon Lund, NBI)</li>
 <li><i>Transactional Partitioning: A New Abstraction for Main-memory Databases</i> (Vivek Shah, DIKU)</li>
 </ul>
</dd>
<dt>13:00</dt><dd>Lunch</dd>
<dt>14:00</dt><dd>Household Finance and Risk Management (Chair: Mogens Steffensen) 
 <ul>
 <li><i><a href="/pdf/HIPERFIT_Dec2014_Nordfang.pdf">Household Finance Problems approached by Numerical Methods</a></i> (Mai-Britt Nordfang, IMF)</li>
 <li><i><a href="/pdf/HIPERFIT_Dec2014_Poulsen.pdf">Rethinking Exchange Rate Risk Management</a></i> (Rolf Poulsen, IMF)</li>
 <li><i>Calibration of the Local Volatility Function</i> (Lykke Rasmussen, IMF) <b><i>CANCELLED</i></b></li>
 </ul>
</dd>
<dt>15:15</dt><dd>Break</dd>
<dt>15:30</dt><dd>Financial Contracts and Valuation (Chair: Andrzej Filinski)
 <ul>
 <li><i><a href="/pdf/HIPERFIT_Dec2014_Elsman.pdf">A Prototype Framework for Parallel Valuation and Risk Calculation</a></i> (Martin Elsman, DIKU)</li>
 <li><i>Certified Management of Financial Contracts</i> (Patrick Bahr, DIKU)</li>
 <li><i>Financial Benchmarks for GPGPU Compilation</i> (Cosmin Oancea, DIKU)</li>
 </ul>
</dd>
<dt>16:45</dt><dd>Thanks - feedback</dd>
<dt>17:15</dt><dd>Chat and a drink</dd>
<dt>18:30</dt><dd>Dinner</dd>
</dl>

A table of participants for the workshop on December 10, and for the
discussion and planning sessions (HIPERFIT staff only) on December 11,
appears below. The schedule for December 11 appears at the very end of
the page.

Participation in the workshop is by invitation only, but please
[contact the HIPERFIT management](/contact.html) if you think you
should have received an invitation.

As always, please visit
[http://www.hiperfit.dk](http://www.hiperfit.dk) for news and
information about [published papers](/publications.html), our [Tuesday
lunch meetings](/lunches.html), and news in general from the HIPERFIT
research center.

### Abstracts

#### 09:00-10:15 &nbsp; Compiling for Parallel Computations

_Futhark - An Array Language for Data-parallel Execution (Troels Henriksen)_

Compiling real-world applications to efficient parallel code,
especially when targeting many-core hardware, requires an optimiser
and code generator that can exploit a combination of high-level
invariants and low-level optimisations.  We present a purely
functional core language, named Futhark, intended as a compilation
target for higher-level languages, that supports nested map-reduce
parallelism on regular array, but also a set of "imperative"
constructs, such as in-place updates and do-loops.  We also report
in-progress work on the Futhark optimizing compiler, which is thought
to allow a gradual transformation of the program, within the same
representation, towards low-level, imperative-like code, which can
then be efficiently and straightforwardly translated to the parallel
assembly languages of our time, such as CUDA and OpenMP.

_Streaming Nested Data Parallelism (Frederik Meisner Madsen)_

A clever compiler relieves the programmer from many technical details,
facilitating rapid development, code re-use and hopefully high
performance. If the compiler obeys a simple optimistic time-space cost
model, the hope becomes a guarantee. This talk aims to identify two
key challenges related to functional data-parallel language design and
costing: Nested data-parallelism and excessive space usage when too
few processors are available. To solve these challenges, a language
based on first-class sequences and dataflow execution is
presented. The language supports nested data parallelism, obeys a
time-space cost model and can run on many different architectures
including single-core machines and GPGPUs. Experiments show promising
results compared to similar languages, and the ideas are currently
being implemented in the next release of Accelerate, a Haskell library
for data-parallel execution on GPGPUs.

_Compiling APL for Data-parallel Execution through a Typed Intermediate Language (Martin Dybdal)_

We present a compiler for a subset of the classical array programming
language APL. The compiler translates APL programs into a typed array
intermediate language, called TAIL, which is equipped with a clear
type system and an operational semantics. We demonstrate, for a few
benchmarks, the feasibility of compiling TAIL further into code that
can execute on parallel architectures, such as GPGPUs.

#### 10:30-11:30 &nbsp; Industry Input

_The MC2 Challenge in Risk (Carl Balslev Clausen, SimCorp)_
 
Monte Carlo methods are required for precise valuation of contracts
that have a certain level of complexity. Monte Carlo methods are also
required for various Risk calculations when large shocks and movements
are modelled. Combining Monte Carlo Risk with Monte Carlo valuation we
encounter the double Monte Carlo challenge, aka the MC2 challenge. We
report on specific use cases and benchmarks from the industry.

_Big Data and Advanced Analytics in a Financial Institution (Nadeem Gulzar, Danske Bank)_ **_CANCELLED_**

In Danske Bank a lot of effort is being put into utilizing new sources
of data (social, weblogs, etc.) to gain a better understanding of the
customers and their behavior. To handle and process the extremely
large amount of data, we require an equally large amount of processing
power. There are many ways to address this ranging from using lots of
cash to optimizing techniques, etc.

_"Carry that Load" &mdash; Risk-minimization in Electricity Markets (Martin Jönsson, IMF)_

In this talk we look at a specific hedging problem of a contract in
the derivatives market for power contracts. We suggest a simple
hedging approach that relies on expected loss minimisation of our
hedged position, and to calculate our optimal hedge we suggest a
simple model for the spot price and consumption of electricity. We
test our approach on empirical data obtained from an energy trading
company, and compare our strategy to the hedging approach currently
used by the company.

#### 11:45-13:00 &nbsp; Bohrium and Big-data

_Bohrium - Bridging High Performance and High Productivity (Kenneth Skovhede)_

In this talk I introduce the Bohrium runtime system and show how it
simultaneously enables rapid development and high performance
execution. I then summarize our current results with the Bohrium
approach for CPU, GPGPU and cluster execution. Finally I present the
state of my current work on FPGA execution in Bohrium.

_Effective Interoperability (Simon Lund)_

Programming languages and models are essential building blocks for
computer-based problem-solving. The general challenge is about
modeling concepts and abstractions for a given problem and expressing
it programmatically to obtain a solution. A challenge that no single
programming model or language can solve for the general case when put
under the constraint of also efficiently utilizing hardware.  However,
many languages and models exist which solves classes of problems
efficiently. Interoperability provides the means of combining them. In
this talk, this approach is exemplified through the use of the
emerging parallel programming language Chapel and the long-lived
productivity language Python. The interoperability approach is
exemplified by introducing Chapel and comparing strengths/weaknesses
of the two languages and how to overcome them through the use of
interoperability.  

_Transactional Partitioning: A New Abstraction for Main-memory Databases (Vivek Shah)_

Online Transaction Processing (OLTP) applications are making new
demands from OLTP databases on variety, performance and application
cost frontiers.  Existing programming models provided by current
OLTP databases do not meet all the demands of these classes of
applications.  The talk presents a new programming model
(transactional partitioning) that needs to be targetted by OLTP
databases (especially main-memory databases) that would allow
them to meet these new application demands. The talk also
outlines the challenges and their possible solutions that are
being investigated while building the prototype system.

#### 14:00-15:15 &nbsp; Household Finance and Risk Management

_Household Finance Problems approached by Numerical Methods (Maj-Britt Nordfang)_
 
Closed-form solutions to mathematical financial problems can only be
obtained when various strict assumptions are met.  As a consequence,
the problems where explicit closed-form solutions exist are usually
highly stylized.  In this talk I will present a particular problem
related to the financial decisions of individual households that
cannot be solved on closed form and discuss numerical approaches to
finding the solution.

_Rethinking Exchange Rate Risk Management (Rolf Poulsen)_

We describe some theoretical and practical (from computational to
legal) issues in the construction of an exchange-rate risk management
system that is feasible for small to medium enterprises. This work is
a collaboration with http://www.gcureports.com/ and you will hear how
the system was almost endorsed by the Pope.

_Calibration of the local volatility function (Lykke Rasmussen)_ _**CANCELLED**_

In this talk we present the results of a study and comparison of 5
different methods for calibrating local volatility functions.

#### 15:30-16:45 &nbsp; Financial Contracts and Valuation

_A Prototype Framework for Parallel Valuation and Risk Calculation (Martin Elsman)_

We give an overview of a simple open architecture and framework for
demonstrating parallel execution of contract and portfolio valuation,
as well as risk calculations. The framework, which is open source,
builds on a contract language for specifying and managing multi-party
contracts and on an efficient parallel pricing engine.

_Certified Management of Financial Contracts (Patrick Bahr)_

We present a contract language for describing complex financial
contracts. Contracts modelled in our language are analysed and
transformed for management according to a precise cash-flow semantics,
formalised and verified using the Coq proof assistant.

_Financial Benchmarks for GPGPU Compilation (Cosmin Oancea)_

We present three studies of array-based applications from the
financial domain, all suitable for GPGPU execution. The studies have
resulted in three concrete application benchmarks for which the
available parallelism is described by nested map-reduce functional
combinators. We also describe the influence of the invariants and code
transformations that govern the main trade-offs of the rich,
dataset-sensitive optimisation space. The application benchmarks
targets both CPUs and GPGPUs and we provide useful insight into the
language constructs and compiler infrastructure capable of expressing
and optimising such applications.

### Participants

| Name | Dec 10 | Dinner Dec 10 | Dec 11 | Room |
| ---- |:------:|:-------------:|:------:|:----:|
Andrzej Filinski (DIKU) |            1 | 1 | 1 | 1 |
Brian Vinter (NBI) |                 1 | 1 | 1 | 1 |
Cosmin Oancea (DIKU) |               0 | 1 | 1 | 1 |
Danil Annenkov (DIKU) |              1 | 1 | 1 | 1 |
Frederik Meisner Madsen (DIKU) |     1 | 1 | 1 | 1 |
Fritz Henglein (DIKU) |              1 | 1 | 1 | 1 |
James Avery (NBI) |                  1 | 1 | 1 | 1 |
Jost Berthold (DIKU) |               1 | 1 | 1 | 1 |
Ken Friis Larsen (DIKU) |            1 | 0 | 1 | 0 |
Kenneth Skovhede (NBI) |             1 | 1 | 1 | 1 |
Lykke Rasmussen (IMF) |              0 | 0 | 0 | 0 |
Mads R. B. Kristensen (NBI) |        1 | 1 | 1 | 1 |
Maj-Britt Nordfang (IMF) |           1 | 1 | 1 | 1 |
Marcos Vaz Salles (DIKU) |           1 | 1 | 0 | 0 |
Martin Dybdal (DIKU) |               1 | 1 | 1 | 1 |
Martin Elsman (DIKU) |               1 | 1 | 1 | 1 |
Martin Jönsson (IMF) |               1 | 1 | 0 | 0 |
Mogens Steffensen (IMF) |            1 | 1 | 1 | 0 |
Oleksandr Shturmov (DIKU) |          1 | 1 | 1 | 0 |
Patrick Bahr (DIKU) |                1 | 1 | 1 | 1 |
Rolf Poulsen (IMF) |                 1 | 1 | 1 | 1 |
Simon Ellersgaard (IMF) |            0 | 0 | 0 | 0 |
Simon Lund (NBI) |                   1 | 1 | 1 | 1 |
Thomas Jensen (DIKU) |               1 | 0 | 0 | 0 |
Troels Blum (NBI) |                  0 | 0 | 0 | 0 |
Troels Henriksen (DIKU) |            1 | 1 | 1 | 1 |
Vivek Shah (DIKU) |                  1 | 1 | 0 | 0 |
Anette Broløs (CFIR) |               1 | 1 | 0 | 0 |
Anders Pall Skött (CFIR) |           1 | 0 | 0 | 0 |
Christian Hjersing (SimCorp) |       1 | 0 | 0 | 0 |
Jens Ehlers (SimCorp) |              1 | 1 | 0 | 0 |
Carl Balslev Clausen (SimCorp) |     1 | 1 | 0 | 0 |
Henrik Nygaard Jensen (Danske Bank)| 1 | 1 | 0 | 0 |
Nadeem Gulzar (Danske Bank) **ILL** |0 | 0 | 0 | 0 |
Uwe Heissner (Nordea) |              1 | 0 | 0 | 0 |
Manuel Torrealba (Nordea) |          1 | 0 | 0 | 0 |
Total |                             31 | 26 | 20 | 17 |

### Schedule December 11, 2014 (HIPERFIT staff only) 

On December 11, 2014, HIPERFIT staff will meet and discuss feedback
and plan future activities and projects within HIPERFIT. Here is a
draft schedule.

<dl class='event'>
<dt>08:30</dt><dd>Breakfast served</dd>
<dt>08:55</dt><dd>Outline for the day (Plenum)</dd>
<dt>09:00</dt><dd>Session 1 (Groups)</dd>
<dt>12:00</dt><dd>Lunch</dd>
<dt>13:00</dt><dd>Session 2 (Groups)</dd>
<dt>15:00</dt><dd>Break</dd>
<dt>15:15</dt><dd>Group Presentations (Plenum)</dd>
<dt>16:30</dt><dd>End</dd>
</dl>
