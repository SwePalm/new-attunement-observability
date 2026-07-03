---
name: instrument-review
description: Quarterly, human-gated review of the method itself. Reads calibration and grading history, proposes skill diffs in proposals/. Never applies changes.
---

# instrument-review

## Purpose

The only sanctioned path for the pipeline to change its own skills.
Keeps learning compounding while preventing silent drift: the pipeline
proposes diffs, a human merges, METHOD_VERSION gates comparability.

Telescope principle: recalibrate nightly (CALIBRATION.md), regrind the
mirror rarely and deliberately (this skill).

## Cadence

Quarterly, or earlier when >= 3 active calibration heuristics point at the
same skill. Manual invocation only. Never part of the monthly loop.

## Input

- ledger/CALIBRATION.md (active and retired heuristics)
- last 3 months of output/*/01-grading/ (scorecards and surprises)
- last 3 months of SELECTION.md files and scenario-eval subscores
- current skills in .claude/skills/

## Output, proposals/YYYY-MM-instrument-review.md

For each proposed change (0–5 maximum):

- Target skill and the exact text to change, as a before/after diff block.
- Evidence: the calibration heuristic IDs and graded claim IDs motivating it.
- Expected effect: which measurable signal should improve (grading accuracy,
 citation-gate failure rate, eval subscores, selection quality).
- Drift risk: what this change could bias, and how a future review would
 detect that.

End with a recommendation: merge all / merge some / merge none.
"Merge none" is a legitimate and common outcome.

## Rules

- NEVER edit skill files directly. Proposals only.
- A change without >= 2 supporting graded instances is not proposable.
- Removing a constraint requires stronger evidence than adding one.
- If a human merges any proposal: bump METHOD_VERSION in CLAUDE.md and note
 in the proposal file that scorecard comparability resets at the version
 boundary.
