# Scope

In this framework, *scope* refers to the boundaries within which a representation can be reasonably relied upon.

Scope answers the question:
> “What is this representation meant to cover — and what is outside of it?”

Scope is not about correctness.
It is about applicability.

---

## Why Scope Matters

Representations are created for particular purposes, under particular assumptions, in particular conditions.

Scope defines:
- what a representation was designed to do
- what it was not designed to do
- where its reliability reasonably applies

Most failures involving representations are not caused by errors in content, but by using them outside their intended scope.

---

## Scope Is Often Implicit

Scope is rarely stated explicitly.

Instead, it is:
- inferred from context
- assumed from prior success
- carried forward by habit
- expanded gradually over time

Because scope is implicit, it tends to expand without deliberate decision.

This expansion often feels rational and efficient in the moment.
Its risks usually appear only later.

---

## Scope Creep

*Scope creep* occurs when a representation is asked to support uses beyond those it was designed for, without reassessing trust or confidence.

Common patterns include:
- exploratory tools becoming decision tools
- summaries becoming justifications
- metrics becoming targets
- models becoming guarantees

As scope expands, confidence often increases rather than decreases, even though reliability does not.

---

## Scope and Context

Scope is related to context, but they are not the same.

- **Context** refers to the situation in which a representation is used.
- **Scope** refers to the range of uses the representation can support.

A representation may be used in the same context but for a different purpose, thereby exceeding its scope.

Conversely, a representation may remain within scope across multiple contexts.

Distinguishing scope from context helps diagnose failure more precisely.

---

## Scope and Trust

Trust is always scoped.

To trust a representation without specifying scope is to trust it everywhere by default.

This framework treats unscoped trust as a warning sign.

Explicitly stating scope allows:
- partial trust
- conditional reliance
- controlled reuse
- safer revision when conditions change

---

## How This Framework Treats Scope

This framework encourages:
- explicitly stating intended scope
- resisting automatic scope expansion
- reassessing trust when scope changes
- reducing confidence as scope widens
- marking where judgment is required to approve scope extension

Scope boundaries are not rigid rules.
They are reminders of design intent.

---

## Practical Signal

If a representation is being used in a way that requires asking:
- “Can it really do that?”
- “Was it meant for this?”
- “Are we stretching it?”

scope is likely being exceeded.

In such cases, the appropriate response is not rejection,
but explicit discussion of scope and its limits.
