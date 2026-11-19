# Category Theory

**Category theory** is a branch of mathematics that studies abstract structures and the relationships between them. Instead of focusing on individual objects (like numbers or sets), it examines how these objects connect, interact, and transform. 

In functional programming, category theory provides the mathematical foundation for core concepts like types, functions, functors, and monads.

## Core Components

Every category consists of three fundamental pieces:
**Objects:** Abstract entities representing data types (e.g., `Int`, `String`, `User`).
**Morphisms:** Arrows or transitions between objects, representing functions (e.g., `f: Int -> String`).
**Composition Rule:** A way to combine two morphisms safely. If function `f` goes from `A -> B` and function `g` goes from `B -> C`, there must exist a composite function `g ∘ f` that goes directly from `A -> C`.

## The Three Category Laws

For a collection of objects and arrows to form a valid category, they must strictly follow these algebraic rules:
**Identity:** Every object `A` must have an identity morphism (`id`) that does nothing when composed with another function (`f ∘ id = f`).
**Associativity:** When chaining three functions together, the grouping does not matter (`h ∘ (g ∘ f) = (h ∘ g) ∘ f`).
**Compositionality:** Any two sequential arrows must always be able to merge into a single valid arrow.

## Key Concepts in Programming

Category theory allows developers to model complex code architectures using universal mathematical abstractions:
**The Category of Types:** In programming, types act as the objects, and pure functions act as the morphisms.
**Functors:** A mapping between two categories that preserves structure. In code, a Functor is a data container (like a List or Optional) that implements a `map` function.
**Monads:** An extension of functors that handles sequential operations while safely managing side effects, errors, or asynchronous states (using `flatMap` or `bind`).
