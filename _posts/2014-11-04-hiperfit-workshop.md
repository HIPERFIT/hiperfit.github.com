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
<dt>09:00</dt><dd>Compilation for Parallel Computations
 <ul>
 <li><i>Futhark - an array language for data-parallel execution</i> (Troels Henriksen)</li>
 <li><i>Streaming Nested Data Parallelism</i> (Frederik Meisner Madsen)</li>
 <li><i>Compiling APL for data-parallel execution through a typed intermediate language</i> (Martin Dybdal)</li>
 </ul>
</dd>
<dt>10:15</dt><dd>Break</dd>
<dt>10:30</dt><dd>Industry Input
 <ul>
 <li><i>SimCorp on Risk</i></li>
 <li><i>"Carry that load" &mdash; Risk-minimzation in electricity markets</i> (Martin Jönsson)</li>
 </ul>
</dd>
<dt>11:45</dt><dd>Break</dd>
<dt>12:00</dt><dd>Bohrium and Big-data
 <ul>
 <li><i>Bohrium - bridging high performance and high productivity</i> (Kenneth Skovhede)</li> 
 <li><i>Title TBA</i> (Simon Lund)</li>
 <li><i>Online transaction processing for big data sources</i> (Vivek Shah)</li>
 </ul>
</dd>
<dt>13:00</dt><dd>Lunch</dd>
<dt>14:00</dt><dd>Household Finance and Risk Management
 <ul>
 <li><i>Household Finance Problems approached by Numerical Methods</i> (Mai-Britt Nordfang)</li>
 <li><i>Rethinking exchange rate risk management</i> (Rolf Poulsen)</li>
 <li><i>Calibration of the local volatility function</i> (Lykke Rasmussen)</li>
 </ul>
</dd>
<dt>15:15</dt><dd>Break</dd>
<dt>15:30</dt><dd>Financial Contracts and Valuation
 <ul>
 <li><i>Certified management of financial contracts</i> (Patrick Bahr)</li>
 <li><i>Financial benchmarks for GPGPU compilation</i> (Martin Elsman)</li>
 <li><i>A prototype framework for parallel valuation and risk calculation</i> (Martin E, perhaps)</li>
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

_Household Finance Problems approached by Numerical Methods (Maj-Britt Nordfang)_
 
Closed-form solutions to mathematical financial problems can only be
obtained when various strict assumptions are met.  As a consequence,
the problems where explicit closed-form solutions exist are usually
highly stylized.  In this talk I will present a particular problem
related to the financial decisions of individual households that
cannot be solved on closed form and discuss numerical approaches to
finding the solution.

_Calibration of the local volatility function (Lykke Rasmussen)_

In this talk we present the results of a study and comparison of 5
different methods for calibrating local volatility functions.

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
