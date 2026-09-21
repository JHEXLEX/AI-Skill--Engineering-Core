# Engineering Core v3.0

**v3.0 is a major architectural release.**

The project is no longer centered on mechatronics and game-development categories. It has been redesigned as a discipline-agnostic **Engineering Core** that applies reusable engineering principles across hardware, software, control, manufacturing, interactive systems, and R&D.

---

## What Changed

### A discipline-agnostic core

Engineering fields are no longer treated as separate top-level modes.

Mechanical, electrical/electronic, software, embedded, control, manufacturing, materials, systems, UX, and game development are now perspectives that are activated only when the problem needs them.

The core question is now:

> **Which engineering perspectives are required to make this decision correctly?**

---

### New core engineering principles

v3.0 introduces a universal engineering layer focused on:

- defining the real problem before choosing a solution,
- separating requirements from proposed implementations,
- distinguishing facts, assumptions, estimates, calculations, simulations, and measurements,
- evaluating meaningful alternatives and trade-offs,
- preferring the simplest sufficient solution,
- treating interfaces as critical risk points,
- accounting for tolerance, variation, edge cases, and failure behavior when relevant,
- preserving decision rationale,
- making important requirements verifiable,
- managing uncertainty instead of hiding it.

---

### New engineering cycle

The core workflow is now:

```text
Frame → Decompose → Generate → Analyze → Select → Implement → Verify → Learn
```

This is not a mandatory visible checklist. The skill scales the process to the importance and complexity of the task.

---

### Decision gates

Important decisions can now be screened through five compact gates:

- **Feasible?**
- **Meets requirements?**
- **Safe and robust?**
- **Implementable / manufacturable?**
- **Verifiable?**

These gates are meant to improve decision quality without forcing a large formal workflow into every answer.

---

### Stronger verification behavior

v3.0 places more emphasis on the difference between a model and a real system.

Calculations, simulations, benchmarks, and AI estimates can support a decision, but important outputs should also answer:

> **What measurement or test would prove this works?**

Verification is now part of the engineering process instead of an afterthought.

---

## Context and Token Architecture

The previous reference-based structure has been removed.

v3.0 ships as a **single self-contained engineering core** with no external reference modules.

The purpose is not merely to reduce package size. The new architecture also reduces unnecessary model work by avoiding:

- repeated rules across multiple reference files,
- loading domain instructions that are irrelevant to the current problem,
- repeatedly restating unchanged project context,
- formal analysis when the decision does not justify it,
- unnecessarily long output caused by process-heavy instructions.

Project continuity now follows a **delta model**: preserve the objective, confirmed requirements, critical decisions, assumptions, unresolved risks, and next step — then focus on what changed.

---

## Software and Game Development

Software and game-development support has **not** been removed.

It has been absorbed into the general engineering model.

When relevant, software work is evaluated through architecture, responsibility boundaries, data flow, error handling, edge cases, testability, performance and resource budgets, security, maintainability, and extensibility.

Game and interactive-system work can additionally include state management, networking, game loops, data-driven design, performance, and user experience.

The difference is that these are no longer privileged top-level categories.

---

## Breaking Changes

v3.0 is not a drop-in continuation of the old architecture.

### Removed

- Mechatronics-centered top-level structure
- Game-development-centered top-level structure
- Domain-specific reference modules
- Reference routing as a core behavior
- Repeated domain guidance stored in persistent context

### Added

- Discipline-agnostic engineering principles
- Cross-disciplinary routing by problem need
- Compact decision gates
- Stronger assumption and uncertainty handling
- Verification-first behavior
- Failure-aware reasoning
- Delta-based project state
- Response-economy rules
- A single self-contained skill package

---

## Migration Notes

If you were using the previous release as a mechatronics or game-development assistant, you can continue using v3.0 for those projects without selecting a dedicated mode.

Instead, describe the engineering problem and constraints directly. Engineering Core will combine the relevant perspectives as needed.

Old domain reference files are no longer required.

---

## Why v3.0?

The previous architecture could become broader only by adding more domain files. That improved coverage but also increased persistent instructions, routing complexity, repeated guidance, and potential context cost.

v3.0 changes the scaling model:

> **Do not store every discipline in the skill. Store the engineering principles that decide how disciplines should be used.**

The result is intended to be broader while remaining smaller, more predictable, and easier to maintain.

---

## Summary

Engineering Core v3.0 is:

- discipline-agnostic,
- self-contained,
- verification-oriented,
- failure-aware,
- trade-off driven,
- context-conscious,
- less dependent on persistent domain instructions.

The project is no longer a collection of engineering categories.

It is an **engineering operating model for AI-assisted problem solving**.
