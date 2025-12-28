# Decision Context

Decision context describes the conditions under which a representation is being used.

Confidence calibration is not only about the representation’s content.
It is also about the situation: stakes, reversibility, detectability, time pressure, and alternatives.

## Core Fields

- **Stakes**
  - What is the cost of being wrong?

- **Reversibility**
  - Can we undo or revise the decision after acting?

- **Detectability**
  - If we are wrong, how quickly will we notice?
  - Are failures visible or silent?

- **Time pressure**
  - Are we deciding now, soon, or later?

- **Alternatives**
  - What other representations, measurements, or checks are available?

## Why This Matters

A representation can be “good” and still deserve low reliance
if stakes are high, reversibility is low, and detectability is hard.

Conversely, a representation can be imperfect and still deserve moderate reliance
in low-stakes, reversible, quickly-detectable situations.

Decision context prevents confidence from being allocated as if all uses are the same.

Practical signal: If stakes are high, reversibility is low, and detectability is hard—but the representation is being treated as decisive—confidence is almost certainly overextended.