# Categories of Functions

Functions are classified into different categories depending on whether they are analyzed through the lens of **computer science**, **mathematics**, or **category theory**.

## 1. Computer Science & Functional Programming
In programming, functions are grouped by how they execute, handle arguments, and interact with the external application state:

**Pure Functions:** Functions that always return the exact same output for the same input and produce zero side effects (e.g., they do not mutate state, log to consoles, or modify external variables).

**Impure Functions:** Functions whose return values can vary despite having identical inputs, or functions that trigger external changes (e.g., `Math.random()`, reading from a file, or fetching data over a network).

**First-Class & Higher-Order Functions:** Functions that can be treated like regular values. They can be stored in variables, passed into other functions as arguments, or returned from functions.

**Anonymous (Lambda) Functions:** Inline functions defined without a bound name or identifier, frequently used as short callbacks inside higher-order operations.

**Recursive Functions:** Functions that solve a larger problem by invoking themselves repeatedly within their own body until they trigger a base termination case.

## 2. Mathematics (Set Theory)
In mathematics and data typing, functions are classified by how their input set (**Domain**) maps to their target output set (**Codomain**):

**Injective (One-to-One):** Every unique input maps to a completely unique output. No two distinct inputs will ever share the same output value.

**Surjective (Onto):** Every single element in the target output set is mapped to by at least one element from the input set. There are no "unreachable" outputs.

**Bijective:** A function that is simultaneously injective and surjective. Every input pairs with exactly one unique output, and every output pairs with exactly one unique input, making the function completely invertible.

## 3. Category Theory
In category theory, functions act as **morphisms** (arrows) between types, classified by how they preserve structural information:

**Monomorphisms:** The abstract category generalization of an injective function. They represent left-cancellative arrows where distinct source structures remain distinct.

**Epimorphisms:** The abstract category generalization of a surjective function. They represent right-cancellative arrows where the target space is fully covered.

**Isomorphisms:** An invertible morphism. If an isomorphism exists between two types, it proves they have structurally identical shapes, meaning you can translate back and forth between them with zero data loss.

**Endomorphisms:** A morphism where the input object and output object are exactly identical (e.g., a function with the type signature `f :: Int -> Int`).
