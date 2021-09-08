---
layout: post
title: "Talk on Extracting Functional Programs from Coq, in Coq by Danil Annenkov"
category: news
tags: [Danil Annenkov]
---
{% include JB/setup %}

__Talk:__ Extracting functional programs from Coq, in Coq

__Presenter:__ Danil Annenkov, Aarhus University

__Time:__ Wednesday, September 15, 2021, 11:15-12:00.

__Place:__ PLTC meeting room (HCØ-01-0-029), Universitetsparken 5.

#### Abstract

Many proof assistants offer a possibility for obtaining code in a
conventional functional programming language from formalised
developments. This functionality is called code extraction. The Coq
proof assistant supports extraction to OCaml, Haskell, and Scheme out
of the box. However, the extraction functionality itself is not
verified. Moreover, there are many interesting target languages not
covered by the standard extraction. We address these challenges by
developing an extraction pipeline entirely in Coq by extending the
MetaCoq verified erasure procedure. We also develop pretty-printing
functionality to new target languages: Elm, Rust, Liquidity, and
CameLIGO. In total, this gives us a way to write dependently typed
programs in Coq, verify, and extract them to several target languages
while retaining a small trusted computing base.

In this talk, we present the current status of our development,
motivate the transformations we currently have in the pipeline, and
discuss further opportunities for extending the pipeline with new
target languages.

Joint work with Mikkel Milo, Jakob Botsch Nielsen, and Bas Spitters.
arXiv preprint:
[https://arxiv.org/abs/2108.02995](https://arxiv.org/abs/2108.02995)

#### Bio

Danil Annenkov is a postdoc researcher at the Concordium Blockchain
Research Center, Aarhus University working on formal verification of
smart contracts. His research areas include programming language
semantics, formal verification, proof assistants, and type
theory. Danil Annenkov received his PhD degree in Computer Science
from the University of Copenhagen, DIKU in 2018 under the supervision
of Martin Elsman. After receiving his PhD degree, Annenkov was a
postdoc researcher at INRIA Nantes, France, where he worked on
extending the Coq proof assistant with new reasoning principles.While
a common staple of many modern functional programming languages, sum
types are an unusual feature in specialized, computeoriented
languages.


__Host:__ Martin Elsman
