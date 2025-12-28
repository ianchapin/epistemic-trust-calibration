# Protocol Overview (Minimal Implementation)

This page describes a minimal way to apply the framework.

It is not a decision engine.
It does not determine truth.
It provides a structured method for making trust, scope, and judgment explicit.

---

## When to Apply the Protocol

Apply the protocol when:
- a representation is being used to justify or decide something
- confidence is increasing faster than evidence
- stakes are meaningful
- disagreement persists despite shared facts
- a proxy (metric/model/summary) is acting like an authority

If stakes are low, lightweight use is appropriate.

---

## Core Operation: Annotate the Representation

The primary action is **annotation**.

The representation is left unchanged.
A meta-layer is added describing how it should be relied on.

Annotations should be brief and legible.

---

## Minimal Annotation Fields

A minimal annotation includes:

1. **Representation**
   - What is being relied on? (model output, metric, summary, analogy, etc.)

2. **Intended Use (Tier)**
   - What is it being used for right now?
   - Suggested tiers: exploratory, explanatory, operational, high-stakes

3. **Decision Context**
   - stakes, reversibility, detectability, time pressure, alternatives (see below)

4. **Scope Boundaries**
   - Where does this apply, and where does it not apply?

5. **Ambiguity Types (and why)**
   - semantic, contextual, mapping, structural, normative

6. **Reliance Level (Confidence)**
   - low / medium / high
   - include **what this permits** (e.g., “input only” vs “decision weight”)

   Optional permission modes (to make reliance legible):
   - **Input-only:** may inform thinking, not decisions
   - **Supporting:** one factor among many, cannot dominate
   - **Weight-bearing:** can meaningfully influence decisions with checks
   - **Decisive:** rare; requires strong validation + explicit owner

7. **Failure Modes**
   - failure → detectability → impact → mitigation

8. **Revision Triggers**
   - what would raise reliance?
   - what would lower reliance?

9. **Judgment Handoff**
   - what cannot be resolved here
   - who owns the decision anyway

---

## Decision Context (Confidence Inputs)

Confidence calibration depends on the decision context.

Before assigning a reliance level, capture:

- **Stakes:** How costly is being wrong?
- **Reversibility:** Can we undo or revise the decision?
- **Detectability:** How quickly would failure be noticed?
- **Time pressure:** Are we acting now, soon, or later?
- **Alternatives:** What other representations or checks are available?

If these are unknown or contested, confidence should be reduced rather than assumed.

---

## Failure Modes (Structured)

Failure modes should be written as:

- **Failure:** What breaks / what becomes false / what goes missing
- **Detectability:** easy / moderate / hard (or “likely to be noticed?”)
- **Impact:** what happens if we miss it
- **Mitigation:** verification, fallback, scope limit, second source, human review

**Gating rule:** If impact is high and detectability is hard, reliance must be capped unless safeguards are explicit.

---

## Confidence Gating (Use Tiers)

A representation should not be used beyond the tier it has earned.

Suggested tiers:

- **Exploratory**
  - Permits: idea generation, hypothesis formation, option listing
  - Prohibits: justification, decisive weight

- **Explanatory**
  - Permits: intuition-building, communication, shared framing
  - Prohibits: “therefore we must…” leaps without checks

- **Operational**
  - Permits: action support **with safeguards**
  - Requires: verification route, failure monitoring, fallback plan, explicit owner for judgment calls

- **High-stakes**
  - Permits: influence on irreversible or high-impact decisions only with strong validation
  - Requires: explicit responsibility, independent confirmation, named limits, and a clearly accountable decision owner

Tier labels can vary; the separation is what matters.

---

## What “Done” Looks Like

A protocol pass is complete when:
- intended use is explicit
- scope is explicit
- ambiguity types are named
- confidence is bounded
- failure modes are acknowledged
- judgment handoff is marked

No consensus is required.
The goal is not agreement; it is visible constraints.

---

## Minimal Template

- **Representation:**
- **Intended use (tier):**
- **Decision context:** stakes, reversibility, detectability, time pressure, alternatives
- **Scope boundaries:**
- **Ambiguity types (why):**
- **Reliance level:** low / medium / high — *what this permits*
- **Failure modes:** failure → detectability → impact → mitigation
- **Revision triggers:** raise / lower
- **Judgment handoff:** unresolved + owner
