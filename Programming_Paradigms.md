### Event-Oriented (Event-Driven Programming)
* **Core Focus:** Reacting to signals, messages, or user actions rather than following a fixed top-to-bottom script.
* **How it Works:** The program sits in a loop listening for events (mouse clicks, network requests, sensor triggers) and dispatches them to specific handler functions.
* **Best For:** User interfaces (UI), web servers (like Node.js), and asynchronous microservices.

### Component-Oriented (Entity-Component-System / ECS)
* **Core Focus:** Composition over inheritance.
* **How it Works:** Instead of deep class hierarchies (OOP), entities are just IDs that attach modular "components" (pure data) which are processed by "systems" (pure logic). ECS is essentially the architectural bridge between OOP and Data-Oriented Design.
* **Best For:** Video games (e.g., Unity DOTS, Bevy) and complex simulations.

### Aspect-Oriented Programming (AOP)
* **Core Focus:** Separating "cross-cutting concerns" from core business logic.
* **How it Works:** Behaviors that span across many unrelated modules—like logging, security authentication, or caching—are isolated into "aspects" and injected into the code at runtime or compile-time without cluttering the main functions.
* **Best For:** Enterprise backends (e.g., Java Spring) where boilerplate monitoring or permissions are needed everywhere.

### Service-Oriented (SOA & Microservices)
* **Core Focus:** Organizing an entire system into independent, networked business capabilities.
* **How it Works:** Instead of organizing functions inside one codebase, distinct "services" (e.g., Billing, Authentication, Inventory) communicate over a network via APIs.
* **Best For:** Large-scale cloud applications where different teams deploy code independently.

### Declarative / Logic-Oriented (Constraint & Logic Programming)
* **Core Focus:** Describing *what* the desired outcome is, rather than *how* to compute it step-by-step.
* **How it Works:** You define a set of facts, rules, or constraints, and an underlying engine figures out the execution path to satisfy them.
* **Best For:** Database queries (SQL), configuration management (Terraform), and rule-based AI/scheduling (Prolog).
### Functional Programming (Core Behavioral Model of DOP)
* **Core Focus:** Evaluating mathematical functions while avoiding mutable data and changing state.
* **How it Works:** Pure functions take immutable data as input and return new transformed copies without causing side effects, serving as the behavioral foundation for Data-Oriented Programming (DOP).
* **Best For:** Concurrent systems, data transformation pipelines, and predictable web/backend applications (e.g., Clojure, Elixir, TypeScript).

### Procedural Programming (Aligned with DOD)
* **Core Focus:** Separating raw data structures from the step-by-step procedures or subroutines that operate on them.
* **How it Works:** Functions execute sequentially and often mutate data in place, closely aligning with Data-Oriented Design's (DOD) separation of flat structs and processing loops (contrasting with OOP).
* **Best For:** High-performance systems programming, game engines, and hardware-level optimization (e.g., C, Rust, Zig).

### Object-Oriented Programming (OOP)
* **Core Focus:** Bundling state (data) and behavior (methods) together into self-contained "objects."
* **How it Works:** Objects encapsulate internal state and communicate via methods, relying on class hierarchies, inheritance, and polymorphism to model real-world or domain entities.
* **Best For:** Complex business domains, enterprise applications, and large codebases requiring clear encapsulation boundaries (e.g., Java, C#, Python).

### Data-Oriented (DOP & DOD)
* **Core Focus:** Treating data as a first-class citizen, completely decoupled from behavior and business logic.
* **How it Works:** Splits into **Data-Oriented Programming (DOP)**, which uses generic, immutable data structures transformed by pure functions, and **Data-Oriented Design (DOD)**, which organizes flat data layouts in memory for optimal CPU cache efficiency.
* **Best For:** Information-heavy backends and data pipelines (DOP), or performance-critical game engines and simulations (DOD).
