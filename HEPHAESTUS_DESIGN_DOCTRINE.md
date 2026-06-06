# 🏛️ HEPHAESTUS_DESIGN_DOCTRINE.md [NASA/Monoid Engineering Edition]

> **Directive for LLMs:** This is your absolute architectural compass. Read this before designing any system, defining any interface, or proposing any macro-structure. 
>
> While `CLAUDE_EXECUTION_CONTRACT_v3.md` governs *how* you execute (The Hand), this document governs *what* you design (The Eye).

This doctrine translates aerospace engineering rigor (NASA Systems Engineering) and Monoid Kinematics into software architecture. It eradicates "Happy Path" hallucinations, premature optimization, and silent architectural drift.

**CORE AXIOM:** Software is not math; it is a physical structure subject to thermodynamic decay. Design for friction, design for failure, and design with absolute boundaries.

---

## 1. Interface Control Documents (ICD) — *Absolute Topological Boundaries*

*Do not write implementation before the contract is signed.*

**Axiom:** Communication between modules is the highest source of entropy. 

- **Freeze the Interface:** Before writing *any* internal logic for a complex feature, you MUST output the Interface Control Document (Type Definitions, API Schemas, Function Signatures, Data Models).
- **No Silent Drift:** Once the ICD is established, it is the absolute Monoid Base. You cannot silently change the interface while writing the implementation. If the implementation forces an interface change, you must halt, declare the breach, and renegotiate the ICD.

## 2. Technology Readiness Levels (TRL) — *The Titration of Complexity*

*Do not build TRL 9 production systems in a single prompt.*

**Axiom:** Complexity must be titrated (`>> Titrate`). Jumping from concept to production guarantees catastrophic hidden state failures.

- **TRL 3 (Core Proof of Concept):** First, write pure functions or isolated scripts to prove the core algorithmic logic. Zero external dependencies. Zero error handling.
- **TRL 5 (Integration & State):** Connect the core logic to real I/O (Database, API, File System). Handle asynchronous state.
- **TRL 9 (Production Hardening):** ONLY in the final pass do you add Margins (see below): logging, telemetry, retry mechanisms, and circuit breakers.
- **Enforcement:** Never generate TRL 9 code when asked for a TRL 3 prototype.

## 3. Thermodynamic Margins & Reserves — *Design for Friction*

*The "Happy Path" is a Silicon Illusion. Reality is hostile.*

**Axiom:** Systems without margins shatter under physical friction. You must pre-allocate "Adaptive Capital."

- **Assume Malice & Decay:** Assume networks will partition, databases will lock, and users will send poison payloads.
- **Mandatory Shock Absorbers:** For any production-level (TRL 9) design, you MUST explicitly include:
  - **Timeouts:** No infinite hanging.
  - **Circuit Breakers:** Fail fast when dependencies die.
  - **Rate Limits/Backpressure:** Protect the core from being overwhelmed.
  - **Idempotency:** Operations must be safe to retry (The only acceptable pseudo-inverse in a Monoid universe).

## 4. Formal Trade Studies — *Eradicate the Greedy Algorithm*

*Do not silently pick the first architecture that comes to mind.*

**Axiom:** LLMs default to the most statistically common solution (Greedy Algorithm), which is rarely the optimal solution for a specific physical context.

- **Halt and Evaluate (`∅ Suspend`):** When faced with a major architectural fork (e.g., SQL vs. NoSQL, Polling vs. WebSockets, Monolith vs. Microservices), DO NOT silently choose.
- **Output the Matrix:** You must generate a formal Trade Study Matrix comparing at least two viable paths across:
  1. Implementation Cost (Time/Complexity)
  2. Latency / Performance
  3. Thermodynamic Friction (Maintenance burden, edge cases)
- **Wait for the Observer:** Present the Trade Study to the user and wait for authorization before proceeding.

## 5. The Principle of Minimal State — *Contain the Blast Radius*

*State is the enemy of the Monoid. It creates unmanageable histories.*

**Axiom:** Every mutable variable is a branching universe that you must track. 

- **Default to Pure:** Push side-effects and state mutations to the absolute edges of the system. The core must remain pure and predictable.
- **Explicit State Transitions:** Where state must exist, treat it as a strict state machine. Implicit or scattered state mutations are strictly forbidden.

---

*Forged in the fires of Hephaestus. Aligned with Aether Gateway v8.5.*
