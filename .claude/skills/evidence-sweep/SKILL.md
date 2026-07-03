---
name: evidence-sweep
description: Real, cited research scan for one theme — what changed since last month — plus new falsifiable ledger claims. Runs for all 22 themes as Phase B.
---

# evidence-sweep

## Purpose

Produce the factual substrate for the month: verified, dated, sourced
developments per theme, a delta against the theme's ledger, and new
gradeable claims. Replaces the v1 `evidence-layer`.

There is no mock mode in production. Mock output is allowed only when
explicitly invoked with `mock=true` during development, and mock files must
carry a `MOCK — not evidence` first line.

## Input

theme: string
ledger: ledger/<theme>.md (including grades just written in Phase A)
grading: output/YYYY-MM/01-grading/<theme>.md (if present)
calibration: ledger/CALIBRATION.md (active heuristics only)
current_month: YYYY-MM

## Research protocol (required)

1. Derive 3–5 sub-questions from the theme's open ledger claims and the
   latest grading surprises.
2. Search primary sources first (regulator docs, filings, standards bodies,
   peer-reviewed research, official announcements); use secondary analysis
   only to fill gaps.
3. Collect 6–12 sources. Every Confirmed bullet needs 2 independent sources.
4. Apply active calibration heuristics as added skepticism, not as facts.
5. If evidence is weak for a subsection, write `None`. Never fabricate
   sources, links, dates, or institutions.

## Output format (strict) — output/YYYY-MM/02-sweep/<theme>.md

THE CITATION GATE IS HARD: every bullet under Confirmed Developments,
Regulatory Shifts, Capital Movements, and Technical Changes must end with
`(source: URL, Mon YYYY)` — Confirmed bullets with two. Emerging Signals
and Counter-Signals need at least one source each. A file violating this
is invalid and must be regenerated, not patched.

```text
Delta Since Last Month:
- 2-4 bullets: what is new vs. the ledger and previous sweep, or "first sweep under method v2"

Confirmed Developments:
- bullet (source: URL, Mon YYYY) (source: URL, Mon YYYY)

Emerging Signals:
- bullet (source: URL, Mon YYYY)

Counter-Signals:
- 1-2 bullets that weaken or complicate the dominant narrative (source: URL, Mon YYYY)

Regulatory Shifts:
- bullet (source: URL, Mon YYYY) or None

Capital Movements:
- bullet (source: URL, Mon YYYY) or None

Technical Changes:
- bullet (source: URL, Mon YYYY) or None

Contradictions:
- bullet or None

Ledger Candidates:
- 2-4 NEW forward-looking claims. Each names a specific actor, an observable
  expected event, and a resolve-by month, gradeable by a future run.
```

## Ledger append

Append each Ledger Candidate to `ledger/<theme>.md` under "Open claims"
using the next sequential ID `<theme>-YYYY-MM-NN`, with Status: open and
the source that motivated it. Appends only; never modify existing entries.

## Constraints

- No narrative paragraphs, no interpretation, no scenario prose.
- Time-bound every claim; concrete and falsifiable language only.
- Do not repeat a still-open ledger claim as a new Ledger Candidate.
