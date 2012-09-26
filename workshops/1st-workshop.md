---
title: 1st HIPERFIT Workshop
layout: page
---
{% include JB/setup %}

The 1st HIPERFIT workshop takes place at DIKU, Universitetsparken 1,
Copenhagen, May 25th, 9:00-14:00, **in room 3-1-25**.

**Room changed: The workshop will be held in the small auditorium (Lille UP 1)**.

(Follow the signs from DIKU's main entrance.) 

The workshop is open to HIPERFIT partners, university faculty and
students, and the public in general. Participation is
free. Registration is required, however, due to space
limitations. (We hope not to run out of space, but may have to
limit participation if we do.)  

To register, please fill out [this form](http://diku.dk/begivenheder/2011/hiperfit_workshop/registration/) by _Monday, May 23rd, 23:59
CET_.

Students are encouraged to attend to get a first-hand impression of
the exciting mix of mathematical finance, programming language and
high performance systems problems addressed, be it because they are
looking for interesting project or thesis topics or whether they first
want to get a sense of which course prerequisites are advantageous to
ready oneself for
that.

## Agenda:

* 8:30: Arrival and Registration

* 9:00: Welcome and introduction (Fritz Henglein, DIKU)

* 9:10: Invited Talk: Logic-based modeling and analysis tools from Microsoft
Research (Nikolaj Bjørner, MSR Redmond)

* 9:45: Break

* 10:00: The HIPERFIT Research Center: Mission and Outline (Jost Berthold, DIKU)

* 10:15: Application of Functional Programming at SimCorp (Niels Hallenberg, Simcorp)

* 10:40: Mortgage refinancing and FX trading strategies - Can domain specific languages and high performance
computing help? (Kourosh Rasmussen, IMM/DTU)

* 11:05: Break

* 11:20: Data-Parallel Functional Programming (Andrzej Filinski, DIKU)

* 11:45: Parallel Contract Valuation (Michael Werk &amp; Joakim
Rønne, DIKU)

* 12:10: GPU Parallelisation of Non-Linear Pricing Problems (Jesper Andreasen, Danske Bank)

* 12:35: Generalizing Execution of Vectorizable Computations by Generating Vector Oriented Byte Code (Troels Blum, eScience Center)

* 13:00: Wrap up, followed by catered buffet lunch and networking (Fritz Henglein, DIKU)

* 14:00: End of the workshop

## Selected abstracts:

* **Nikolaj Bjørner (MSR Redmond): Logic-based modeling and analysis tools
from Microsoft Research.**

  This talk takes as starting point the symbolic
theorem prover Z3, developed in the Research in Software Engineering
group (RiSE) at Microsoft Research, Redmond. Z3 is used in several
software engineering tools, including static analysis, test-case
generation and verification tools, but also increasingly for
model-based development. I provide some details of some the tools that
are of interest for HIPERFIT.

  FORMULA (Formal Modeling Using
Logic Programming and Analysis) is a modern formal specification
language targeting model-based development. It supports concise
specifications of abstractions and model transformations using
strongly-typed constraint logic programming with algebraic
data-types. A main advantage of FORMULA is its model finding and
design space exploration facility, using logic programming and
Z3. FORMULA can be used to construct complete system models from
partial specifications and complex domain constraints. Model search
and exploration is then used to traverse the space of complete models
until it finds a globally satisfactory design. The F* language
integrates refinement types into the core of the functional
programming language F#. It uses Z3 to check type checking obligations
arising from refinement types. I demonstrate F* on a set of functional
program examples.

Nikolaj Bjørner is a Senior Researcher and head of the Foundations of
Software Engineering group at Microsoft Research Redmond.

* **Jost Berthold (DIKU): The HIPERFIT Research
Center: Mission and Outline.**

  This talk provides a quick
overview of the HIPERFIT Research Center. We present our research
vision in HIPERFIT, describe the organisation of research and projects
in the center, and outline its research areas and themes. One
particular focus of this talk is to position HIPERFIT in the landscape
of parallel functional languages.

  Jost Berthold is assistant
professor at DIKU and researcher in HIPERFIT FP. He received his
doctorate degree from the Philipps University of Marburg, Germany, in
2008. His research interests are parallel programming concepts,
parallel functional programming. In particular, he has worked
intensively on the implementation of parallel Haskell
extensions.

* **Niels Hallenberg (SimCorp): Application of Functional Programming at
SimCorp.**

  SimCorp has used functional programming for a number of years. One
example is building short time-to-market financial instruments using a
contract language developed by LexiFi
(<http://www.lexifi.com>). Another example is developing automatic
test programs using a domain specific language written in F#. In this
talk we give a few examples of this and raise challenges and problem
areas that might be interesting thesis projects.

  Niels Hallenberg is manager at
[SimCorp](http://dk.linkedin.com/company/simcorp?trk=ppro_cprof) and
External Lecturer at IT University of Copenhagen.

* **Kourosh Rasmussen (DTU): Mortgage refinancing and
FX trading strategies - Can domain-specific languages and
high-performance computing help?**

  A number of Stochastic
Programming (SP) models on mortgage choice and refinancing for Danish
households have been introduced during recent years (Nielsen &amp;
Poulsen 2004, Rasmussen and Clausen 2007, Rasmussen and Zenios
2007). Whereas most mortgage banks in Denmark today advise private
home owners to finance their property with one loan only, our models
suggest that most households are better off with two loans. With
regards to mortgage refinancing, our models suggest a higher level of
refinancing activity than what is observed today. The empirical study,
which is the main subject of this talk, is designed to perform
extensive historical ex-ante tests of the advice generated by our
model framework for the period 1995-2010. We will compare SP-based
advice with current practice which is based on rules of thumb and
short-sighted forecasts and show there is significant potential for
improvements in refinancing strategies for private home owners. The
ex-ante testing of several strategies requires huge amount of
computational work and here massive parallelization, for example on a
cloud environment, can make similar analysis possible on the desktops
of analysts and advisors. The talk is concluded with a few remarks on
the possible applications of domain-specific languages within testing
of refinancing and trading strategies. We suggest that tools combining
domain-specific languages and high-performance computing will give
financial institutions a competitive edge on product and strategy
development and assessment.

  Kourosh Rasmussen holds a
Ph.D in Operations Research. He is a partner in FinE Analytics Aps and
an associate professor at DTU.

* **Andrzej Filinski (DIKU): Data-Parallel Functional Programming.**

  Data-parallel
functional programming aims to combine the expressivity and
transparency of the applicative (functional) programming model with
the efficiency of bulk-oriented approaches to data processing on
modern, highly parallel computing platforms, such as GPGPUs. This talk
is intended to serve as an introduction to the theory and practice of
data parallelism in a functional setting, and to help dispel some
common misconceptions about the subject area.

  Andrzej
Filinski is associate professor in the Algorithms and Programming
Languages (APL) researcher group at DIKU, working primarily on applied
programming-language semantics. He heads the Functional Programming
(FP) research area of HIPERFIT.

  Andrzej Filinski is
associate professor at DIKU, heading the Functional Programming
research area in HIPERFIT. He holds a PhD in computer science from
Carnegie Mellon University.

* **Michael Werk and Joakim Rønne (DIKU): Parallel Contract Valuation (work in
progress).**

  As previously shown by Peyton Jones and Eber
(2003), the building blocks of a large class of financial
contracts can be expressed as a combinator library. This talk
summarizes this approach and then focuses on how to efficiently
price financial contracts expressed in this generic
way. The strategy chosen is to build an embedded domain specific
language for Haskell which is simultaneously expressive enough to
implement observables, models and pricers and which supports
Monte Carlo simulation on a GPGPU.

  Michael Werk and Joakim Ahnfelt-Rønne are final-year master
students&nbsp;in computer science at DIKU, with particular interests
in programming&nbsp;languages, functional programming, parallelism and
concurrency.

* **Jesper Andreasen (Danske Bank): GPU Parallelisation of Non-Linear
Pricing Problems.**

  A range of non-linear pricing problems such as Value-at-Risk and CVA
(credit value adjustment) can be solved using recursive regression
techniques similar to those previously applied to American option
pricing problems, as for example in Longstaff and Schwartz
(2001). This dramatically reduces the complexity of the calculations
and enables accurate calculations even for&nbsp;exotic
derivatives.&nbsp; Technically, it shifts the burden of the
calculation from path generation to payoff evaluation. If, in turn,
the payoff evaluation can be GPU parallelised it opens for real time
calculation of VaR and CVA and tactical risk management based on such
quantities. We discuss different strategies for such parallelisation
in the context of the Danske Markets' Jive scripting language.

Jesper Andreasen heads the Quantitative Research Department at Danske
Bank in Copenhagen. Prior to this, Jesper has held positions in the
quantitative research departments of Bank of America, Nordea, and
General Re Financial Products. Jesper's research interest include:
term structure modeling, volatility smiles, and numerical methods. In
2001 Jesper received Risk Magazine's Quant of the Year award. Jesper
holds a PhD in Mathematical Finance from Aarhus University, Denmark.

* Troels Blum (eScience Center, KU): Generalizing Execution of
Vectorizable Computations by Generating Vector Oriented Byte Code.

In my work I have used a new approach to the problem of closing the
gap between productivity tools, and highly parallel systems, which
allows a high degree of modularity and there by reuse. My approach
involves creating a model, cphVB, in which the computing devices
(hardware) are viewed as engines processing vectorized instructions,
called Vector Engines. It defines a clear and easy to understand byte
code language, which is processed by these Vector Engines.  cphVB also
contains a protocol to govern the safe, and efficient exchange,
creation, and destruction of model data.

  I have made a proof of concept implementation of the cphVB model for
NumPy, that uses CUDA devices for executing the byte code. This
implementation has proven very efficient, and cemented that the cphVB
model, with its byte code, is a viable solution to the problem of
exposing exotic hardware to languages, and other front-ends, that
scientists, and other programmers use every day.

  Troels Blum is working in the research group of Brian Vinter, who is
head of the High Performance Systems research area in HIPERFIT. He
works on the HPHP (High Performance - High Productivity) project at
the eScience center. His primary focus since obtaining his M.S. degree
is GPGPU programming.