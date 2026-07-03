---
name: theme-selection
description: Rank all 22 themes by evidence delta and pick 4-6 for this month's deep dives. Phase C of the monthly loop.
---

# theme-selection

## Purpose

Concentrate deep-dive effort where the evidence actually moved, instead of
regenerating all 22 themes every month.

## Input

grading_reports: output/YYYY-MM/01-grading/*.md
sweeps: output/YYYY-MM/02-sweep/*.md
history: SELECTION.md files from previous months (for the coverage rule)

## Scoring (per theme)

Score each theme 0–5 on each dimension and sum:

- Grade surprises: falsified or unexpectedly confirmed claims this month.
- Evidence delta: weight of new Confirmed Developments and Delta bullets.
- Contradiction density: counter-signals plus contradictions in the sweep.
- Staleness: months since last deep dive (5 if never deep-dived under
  method v2).

## Coverage rule

Every theme must be deep-dived at least once per 5 months. A theme reaching
month 5 without a dive is selected regardless of score.

## Output — output/YYYY-MM/SELECTION.md

```text
Selected Themes (4-6):
- <theme> — score N — one-line rationale citing specific sweep or grading items

Not Selected:
- <theme> — score N — one-line reason

Coverage Status:
| theme | months since last deep dive |
```

## Constraints

- Minimum 4 themes, maximum 6.
- Rationale must cite actual evidence items (claim IDs, sweep bullets),
  not general impressions.
- Deterministic: the same inputs must produce the same selection.
