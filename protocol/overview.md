# Protocol Overview (Minimal Implementation)

This page describes a minimal way to apply the framework.

It is not a decision engine.
It does not determine truth.
It provides a structured method for making trust, scope, and judgment explicit.

---

## Key Terms (to prevent confusion)

- **Trust** = whether reliance on this representation is appropriate at all for a given **purpose and scope**.
- **Reliance** = what this representation is **allowed to do** in this context (behavior / permission).
- **Reliance cap** = the **maximum permitted** reliance level in this context.
- **Confidence** = your **assessment** that the chosen reliance level (and cap) is warranted, given stakes, reversibility, detectability, and safeguards.

Confidence is not a probability estimate. It’s a justification for a reliance level (and cap).

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

2. **Trust (appropriate reliance at all?)**
   - Is reliance appropriate at all for the intended purpose and scope?
   - If yes: what purpose/scope is it trusted for?
   - If no: what use should be prohibited?

3. **Intended Use (Tier)**
   - What is it being used for right now?
   - Suggested tiers: exploratory, explanatory, operational, high-stakes

4. **Decision Context**
   - stakes, reversibility, detectability, time pressure, alternatives, safeguards (see below)

5. **Scope Boundaries**
   - Where does this apply, and where does it not apply?

6. **Ambiguity Types (and why)**
   - semantic, contextual, mapping, structural, normative

7. **Reliance Level (Permission Mode) + Reliance Cap**
   Pick the reliance level you are granting, and state the cap (the maximum permitted level) for this context:

   - **Input-only:** may inform thinking; cannot justify action
   - **Supporting:** one factor among many; cannot dominate
   - **Weight-bearing:** can drive action **in-scope** with checks/monitoring
   - **Decisive:** rare; requires independent validation + explicit owner + appeal/fallback

   **Confidence (optional):** Low / Medium / High — your assessment that this reliance level (and cap) is warranted in this decision context (given safeguards and failure detectability).

8. **Failure Modes**
   - failure → detectability → impact → mitigation

9. **Revision Triggers**
   - what would raise reliance or increase the cap?
   - what would lower reliance or reduce the cap?

10. **Judgment Handoff**
   - what cannot be resolved here
   - who owns the decision anyway

---

## Decision Context (Confidence Inputs)

Confidence calibration depends on the decision context **and safeguards** — and it exists to justify (or reject) a chosen reliance level (and cap).

Before assigning a reliance level, capture:

- **Stakes:** How costly is being wrong?
- **Reversibility:** Can we undo or revise the decision?
- **Detectability:** How quickly would failure be noticed?
- **Time pressure:** Are we acting now, soon, or later?
- **Alternatives:** What other representations or checks are available?
- **Safeguards:** What makes failure less likely, more detectable, or less costly? (monitoring, independent review, validation path, fallback, appeal, audits)

If these are unknown or contested, confidence should be reduced rather than assumed.

If you cannot justify the reliance level from the context + safeguards, downgrade reliance and/or reduce the cap.

---

## Failure Modes (Structured)

Failure modes should be written as:

- **Failure:** What breaks / what becomes false / what goes missing
- **Detectability:** easy / moderate / hard (or “likely to be noticed?”)
- **Impact:** what happens if we miss it
- **Mitigation:** verification, fallback, scope limit, second source, monitoring, human review

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
- trust (appropriate reliance at all) is stated for the purpose/scope
- intended use is explicit
- scope is explicit
- ambiguity types are named
- reliance level and reliance cap are explicit
- confidence is bounded and justified by context + safeguards
- failure modes are acknowledged
- judgment handoff is marked

No consensus is required.
The goal is not agreement; it is visible constraints.

---

## Minimal Template

- **Representation:**
- **Trust (appropriate at all?)** for purpose/scope:
- **Intended use (tier):**
- **Decision context:** stakes, reversibility, detectability, time pressure, alternatives, safeguards
- **Scope boundaries:**
- **Ambiguity types (why):**
- **Reliance level (permission mode):** Input-only / Supporting / Weight-bearing / Decisive — what this permits
- **Reliance cap:** maximum permitted reliance level in this context
- **Confidence (optional):** Low / Medium / High — why this reliance level/cap is warranted
- **Failure modes:** failure → detectability → impact → mitigation
- **Revision triggers:** raise / lower
- **Judgment handoff:** unresolved + owner

---

### Example (showing the difference)

- **Reliance:** Supporting (may guide discussion; cannot justify action)
- **Reliance cap:** Supporting (do not escalate without new checks)
- **Confidence:** Medium (stakes moderate, reversible, failures detectable, plus a second-source check)
