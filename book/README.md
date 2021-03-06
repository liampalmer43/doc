# The Flix Programming Language

Welcome to the official website for the documentation of the [Flix](https://github.com/flix) programming language.

***NB: Flix is still under major development and the language is expected to change.***

Flix is a [functional](https://en.wikipedia.org/wiki/Functional_programming) and 
[logic](https://en.wikipedia.org/wiki/Logic_programming) programming language for 
[fixpoint](https://en.wikipedia.org/wiki/Fixed_point_mathematics) computations on 
[lattices](https://en.wikipedia.org/wiki/Lattice_order).

Flix is heavily inspired by the [Datalog](https://en.wikipedia.org/wiki/Datalog) language,
but extends its expressive power by adding support for user-defined lattices and operations on them.
The primary use case of Flix is for development and implementation of scalable 
[static analysis](https://en.wikipedia.org/wiki/Static_analysis) tools,
especially [points-to analysis](https://en.wikipedia.org/wiki/Pointer_analysis) and 
[dataflow analysis](https://en.wikipedia.org/wiki/Data-flow_analysis).

As a special case, Flix can be used as a general-purpose Datalog solver with the benefits of
a type system plus an integrated profiler and debugger.

Unlike [general-purpose](https://en.wikipedia.org/wiki/General-purpose_programming_language) languages such as
C++ and Java, Flix is a special-purpose ([domain-specific](https://en.wikipedia.org/wiki/Domain-specific_language))
programming language. Flix is intended for (recursive) constraints on relations and lattices. In other words,
you cannot write a web server or a video game in Flix.

A Flix program is a set of facts and a set of constraints (rules) for deriving new facts. 
The computation of a Flix programs determines all possible facts that can be derived from the initial facts
and the constraints.