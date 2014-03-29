---
title: Student Project - Structural Description Language
layout: page
group: studentprojects
---
{% include JB/setup %}

As part of its research into parallel functional programming, HIPERFIT
has developed a programming language, L0, and an optimising compiler.
This project is about designing and implementing a schema-like
description language for recursive syntax trees, then use it to write
tests that specify the desired high-level structure of the optimised
program.

### Contact person

[Cosmin Oancea](people.html) (or [Troels Henriksen](people.html)).

### Notes

Compiling code in a high-level language for efficient execution on
modern hardware requires an optimising compiler, that supports powerful
structural transformations, such as hoisting, loop interchange and
fusion.  Unfortunately, these optimisations are usually complex and
difficult to implement, and as a result, changes in one part of the
compiler may result in an optimisation in another part to become
nonfunctional.

While the L0 compiler has a comprehensive test suite, it is only able to
check whether the resulting programs are still correct, and compute the
right results.  Specifically, the test suite cannot detect whether the
resulting program is not optimised as well as intended.

We could solve this by annotating every test program with a high-level
description of the desired structure after optimisation.  The
description should be insensitive to small pertubations, such as
variable names or statement ordering, and be relatively concise.  This
could be done by only specifying loop nesting and dependencies between
control-flow structures.

The RELAX NG and HTML DTD schema languages from the web world can
serve as inspiration, although we would prefer a much more concise
notation, perhaps similar to regular expressions.

As L0 is an experimental language, its precise syntax tree is likely to
change in the future.  Ideally, the description language should be
relatively easy to extend.  The particularly motivated student may want
to make the description language "generic", in the sense that it can be
fitted onto any tree structure with a small bit of glue code.

The L0 compiler is implemented in Haskell, and it would thus be
desirable if the description language was likewise, although this is not
a strict requirement.

### Key topics

Functional programming, Haskell, Formal languages

### Input

A description of L0 is available in the paper ["A T2 Graph-Reduction
Approach To Fusion"](pdf/fhpc13_troels.pdf).

The [L0 compiler is available on
Github](https://github.com/HIPERFIT/L0Language).


### Prerequisites

Capable of writing small and middle sized applications in Haskell.
Understanding of basic compiler technology (equivalent to taking DIKUs
compiler course and enjoying it).
