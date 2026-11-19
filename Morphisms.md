# Morphisms

- Morphisms are not functions or data structures in and of themselves.

Instead they're:
   - Function Shapes
   - Traversal patterns, or
   - Vectors/Directions

| Morphism | Traversal Archetype | Direction | What Each Step Observes | Array / Data Effect |
| :--- | :--- | :--- | :--- | :--- |
| :--- | :--- | :--- | :--- | :--- |
| **Catamorphism** | The Summary | Consume (Teardown) | Current element + accumulated result so far | Collapses an array into a single value (`reduce`, `sum`) |
| **Paramorphism** | The Lookahead | Consume (Teardown) | Current element + accumulator + *untouched remainder* | Reduces while inspecting the rest of the array (`tails`, scans) |
| **Histomorphism** | The Memory | Consume (Teardown) | Current element + *all previous intermediate results* | Looks back at past states (dynamic programming, stencils) |
| **Zygomorphism** | The Dual-Track | Consume (Teardown) | Current element + main accumulator + *helper accumulator* | Runs two parallel observations simultaneously (`map` + `reduce`) |
| :--- | :--- | :--- | :--- | :--- |
| **Hylomorphism** | The Pipeline | Produce → Consume | Seed state passed directly to accumulator | Generates and reduces in one pass with no intermediate array |
| :--- | :--- | :--- | :--- | :--- |
| **Anamorphism** | The Expansion | Produce (Build-up) | Current seed state | Emits one element and updates the seed (`iota`, `unfold`) |
| **Apomorphism** | The Early Exit | Produce (Build-up) | Seed state + option to emit the *entire remaining tail* | Unfolds with short-circuit termination (early exit / insert) |
| **Futumorphism** | The Multi-Step | Produce (Build-up) | Seed state + ability to emit *multiple future elements* | Generates chunks or multi-element lookaheads at once |
