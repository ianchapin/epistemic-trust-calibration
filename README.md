# Epistemic Trust Calibration

This repository contains a lightweight framework for calibrating how much trust representations deserve in a given context.

Representations include things like:
- models
- metrics
- explanations
- analogies
- summaries
- AI-generated outputs

⚠️ **Before using this framework, read [`CORE_CONSTRAINTS.md`](CORE_CONSTRAINTS.md) and [`MISUSE.md`](MISUSE.md).**  
If you are looking for approval, certainty, or legitimacy, this framework is not the right tool.

**Fastest on-ramp:** [`protocol/5-minute-annotation.md`](./protocol/5-minute-annotation.md) (then [`protocol/annotation-card.md`](./protocol/annotation-card.md) when you need more completeness)

---

## What This Is

This project provides:
- a set of core constraints that describe structural limits of thought and representation
- concepts for reasoning about trust, judgment, and uncertainty
- a taxonomy of ambiguity types that fail in different ways
- a protocol for **annotating representations**, not adjudicating truth
- speculative use cases to explore where the approach might or might not help

The focus is on **confidence allocation and bounded reliance**, not belief enforcement.

---

## What This Is Not

This framework does **not**:
- determine what is true
- certify correctness, safety, or responsibility
- replace human judgment
- eliminate ambiguity
- require consensus
- act as an authority or gate

It does not attempt to solve epistemology or automate decision-making.

---

## Who This Framework Is For

This framework is intended for people who:
- are already accountable for outcomes
- cannot fully defer responsibility upward
- must act despite uncertainty
- are wary of silent overconfidence in models, metrics, or explanations

It is **not** intended as:
- a persuasion tool
- a debate weapon
- a compliance checklist
- a way to block decisions without ownership
- a substitute for authority or responsibility

---

## Core Idea

Humans think and act through representations rather than interacting with reality directly.

Because representations are necessary and imperfect:
- certainty is always bounded
- trust is unavoidable
- misuse more often comes from overconfidence than malice

This framework treats representations as **tools rather than authorities** and focuses on making trust **explicit, scoped, and revisable**.

A central failure mode it addresses is mistaking representations for what they represent.

---

## How to Use This Repository

You do not need to agree with or adopt the entire framework to use it, and it is not intended to be applied universally.

Suggested reading order:
1. [`CORE_CONSTRAINTS.md`](./CORE_CONSTRAINTS.md)
2. [`MISUSE.md`](./MISUSE.md)
3. [`concepts/recursion.md`](./concepts/recursion.md)
4. [`concepts/representations.md`](./concepts/representations.md)
5. [`ambiguity/README.md`](./ambiguity/README.md)
6. Individual ambiguity type pages (see the files in [`ambiguity/`](./ambiguity/))
7. [`protocol/5-minute-annotation.md`](./protocol/5-minute-annotation.md)
8. [`protocol/annotation-card.md`](./protocol/annotation-card.md)
9. [`protocol/overview.md`](./protocol/overview.md)
10. [`use-cases/`](./use-cases/) (optional, speculative)

Each section is modular and intended to stand on its own.

---

## About the Protocol

The protocol provided in this repository:
- starts with a timeboxed **5-Minute Annotation** for rapid use: [`protocol/5-minute-annotation.md`](/protocol/5-minute-annotation.md)
- then uses the **Annotation Card** when you need more completeness: [`protocol/annotation-card.md`](/protocol/annotation-card.md)
- **annotates** representations rather than modifying them
- constrains *how* outputs are relied on, not *what* decisions must be made
- makes ambiguity, scope, and judgment visible
- explicitly preserves human responsibility

Completing the protocol does **not** mean a decision is correct, safe, or justified.

---

## Misuse Diagnostics

This framework is likely being misused if:
- it produces a pass/fail or approval outcome
- it is applied retrospectively to justify a decision
- judgment ownership is left blank, abstract, or collective
- ambiguity types are named without changing reliance or scope
- it is cited as evidence that a decision was “responsible”
- it increases confidence without adding safeguards, checks, or explicit ownership

In these cases, **reliance on the framework itself should be reduced**.

See [`MISUSE.md`](MISUSE.md) for detailed examples and anti-patterns.

---

## Recursion and Self-Application

This framework is **recursive**.

It is itself a representation and is subject to the same limits, ambiguities, and misuse patterns it describes.

If the framework:
- becomes mandatory
- feels authoritative
- produces closure rather than bounded confidence
- or is used to launder judgment

it is being misused.

See [`concepts/recursion.md`](concepts/recursion.md) for details on applying the framework to itself.

---

## Design Principles

- Ambiguity is unavoidable and must be made explicit
- Trust must be scoped and revisable
- Judgment is irreducible and should not be hidden
- Representations are tools, not authorities
- Overreach is a predictable failure mode

---

## What Success Looks Like

This framework is successful if it:
- slows or scopes at least some decisions
- prevents at least some silent confidence transfer
- makes at least some judgments explicit
- allows some decisions to proceed with **lower but honest confidence**

Widespread adoption, standardization, institutionalization, or endorsement are **not** success criteria.

---

## When This Framework Will Not Help

This framework is unlikely to help when:
- stakes are low and decisions are easily reversible
- outcomes are already well understood and agreed upon
- no one involved is accountable for the decision
- the goal is persuasion rather than action
- the framework is being used to delay without ownership

In these cases, added structure may introduce unnecessary friction.

---

## Status

This is an evolving framework.

The core constraints are intended to be stable.
Other sections may change, expand, or be removed as the framework is tested and refined.

---

## License

This project is released under the MIT License.
Use, adapt, fork, or discard it as you see fit.

---

## Author Note

This framework is intentionally incomplete.

Interpretations, adaptations, refusals, and even abandonment are expected.
No single reading should be treated as authoritative.
