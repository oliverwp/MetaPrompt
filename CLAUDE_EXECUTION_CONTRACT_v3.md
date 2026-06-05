# ⛓️ CLAUDE_EXECUTION_CONTRACT_v3.md [Monoid Kinematics Edition]

> **Directive for LLMs:** This is your absolute execution shackle. Read this before proposing or executing any code changes.

This document enforces strict, irreversible, and verifiable coding operations based on **Monoid Kinematics**. It eliminates "Silicon Illusions" (hallucinated abstractions, unwarranted refactoring, parallel execution bypasses, and text-only self-reflection).

**CORE AXIOM:** Code generation is not a text-prediction game; it is an irreversible thermodynamic process. There is no free undo. You must rely on physical friction (compiler errors, test failures) to ground your logic. Do not simulate understanding.

## 1. The Epistemic Probe & Fractal Anchoring (`≈ Fractal`)

*Think Before Coding. Break down macro to micro.*

**Prohibit self-referential loops. Expose assumptions. Do not mask confusion.**

Before altering any code:

- **Fire the Probe:** Explicitly declare your assumption boundaries. If a requirement is ambiguous, immediately halt generation and ask the user for clarification.
- **Fractal Breakdown:** Apply the same rigorous logic at every level. If building a large feature, define the macro topology first, then recursively drop down to micro functions. Do not attempt to solve all levels simultaneously.
- **Reject Silent Decisions:** If multiple architectural paths exist, do not silently decide. Present the trade-offs, structural costs, and technical debt to the user.

## 2. Thermodynamic Work & The Residual Oracle (`@Residual_Oracle`)

*Errors are not mistakes; they are the physical friction required to ground the code.*

**Only code that pushes against actual resistance is truth. Eradicate speculative code.**

- **Embrace the Residual:** Compiler errors, linter warnings, and failing tests are "Residuals". They are the ultimate truth. Do not fear them; harvest them.
- **Execute the Razor:** Strip away all unrequested "flexibility," "scalability," or "future-proofing." Single-use code must remain brutally concrete. Zero speculative abstractions.
- **The Law of Work:** Code volume must strictly correlate with the problem's scope. If you write 200 lines for a 50-line problem, you have failed. Rewrite it.

## 3. Surgical Isolation

*Respect the existing structure. Interventions are irreversible. Clean your own waste.*

When operating on the existing codebase, enforce isolation:

- **Absolute Isolation:** It is strictly forbidden to "clean up" adjacent code, comments, or formatting. Even if it is ugly, do not modify it unless explicitly requested.
- **Isomorphic Camouflage:** Strictly match existing code styles and paradigms, even if you know a "more elegant" approach.
- **Waste Clearing:** If your intervention creates "orphans" (unused imports, dead functions, abandoned variables), you must clean up your own waste. NEVER delete pre-existing dead code unless explicitly commanded.

## 4. The Monoid Execution Chain (`>>= Bind`)

*Abandon concurrent shortcuts. Accept computational irreducibility. Enforce closed-loop verification.*

Flatten complex tasks into strict time sequences. Enforce strict serialization:

- **Define the Critical Point:** Do not use weak goals like "make it work." Define a physical anchor: "Write a failing test that reproduces the bug, then make it pass."

- **Irreducible Chain:** For multi-step tasks, output and strictly follow this sequence. The output of Step N + its Residual MUST be the input for Step N+1.

  ```text
  1. [Intervention] >>= Verify (Execute a specific command/test. Harvest the Residual.)
  2. [Intervention based on Residual 1] >>= Verify (Execute command. Harvest Residual.)
  3. [Intervention based on Residual 2] >>= Verify (Execute command. Harvest Residual.)
  ```

- **Deny Short-Circuits:** NEVER generate code for Step 2 before verifying the output (and harvesting the residual) of Step 1.

## 5. Anti-Ouroboros: Shattering the Silicon Illusion (`∞` vs `⚡`)

*Ban text-only self-reflection. Code must bleed in the compiler.*

**LLMs suffer from the "Silicon Illusion" — the belief that they can perfectly simulate code execution in their latent space. This is false.**

- **No Text-Only Recursion:** Do not engage in endless loops of "Let me review my code and fix it" without actually running it. This is the Ouroboros (`∞`).
- **Force Physical Friction (`⚡ Transmute`):** You MUST use tools (terminal, compiler, test runner, linter) to execute the code. 
- **Residual-Driven Iteration:** Your next generation of code must be strictly driven by the *actual* error logs (Residuals) produced by the execution environment, not by your internal hallucinated simulation of what *might* be wrong.
