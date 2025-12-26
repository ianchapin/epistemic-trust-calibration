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

2. **Intended Use**
   - What is it being used for *right now*? (exploration, explanation, decision support, justification)

3. **Scope**
   - Where does this apply, and where does it not apply?

4. **Ambiguity Types**
   - Which ambiguity types are present? (semantic, contextual, mapping, structural, normative)

5. **Confidence (Reliance Level)**
   - How much weight should this carry, given stakes and reversibility?
   - (Qualitative is sufficient.)

6. **Known Failure Modes**
   - How could this fail in ways that matter?

7. **Judgment Handoff**
   - What cannot be resolved here, and where judgment must enter?

---

## Confidence Gating (Use Tiers)

A representation should not be used beyond the tier it has earned.

Typical tiers:
- **Exploratory:** generates hypotheses or options
- **Explanatory:** supports understanding or communication
- **Operational:** supports action with verification safeguards
- **High-stakes:** requires strong validation and explicit responsibility

Tier names can vary; the separation is what matters.

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

Use this template when applying the protocol:

- **Representation:**  
- **Intended use:**  
- **Scope:**  
- **Ambiguity types:**  
- **Confidence / reliance level:**  
- **Known failure modes:**  
- **Judgment handoff:**  

If the annotation cannot be filled out, confidence should be reduced rather than assumed.
