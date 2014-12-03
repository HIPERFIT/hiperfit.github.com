---
layout: post
title: "HIPERFIT Workshop"
category: news
tags: [workshop]
---
{% include JB/setup %}

<img width="200" alt="HIPERFIT logo" align="right" src="/images/hiperfit.jpg">

### HIPERFIT Workshop for partners and faculty in December

On December 10, 2014, HIPERFIT is hosting a workshop for HIPERFIT
partners and faculty. At the workshop, HIPERFIT faculty and PhD
students will present the latest developments in the various HIPERFIT
project developments. The workshop also offers [HIPERFIT partners](/partners.html) the
possibility to present opportunities for involving HIPERFIT
researchers in obstacles encountered by the partners with respect to
high-performance computational problems in the finance domain. A
separate session is therefore devoted to partners for presenting such
encounters in the finance industry.

#### The Venue

[Kurhotel Skodsborg](http://www.skodsborg.dk/), Skodsborg Strandvej 139, 2942 Skodsborg (45585800)


#### Draft schedule (December 10, 2014)

<dl class='event'>
<dt>08:30</dt><dd>Breakfast served</dd>
<dt>08:55</dt><dd>Welcome (Fritz Henglein)</dd>
<dt>09:00</dt><dd>Compilation for Parallel Computations (Chair: Ken Friis Larsen)
 <ul>
 <li><i>Futhark - an array language for data-parallel execution</i> (Troels Henriksen)</li>
 <li><i>Streaming Nested Data Parallelism</i> (Frederik Meisner Madsen)</li>
 <li><i>Compiling APL for data-parallel execution through a typed intermediate language</i> (Martin Dybdal)</li>
 </ul>
</dd>
<dt>10:15</dt><dd>Break</dd>
<dt>10:30</dt><dd>Industry Input (Chair: Fritz Henglein)
 <ul>
 <li><i>SimCorp on Risk</i></li>
 <li><i>Danske Bank (Nadeem Gulzar)</i></li>
 <li><i>"Carry that load" &mdash; Risk-minimzation in electricity markets</i> (Martin Jönsson)</li>
 </ul>
</dd>
<dt>11:45</dt><dd>Break</dd>
<dt>12:00</dt><dd>Bohrium and Big-data (Chair: Brian Vinter)
 <ul>
 <li><i>Bohrium - Bridging High Performance and High Productivity</i> (Kenneth Skovhede)</li> 
 <li><i>Effective Interoperability</i> (Simon Lund)</li>
 <li><i>Transactional Partitioning: A New Abstraction for Main-memory Databases</i> (Vivek Shah)</li>
 </ul>
</dd>
<dt>13:00</dt><dd>Lunch</dd>
<dt>14:00</dt><dd>Household Finance and Risk Management (Chair: Mogens Steffensen) 
 <ul>
 <li><i>Household Finance Problems approached by Numerical Methods</i> (Mai-Britt Nordfang)</li>
 <li><i>Rethinking Exchange Rate Risk Management</i> (Rolf Poulsen)</li>
 <li><i>Calibration of the Local Volatility Function</i> (Lykke Rasmussen)</li>
 </ul>
</dd>
<dt>15:15</dt><dd>Break</dd>
<dt>15:30</dt><dd>Financial Contracts and Valuation (Chair: Andrzej Filinski)
 <ul>
 <li><i>A Prototype Framework for Parallel Valuation and Risk Calculation</i> (Martin Elsman)</li>
 <li><i>Certified management of financial contracts</i> (Patrick Bahr)</li>
 <li><i>Financial benchmarks for GPGPU compilation</i> (Cosmin Oancea)</li>
 </ul>
</dd>
<dt>16:45</dt><dd>Thanks - feedback</dd>
<dt>17:15</dt><dd>Chat and a drink</dd>
<dt>18:30</dt><dd>Dinner</dd>
</dl>

On the day following the workshop (on December 11, 2014), HIPERFIT
staff will meet and discuss feedback and plan future activities and
projects within HIPERFIT.

A table of participants for the workshop on December 10, and for the
discussion and planning sessions on December 11, appears below.

Participation in the workshop is by invitation only, but please
[contact the HIPERFIT management](/contact.html) if you think you
should have received an invitation.

As always, please visit
[http://www.hiperfit.dk](http://www.hiperfit.dk) for news and
information about [published papers](/publications.html), our [Tuesday
lunch meetings](/lunches.html), and news in general from the HIPERFIT
research center.

#### Abstracts

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

_Compiling APL for data-parallel execution through a typed intermediate language (Martin Dybdal)_

We present a compiler for a subset of the classical array programming
language APL. The compiler translates APL programs into a typed array
intermediate language, called TAIL, which is equipped with a clear
type system and an operational semantics. We demonstrate, for a few
benchmarks, the feasibility of compiling TAIL further into code that
can execute on parallel architectures, such as GPGPUs.

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

_Calibration of the local volatility function (Lykke Rasmussen)_

In this talk we present the results of a study and comparison of 5
different methods for calibrating local volatility functions.

_A Prototype Framework for Parallel Valuation and Risk Calculation (Martin Elsman)_

We present a simple open architecture and framework for demonstrating
parallel execution of contract and portfolio valuation, as well as
risk calculations. The framework, which is open source, builds on a
contract language for specifying and managing multi-party contracts
and on an efficient parallel pricing engine.

_Certified management of financial contracts (Patrick Bahr)_

We present a contract language for describing complex financial
contracts. Contracts modelled in our language are analysed and
transformed for management according to a precise cash-flow semantics,
formalised and verified using the Coq proof assistant.


#### Participants

| Name | Dec 10 | Dinner Dec 10 | Dec 11 | Room |
| ---- |:------:|:-------------:|:------:|:----:|
Andrzej Filinski |                   1 | 1 | 1 | 1 |
Brian Vinter |                       1 | 1 | 1 | 1 |
Cosmin Oancea |                      0 | 1 | 1 | 1 |
Danil Annenkov |                     1 | 1 | 1 | 1 |
Frederik Meisner Madsen |            1 | 1 | 1 | 1 |
Fritz Henglein |                     1 | 1 | 1 | 1 |
James Avery |                        1 | 1 | 1 | 1 |
Jost Berthold |                      1 | 1 | 1 | 1 |
Ken Friis Larsen |                   1 | 0 | 1 | 0 |
Kenneth Skovhede |                   1 | 1 | 1 | 1 |
Lykke Rasmussen |                    1 | 1 | 1 | 1 |
Mads Ruben Burgdorff Kristensen |    1 | 1 | 1 | 1 |
Maj-Britt Nordfang |                 1 | 1 | 1 | 1 |
Marcos Vaz Salles |                  1 | 1 | 0 | 0 |
Martin Dybdal |                      1 | 1 | 1 | 1 |
Martin Elsman |                      1 | 1 | 1 | 1 |
Martin Jönsson |                     1 | 0 | 0 | 0 |
Mogens Steffensen |                  1 | 1 | 1 | 0 |
Patrick Bahr |                       1 | 1 | 1 | 1 |
Rolf Poulsen |                       1 | 1 | 1 | 1 |
Simon Ellersgaard |                  0 | 0 | 0 | 0 |
Simon Lund |                         1 | 1 | 1 | 1 |
Thomas Jensen |                      1 | 0 | 0 | 0 |
Troels Blum |                        0 | 0 | 0 | 0 |
Troels Henriksen |                   1 | 1 | 1 | 1 |
Vivek Shah |                         1 | 1 | 0 | 0 |
Anette Broløs (CFIR) |               1 | 1 | 0 | 0 |
Anders Pall Skött (CFIR) |           1 | 0 | 0 | 0 |
Christian Hjersing (SimCorp) |       1 | 0 | 0 | 0 |
Carl Balslev Clausen (SimCorp) |     1 | 0 | 0 | 0 |
Henrik Nygaard Jensen (Danske Bank)| 1 | 0 | 0 | 0 |
Nadeem Gulzar (Danske Bank) |        1 | 0 | 0 | 0 |
Total |                             29 | 22 | 20 | 18 |
