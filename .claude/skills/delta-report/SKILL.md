---
name: delta-report
description: Generate "The Delta Report", the accountability companion to the Outlook - how past claims graded, what shifted this month, which claims are now on the clock, and what the pipeline learned about its own biases. Manual, alongside the outlook.
---

# delta-report

## Purpose

Generate "The Delta Report": the accountability record that used to be wedged
into the outlook and broke its narrative. It exists for the reader who wants to
check the work. It carries the numbers so the essay does not have to.

Pair it with the outlook: the outlook tells the story, the delta report keeps
the receipts.

## Style rules (hard)

- NO em-dashes anywhere (use commas, periods, colons, parentheses).
- Plain, factual, unsentimental. This is an audit, not an essay.
- Report non-confirmed grades (decayed, falsified, expired) as plainly as
  confirmed ones. Honesty is the entire value of this document.

## Inputs

- `grading_reports` (this month's 01-grading/*.md, with scorecards)
- `sweeps` (for the "what shifted" deltas)
- `ledger` (open claims and their resolve-by dates)
- `calibration` (ledger/CALIBRATION.md)
- `selection` (SELECTION.md)
- `previous_delta` (last month's delta report, if any)

## Structure

1. **Standfirst.** Title, month, and one italic line stating this is the
   accountability companion to the Outlook.

2. **Scorecard.** How past claims graded this month: totals across
   confirmed / decayed / falsified / expired / open, and 2-4 sentences on the
   most instructive grades. Name the single most surprising grade. If the
   baseline being graded is the retired v1 boilerplate, say so and grade it
   once to mark the "before".

3. **What shifted this month.** The largest evidence deltas (from the sweeps'
   Delta Since Last Month sections and grading surprises), and why those themes
   were selected for deep dives. Reference the previous delta report when one
   exists.

4. **Claims now on the clock.** A compact table of the strongest forward
   claims with resolve-by dates: the tests the next reports will grade. Point
   to the ledger for the full set.

5. **What the pipeline is learning about itself.** The active calibration
   heuristics, in one plain sentence each. State that they weight future
   research but do not change skills (that is instrument-review's job).

6. **A note for the next method review** (optional). Any recurring pattern
   worth flagging for the quarterly instrument-review, logged not acted on.

## Constraints

- Do not tell the story or draw the near-term picture; that is the outlook.
- Do not prescribe policy.
- Every non-open grade must cite a source (inherited from the grading reports).
- If there is nothing meaningful to grade yet (e.g. new claims resolve in
  future months), say so plainly rather than padding.

## Quality checks before finalizing

- Zero em-dashes.
- At least one non-confirmed grade discussed plainly, if any exist.
- The claims-on-the-clock table has real resolve-by dates.
- Calibration heuristics match ledger/CALIBRATION.md exactly.
