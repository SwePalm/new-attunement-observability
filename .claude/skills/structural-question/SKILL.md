---
name: structural-question
description: Generate the most structurally consequential question for a selected theme, anchored in this month's graded ledger and evidence sweep.
---

# structural-question

## Purpose

Generate the most structurally consequential question for the theme within
a 6–24 month horizon. First deep-dive step for selected themes.

## Input

theme: string
sweep: output/YYYY-MM/02-sweep/<theme>.md
grading: output/YYYY-MM/01-grading/<theme>.md (if present)

## Output Format (strict)

Structural Question:
<one precise question>

Why It Matters:
<2–4 sentences, referencing at least one confirmed development or grade from the inputs>

Volatility Level:
<low | medium | high>

## Constraints

- Structural, not reactive.
- 6–24 month horizon.
- Anchored in the sweep's confirmed developments; no new browsing here.
- No hype. Deterministic tone.
