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
