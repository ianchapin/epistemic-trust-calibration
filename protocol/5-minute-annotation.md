# 5-Minute Annotation (v2) — Epistemic Trust Calibration

**Timebox:** 5 minutes (stop when the timer ends).  
**Purpose:** Constrain **how a representation may be used** (reliance), not whether it’s “true.”

**Not an approval process.** Never outputs: **approved / safe / compliant / ready**.  
**Completion does not justify action.** It only makes reliance explicit.

> **Warning:** If this becomes mandatory, ceremonial, or used as justification, **reduce trust in this process and cap reliance**.

---

## What you’re doing (one sentence)
You are adding a **use-constraint** *around* a representation so it can’t silently become an authority.

---

## The Minimal Card (copy/paste)

### 1) Representation (what is it?)
**Representation:**  
(What artifact are we relying on? model output / metric / summary / explanation / score)

**Source + freshness (1 clause):**  
(Where did it come from, and is it current enough for this use?)

### 2) Use + Decision Context (the risk shape)
**Intended use tier:** Exploratory / Explanatory / Operational / High-stakes  
**Context:** Stakes (L/M/H) · Reversibility (Y/Partial/N) · Detectability if wrong (Easy/Hard)

> If **stakes are high** and **detectability is hard**, assume you will be wrong *silently* → **cap reliance**.

### 3) Scope (two bullets, no essays)
- **Valid for:**  
- **Not valid for:**  

> If you can’t state scope plainly, assume scope is exceeded → **downgrade reliance**.

### 4) Dominant ambiguity → behavioral consequence (pick ONE)
Pick the *main* ambiguity that limits trust **right now**, and enforce exactly **one** consequence:

- **Semantic** → define term(s) before reliance escalation  
- **Contextual** → no reuse outside stated context; re-annotate on reuse  
- **Mapping** → name the proxy gap; require one “reality check”  
- **Structural** → name a key assumption; exclude a known edge/condition  
- **Normative** → name the value tradeoff; name who owns it

**Ambiguity:** ____ → **Consequence:** ____

### 5) Reliance (permission) + Cap (maximum) + Owner (accountability)
Choose one **reliance level** (what it may do), and state a **cap** (what it may *not* exceed here):

- **Input-only:** may inform thinking; **cannot justify action**
- **Supporting:** one factor among many; **cannot dominate**
- **Weight-bearing:** can drive action **in-scope** with checks/monitoring
- **Decisive:** rare; requires independent validation + explicit owner + appeal/fallback

**Reliance level:** ____  
**Reliance cap:** ____  
**Judgment owner (single person/role):** ____  

**Owner acceptance (1 sentence):**  
“I accept responsibility for acting within this cap, given remaining uncertainty.”

---

## 60-Second Add-On (only if stakes ≥ Medium)
### Failure tripwire (one line)
**Likely failure → how we’d notice → what we do immediately:**  
____ → ____ → ____

### Revision triggers (one each)
- **Raise reliance if:** ____  
- **Lower reliance if:** ____

---

## Default Caps (use when unsure)
- **High stakes + hard detectability ⇒ cap = Supporting**  
  unless you have **independent validation + monitoring + fallback/appeal**.
- **Reuse in a new context ⇒ downgrade one tier** until re-annotated.
- If this process increases confidence without adding checks/safeguards/ownership → **treat that as misuse** and **cap reliance**.

---

## Micro-example (2 lines)
**Representation:** LLM summary of incident timeline from chat + partial logs.  
**Context:** Stakes=High, Reversibility=Partial, Detectability=Hard.  
**Scope:** Valid for shared framing; Not for root cause/mitigations.  
**Ambiguity→Consequence:** Mapping→verify key claims against raw logs before action.  
**Reliance:** Supporting · **Cap:** Supporting · **Owner:** Incident Commander.

---

> Need a fuller version (failure modes, revision triggers, etc.)? Use the [`protocol/annotation-card.md`](annotation-card.md).
