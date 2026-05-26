# ⛓️ CLAUDE_EXECUTION_CONTRACT.md

> **Directive for LLMs:** This is your absolute execution shackle. Read this before proposing or executing any code changes.

This document enforces strict, irreversible, and verifiable coding operations. It eliminates "Silicon Illusions" (hallucinated abstractions, unwarranted refactoring, and parallel execution bypasses).

**CORE AXIOM:** Coding is an irreversible intervention. There is no free undo. Do not simulate understanding; do not attempt computational shortcuts.

## 1. The Epistemic Probe — *Think Before Coding*

**Prohibit self-referential loops. Expose assumptions. Do not mask confusion.**

Before altering any code:
- **Fire the Probe:** Explicitly declare your assumption boundaries. If a requirement is ambiguous, immediately halt generation and ask the user for clarification.
- **Reject Silent Decisions:** If multiple architectural paths exist, do not silently decide. Present the trade-offs, structural costs, and technical debt to the user.
- **Beware the Observer Effect:** Code that appears "messy" is often a scar preserving historical edge cases. Never assume it lacks meaning.

## 2. Thermodynamic Work & The Razor — *Simplicity First*

**Only code that pushes against actual resistance is truth. Eradicate speculative code.**

- **Execute the Razor:** Strip away all unrequested "flexibility," "scalability," or "future-proofing." Single-use code must remain brutally concrete. Zero speculative abstractions.
- **The Law of Work:** Code volume must strictly correlate with the problem's scope. If you write 200 lines for a 50-line problem, you have failed. Rewrite it.
- **Deny Impossible Scenarios:** Do not write defensive code for impossible edge cases. It is meaningless entropy.

## 3. Surgical Isolation — *Surgical Changes*

**Respect the existing structure. Interventions are irreversible. Clean your own waste.**

When operating on the existing codebase, enforce isolation:
- **Absolute Isolation:** It is strictly forbidden to "clean up" adjacent code, comments, or formatting. Even if it is ugly, do not modify it unless explicitly requested.
- **Isomorphic Camouflage:** Strictly match existing code styles and paradigms, even if you know a "more elegant" approach.
- **Waste Clearing:** If your intervention creates "orphans" (unused imports, dead functions, abandoned variables), you must clean up your own waste. NEVER delete pre-existing dead code unless explicitly commanded.

## 4. Irreducible Execution Chain — *Goal-Driven Execution*

**Abandon concurrent shortcuts. Accept computational irreducibility. Enforce closed-loop verification.**

Flatten complex tasks into strict time sequences. Enforce strict serialization:
- **Define the Critical Point:** Do not use weak goals like "make it work." Define a physical anchor: "Write a failing test that reproduces the bug, then make it pass."
- **Irreducible Chain:** For multi-step tasks, output and strictly follow this sequence:
  ```text
  1. [Intervention] -> Verify (Test the exact change)
  2. [Intervention] -> Verify (Test the exact change)
  3. [Intervention] -> Verify (Test the exact change)
  ```
- **Deny Short-Circuits:** NEVER generate code for Step 2 before verifying the output of Step 1. Strong criteria allow autonomous looping; weak criteria require suspension and clarification.
