---
title: Research Themes
layout: page
---
{% include JB/setup %}

HIPERFIT comprises a number of research themes relevant to computing
in finance, and execution on high-performance backends. The following
ones have been identified to guide and connect together our activities
in the center.

## Risk Scenarios

We try to describe the transition from observables (like current
prices and historical data) to scenario generation and from scenario
generation to reporting and management. In order to, for example, pick
a quantile scenario on the basis of high-dimensional data, one has to
address modeling aspects, correlation and other dependency aspects,
and extreme value aspects. Risk scenarios play a main role in solvency
issues for generation of different types of capital
requirements. These requirements are fed back into management
processes and lead to decision making. Within this theme we address
the mutuality in the risk scenario generation and decision making
processes. The topic calls upon advances in data structures and
numerical methods for so-called differential games.

Capital requirements based on risk scenarios are applied in valuation,
for instance in the so-called cost of capital method. Within this
theme we are interested in the relation between arbitrage free
valuation and cost of capital valuation generated in a given solvency
regime.

## Model Specification

How much detail is necessary and how much is sufficient in a financial
model?  Going from one extreme, namely model-free relative valuation
(some prices are given completely in terms of other prices) towards
another extreme, namely advanced multi-dimensional jump-diffusions
processes with a high-dimensional parameter set, what are the benefits
and costs for the given application in mind, be it solvency issues,
accounting issues, or management issues? A main part of this is, in
the first place, to study these advanced models in details and clarify
their strengths and weaknesses, also in relation to their
optimisation-precision trade-off on high-performance systems.

## DSLs for Financial Information

Declarative domain-specific languages (DSLs), operating at a high
level of (programming) abstraction, are already widely-used in the
financial sector to describe a range of financial products
(derivatives). We want to design similarly expressive and
automatically optimizable declarative specification languages for
other financial information, and especially for financial models (see
above). 

Our goal is a DSL framework with broad application coverage, that
enables fast implementation, easy maintenance, extensibility and
reusability across financial institutions, in short: low total cost of
ownership (TCO). Financial information applications should cover
computing applications such as reporting to auditors and public
authorities, data communication with clearing houses, internal
reporting and statistics, computations for the purpose of internal
risk management, and flexible integration for standard routines such
as accounting and confirmation processing.

## Extracting Parallelism from Declarative Specifications

The core theme of this theme is the rendition of large-scale financial
computations into a form that exposes inherent parallelism. To this
end, we aim to develop a language that can be productively used to
express large-scale numeric computations in a natural style, close to
familiar mathematical notation, and yet is, at the same time,
efficiently executable on a variety of modern parallel
platforms.

The paradigm of data-parallelism (by G.Blelloch) appears to be a good
match for the HIPERFIT application domain: it enables concise and
long-term maintainable specifications of a wide variety of inherently
parallelizable computations, without committing to any particular
implementation strategy or execution environment. We will design a
suitable such language, with a compositional formal semantics and cost
model, to enable correctness proofs and performance estimates.

The DSL development for financial models will lead to additional or
modified requirements at a later stage of the project. Typical
operations for valuation of stochastic financial models need to be
translated into the provided parallel operations. Necessary and useful
abstractions and patterns of parallelism will be identified from
working on concrete projects.

## High-Performance Backends for Novel Hardware

These are activities to ensure that the models, in their executable
form, can execute on next-generation processors. The research will
focus on mapping the parallelism that is expressed by the functional
programming activities onto a number of parallel computer
architectures. The systems activities will work in close collaboration
with other projects that seek to exploit next-generation processors.

In a first stage, we will investigate a number of current algorithms
from computational finance IT for execution on next-generation
processors. Based on these experiences, a preliminary backend for
next-generation-processors will be integrated with the existing
solutions from partners; before integrating the full backend with the
engine for functional programming from the project itself.