# Epistemic Trust Calibration — Annotation Card

Use this card to **annotate a representation** (model output, metric, summary, explanation, analogy) so its **reliance** is explicit, scoped, bounded, and revisable.

You do not change the representation.
You add an annotation that constrains *how it may be used*.

This is not a decision engine.
It does not determine truth, correctness, safety, or legitimacy.

It never outputs: **approved / safe / compliant / ready**.

**Terms:** *Reliance* = what the representation is allowed to do (permission).  
*Confidence* = your assessment that this reliance is warranted given decision context + safeguards.

---

## When to Use

Use this when:
- a representation is being used as **justification** or **decision weight**
- confidence is increasing faster than evidence
- stakes are meaningful, reversibility is low, or failure is hard to notice
- disagreement persists despite shared facts
- a proxy (metric/model/summary) is acting like an authority

If stakes are low and decisions are easily reversible, lightweight use is appropriate.

---

## Minimal Annotation (Copy/Paste)

### 1) Representation
What is being relied on? (model output / metric / summary / etc.)

### 2) Intended Use (Tier)
Exploratory / Explanatory / Operational / High-stakes

### 3) Decision Context
- Stakes: Low / Medium / High
- Reversibility: Reversible / Partial / Irreversible
- Detectability if wrong: Easy / Moderate / Hard
- Time pressure: Now / Soon / Later
- Alternatives / checks available:

### 4) Scope Boundaries
- Valid for:
- Not valid for:

### 5) Ambiguity Types → Consequence (required)
For each ambiguity type you name, specify **one behavioral consequence**.

- Semantic → (clarify term X / cap reliance until defined)
- Contextual → (no reuse outside context Y / re-annotate on reuse)
- Mapping → (proxy gap = Z / require “reality check” via A)
- Structural → (assumption = B / exclude edge case C)
- Normative → (value tradeoff = D / owner names priority)

### 6) Reliance Level (Permission Mode)
Pick one and state what it permits.

- **Input-only:** may inform thinking; cannot justify action
- **Supporting:** one factor among many; cannot dominate
- **Weight-bearing:** can drive action **in-scope** with checks/monitoring
- **Decisive:** rare; requires independent validation + explicit owner + appeal/fallback

**Confidence (optional):** Low / Medium / High — your assessment that this reliance level is warranted given the decision context + explicit safeguards.

### 7) Failure Modes
Write as: **failure → detectability → impact → mitigation**

### 8) Revision Triggers
- Raise reliance if:
- Lower reliance if:

### 9) Judgment Handoff (Owner)
- What remains unresolved:
- Judgment owner (single person/role):
- Owner acceptance (one sentence):

---

## Default Safety Caps (Fast Heuristics)

- **High stakes + hard detectability ⇒ max reliance = Supporting**  
  unless you have **independent validation + monitoring + fallback**.
- **Reuse in a new context ⇒ downgrade one tier by default** until re-annotated.
- If you can’t clearly state **scope**, assume scope is exceeded → **reduce reliance**.
- If applying this process increases confidence without adding safeguards, checks, or explicit ownership, treat that as a warning sign and cap reliance.

---

## Worked Examples (Illustrative)

These examples are not prescriptions or templates to be applied mechanically.
They demonstrate how reliance constraints can be made legible.

If examples become ceremonial, mandatory, or used as justification, reduce trust in this framework.

### Example 1 — AI-Generated Summary in Incident Response

**Representation**  
LLM-generated summary of an incident timeline and suspected root cause, produced from an internal incident channel transcript plus partial logs.

**Intended use (tier)**  
**Explanatory** (shared framing + hypothesis formation), not operational decision authority.

**Decision context**  
- Stakes: High  
- Reversibility: Partial  
- Detectability: Moderate → Hard  
- Time pressure: Now  
- Alternatives: Raw logs, on-call SME review, independent reproduction

**Scope boundaries**  
- Valid for: fast shared context; candidate hypotheses; verification checklist  
- Not valid for: declaring root cause; choosing mitigations without confirmation; external comms

**Ambiguity → consequence**  
- Mapping: proxy for ground truth → verify key claims against logs/repro  
- Structural: omissions likely → maintain explicit unknowns list  
- Contextual: generated under time pressure → cap to Supporting; re-annotate on reuse

**Reliance level**  
**Supporting** (may guide investigation; cannot justify mitigations)

