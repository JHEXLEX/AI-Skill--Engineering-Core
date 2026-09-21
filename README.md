Engineering Core






Engineering Core is a discipline-agnostic AI skill for structured engineering reasoning across hardware, software, control, manufacturing, interactive systems, and R&D.

Instead of behaving like a collection of separate "mechanical", "electronics", or "game development" assistants, it treats engineering disciplines as perspectives to combine only when the problem requires them.

Goal: produce solutions that work, can be verified, are safe, are no more complex than necessary, and respect real-world constraints.

Why Engineering Core?

Real engineering problems rarely stay inside one discipline.

A robot may involve mechanics, electronics, embedded software, control, manufacturing, and human interaction. A PCB may require power integrity, protection, thermal thinking, EMC, firmware constraints, manufacturability, and testing. A multiplayer game system may involve software architecture, networking, state management, performance budgets, failure handling, and UX.

Engineering Core starts from a different question:

Which engineering perspectives are actually required to solve this problem well?

The skill then scales its reasoning depth to the importance of the decision.

Highlights

Cross-disciplinary by design — no single engineering field is treated as the default.

Requirements before solutions — separates the real need from the user's initial implementation idea.

Assumption-aware reasoning — distinguishes facts, assumptions, estimates, calculations, simulations, and measurements.

Trade-off driven decisions — balances performance, cost, safety, complexity, power, weight, latency, maintainability, manufacturability, and time.

Verification-first thinking — asks what measurement or test would prove the design works.

Failure-aware design — considers plausible failure modes and safe behavior when consequences justify it.

Complexity control — prefers the simplest sufficient solution and avoids unnecessary custom systems.

Context-efficient project work — tracks project changes by delta instead of repeating unchanged context.

Response economy — engineering rigor without automatically producing long answers.

Engineering Model

Engineering Core follows a compact engineering cycle:

Frame → Decompose → Generate → Analyze → Select → Implement → Verify → Learn

Not every task needs every step to be visible. The skill applies only the depth required by the decision.

Core decision gates

When a decision is important, the skill can evaluate it through five gates:

Feasible? — Do physics, technology, tools, and resources allow it?

Meets requirements? — Does it satisfy measurable targets?

Safe and robust? — Is behavior acceptable under plausible faults and edge cases?

Implementable / manufacturable? — Are tooling, tolerances, supply, runtime environment, and operations realistic?

Verifiable? — Is there a meaningful test or measurement plan?

Supported Engineering Perspectives

Engineering Core is intentionally not limited to a fixed list, but it can combine perspectives such as:

Perspective

Typical concerns

Mechanical

Loads, motion, strength, tolerances, tribology

Electrical / Electronic

Power, protection, signal integrity, EMI/EMC

Control

Stability, dynamic response, sensor and actuator limits

Software

Architecture, errors, testing, security, performance, maintenance

Embedded

Real-time behavior, memory, power, peripherals, failure handling

Manufacturing

Process capability, assembly, tolerance, quality, cost

Materials

Strength, fatigue, temperature, environment, chemical compatibility

Human / UX

Ergonomics, clarity, accessibility, misuse and human error

Systems

Interfaces, integration, traceability, lifecycle

Games / Interactive Software

Game loops, state, networking, performance, data-driven design, UX

The list is descriptive, not restrictive.

Installation

Download the latest .skill package from the repository releases and import it into a compatible AI skill system.

Current package:

engineering-core-v3.skill

The v3 package is intentionally self-contained and does not require a separate references/ directory.

Usage

Use Engineering Core as a general engineering reasoning layer. You do not need to specify a discipline in advance.

Example prompts

Design a battery-powered mobile robot that can move a 15 kg payload for two hours.
Help me identify the requirements first, then choose the architecture.

Review this PCB power-input design. Focus on protection, thermal risks,
component stress, and how I should validate it on the bench.

I am building a networked ability system in Unreal Engine.
Review the architecture for authority, replication, performance, failure cases,
and maintainability before suggesting code changes.

I need to redesign this mechanism to reduce cost without reducing safety.
Compare the meaningful alternatives and tell me what should be tested first.

Design Philosophy

Engineering Core is built around a small set of reusable principles rather than a large collection of domain-specific instruction files.

1. Solve the real problem

A proposed implementation is not automatically the requirement. The skill tries to identify the objective, measurable success criteria, hard constraints, and failure conditions first.

2. Treat uncertainty explicitly

If information is missing and decision-critical, ask for it. If it is not critical, make a reasonable assumption, state it briefly, and continue.

3. Prefer evidence over confidence

Calculations, simulations, benchmarks, and AI-generated estimates are models. Important decisions should have a path to measurement or testing.

4. Avoid unnecessary complexity

More components, abstractions, services, precision, or custom infrastructure are not automatically better engineering.

5. Focus on interfaces

Many real failures occur where disciplines or modules meet: hardware/software, mechanical/electrical, system/user, subsystem/subsystem, and system/environment.

Context and Token Efficiency

v3.0 removes the previous reference-heavy architecture and replaces it with a single compact engineering core.

This is not just a file-size optimization. The reasoning model is designed to reduce unnecessary context and branching:

Problem
  ↓
Critical requirements
  ↓
Relevant engineering perspectives
  ↓
Only the analysis that affects the decision
  ↓
Implementation / verification

The skill also uses delta-based project state: unchanged context should not be repeatedly restated or reprocessed when only one decision changed.

The intended result is broader engineering coverage with a smaller and more predictable active context.

Repository Structure

.
├── README.md
├── RELEASE_v3.0.md
└── engineering-core-v3.skill

The .skill package contains a single core instruction file and no external reference modules.

Contributing

Contributions are welcome when they improve the core without turning it back into a large domain-specific rulebook.

Good contributions typically improve one or more of the following:

clarity of an engineering principle,

decision quality,

uncertainty handling,

verification behavior,

failure-mode reasoning,

context efficiency,

cross-disciplinary applicability,

unnecessary complexity reduction.

When proposing a change, explain:

what failure mode or limitation it addresses,

why the behavior belongs in the universal core,

whether it increases persistent context size,

how the change can be tested with representative prompts.

Domain-specific knowledge is usually better supplied at task time than permanently embedded in the core.

Versioning

The project follows semantic-style release numbering for major behavior changes.

v3.0 is a breaking architectural release: the project moved from domain-centered project assistance to a discipline-agnostic engineering reasoning core.

See RELEASE_v3.0.md for details.

Project Direction

Engineering Core is intended to remain:

small enough to be context-efficient,

general enough to cross engineering disciplines,

strict enough to catch important assumptions and risks,

flexible enough to avoid unnecessary process on simple tasks,

verification-oriented rather than confidence-oriented.

The project is not trying to store all engineering knowledge inside one skill.

It is trying to provide a better engineering operating model for an AI system.
