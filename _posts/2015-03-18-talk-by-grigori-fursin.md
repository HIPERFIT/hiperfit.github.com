---
layout: post
title: "Talk by Grigori Fursin on Collaborative and Reproducible Computer Engineering"
category: news
tags: [visit, talk, Grigori Fursin]
---
{% include JB/setup %}

__Collective Knowledge Project: Towards Collaborative and Reproducible Computer Engineering__

Grigori Fursin, CTO, cTuning foundation.

Time and location: March 19, 15:30-16:30. The APL meeting room, DIKU, Universitetsparken 5, Building B, 2100 Copenhagen Ø.

To attend the talk, please signup by email to Martin Elsman (mael at di.ku.dk).

__Abstract:__

Designing novel computer systems and optimizing their software 
is becoming too tedious, ad-hoc, time consuming and error prone 
due to an enormous number of available design and optimization choices.
Empirical auto-tuning combined with run-time adaptation and
machine learning has been demonstrating some potential to address
the above challenges for several decades but is still far from
widespread production. Main reasons include unbearably long
exploration and training times, ever changing tools and their
interfaces, lack of a common experimental methodology, and lack
of unified mechanisms for knowledge building and exchange apart
from publications where reproducibility of results is often not
even considered.

In this talk, I will present our community-driven approach and the
4th version of our public infrastructure and repository
to preserve, systematize and share knowledge and experience about
program optimization. Our framework helps to describe and
preserve the whole  experimental setup with all related
artifacts (benchmarks, kernels, data sets, libraries, tools) in
a reproducible way to automate and crowdsource optimization space
exploration and learning. Any unexpected behavior is recorded and
analyzed using shared data mining and predictive modeling plugins
or is exposed to the community for collaborative explanation.
Collected knowledge can be used to validate past research
techniques or can be extrapolated to predict better
optimizations, run-time adaptation scenarios and hardware
designs. During the past 5 years, this approach has been extensively
validated with our industrial partners, and helped initiate a new
publication model where experiments and artifacts are validated
and improved by the community. A beta version of the new framework
is available at [http://github.com/ctuning/ck](http://github.com/ctuning/ck).

__Bio:__

Grigori Fursin is a founder and CTO of the cTuning foundation.
In the past, he was a tenured research scientist at INRIA Saclay
and was co-founder of the Intel Exascale Lab in France. Grigori has an
interdisciplinary background in computer engineering, physics,
electronics, machine learning and mathematics. He obtained a PhD in
Computer Science from the University of Edinburgh in 2004.

Grigori pioneered machine-learning based program auto-tuning
and hardware co-design combined with crowdsourcing and run-time adaptation.
In 2008, he established a public repository of optimizations knowledge
(cTuning.org) to initiate collaborative and reproducible R&D in computer
engineering. Since then, his techniques and tools have been used and 
extended in multiple industrial projects together with ARM, IBM, Intel, 
Synopsys and ST. In 2012, Grigori received an INRIA award and 4-year
fellowship for "making an outstanding contribution to research".
He is leading an Artifact Evaluation initiative for CGO and PPoPP
while developing an open research SDK to preserve, structure 
and reuse knowledge about program and architecture optimization:
[http://github.com/ctuning/ck](http://github.com/ctuning/ck).