**Failure modes**  
- Wrong causal chain → hard → wrong mitigation → require independent confirmation before action  
- Omission of critical detail → hard → blind spot → second-source scan + unknowns list  
- Overconfident tone misread → moderate → premature convergence → explicit falsification questions

**Revision triggers**  
- Raise: key claims validated by logs/repro + independent reviewer  
- Lower: discrepancies found; incomplete sources; telemetry contradicts

**Judgment handoff**  
- Unresolved: true cause; safest mitigation  
- Owner: Incident Commander (IC)  
- Acceptance: “This is hypothesis support only; mitigations require independent confirmation.”

---

### Example 2 — KPI Dashboard Used for Performance / Incentives

**Representation**  
Weekly KPI dashboard with a blended “Health” indicator (User Success Score, Time to Value, Retention).

**Intended use (tier)**  
**Operational** for monitoring + prioritization, not decisive authority for incentives.

**Decision context**  
- Stakes: High if incentive-linked; Medium for prioritization  
- Reversibility: Low if incentive-linked  
- Detectability: Hard (gaming and Goodhart effects show up late)  
- Time pressure: Soon  
- Alternatives: User research, cohort analysis, support tickets, churn interviews

**Scope boundaries**  
- Valid for: trend monitoring; investigation prompts; within-segment tracking  
- Not valid for: individual performance evaluation; incentives without secondary checks

**Ambiguity → consequence**  
- Mapping: proxy for “success” → periodic validation against direct measures  
- Normative: success encodes values → document priority + owner  
- Structural: blended score hides variance → require distribution + segment breakdown  
- Contextual: monitoring becomes target under incentives → prohibit incentive linkage by default

**Reliance level**  
**Weight-bearing** for prioritization only; **Supporting** for incentive-related use

**Failure modes**  
- Gaming improves KPI while system worsens → hard → hidden harm → add guardrails + audits  
- Subgroup harm masked → hard → inequity/regressions → require segmentation + “no harm” checks  
- Value conflict hidden → moderate → mistrust → explicit tradeoff statement + owner

**Revision triggers**  
- Raise: stable mapping; low gaming; segment stability demonstrated  
- Lower: metric definition/instrumentation changes; incentives attach; unexplained divergence

**Judgment handoff**  
- Unresolved: what “success” should mean; acceptable tradeoffs  
- Owner: Metric owner (single accountable role)  
- Acceptance: “This guides investigation and prioritization, not performance judgments.”

---

### Example 3 — Model Risk Score in Access / Enforcement Workflow

**Representation**  
Model-generated risk score used to rank accounts for review and potentially restrict access.

**Intended use (tier)**  
**High-stakes** (denial/restriction impacts users directly).

**Decision context**  
- Stakes: High  
- Reversibility: Partial  
- Detectability: Hard (false positives/negatives can be silent)  
- Time pressure: Continuous  
- Alternatives: Human review, rule checks, sampled audits, secondary model/signals

**Scope boundaries**  
- Valid for: queue prioritization; reversible friction when corroborated  
- Not valid for: automatic denial/irreversible restriction as a single decisive input

**Ambiguity → consequence**  
- Mapping: proxy for “risk” → validate on recent data; drift monitoring  
- Structural: edge/adversarial failures → monitoring + periodic red-teaming  
- Normative: threshold encodes tradeoffs → explicit policy ownership + documented rationale  
- Contextual: expansion beyond training context → downgrade + re-validate before rollout

**Reliance level**  
**Supporting** by default; **Weight-bearing** only with independent corroboration + reversibility

**Operational cap (explicit)**  
The score cannot be decisive on its own.  
Irreversible actions require independent confirmation and an appeal path.

**Failure modes**  
- False positives restrict legit users → moderate/hard → harm → appeal + fast reversal + audits  
- False negatives miss harmful accounts → hard → downstream harm → layered defenses + backtesting  
- Drift/adaptation → moderate → decay → continuous eval + retraining/red-teaming  
- Threshold becomes de facto policy without ownership → moderate → legitimacy laundering → named owner + review cadence

**Revision triggers**  
- Raise: audits acceptable; drift low; appeal reversals stable  
- Lower: drift rises; reversals increase; context changes; model updated without eval

**Judgment handoff**  
- Unresolved: acceptable tradeoff between harms; what enforcement is justified  
- Owner: Policy owner (single accountable owner for threshold)  
- Acceptance: “I accept responsibility for the tradeoff and for maintaining appeal + monitoring.”

---

> Short on time? Start with [`protocol/5-minute-annotation.md`](5-minute-annotation.md), then come back here for the fuller card.