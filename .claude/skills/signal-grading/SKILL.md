---
name: signal-grading
description: Grade open ledger claims against reality using web research, append grades, and maintain the bounded calibration memo. Phase A of the monthly loop.
---

# signal-grading

## Purpose

Make the observatory accountable to its own past claims. For one theme:
research each open ledger claim and grade it. After all themes: distill
recurring error patterns into calibration heuristics.

This step is what turns deep research into re-search. It runs before any
new evidence is gathered, so the month starts from a scored baseline.

## Input

theme: string
ledger: ledger/<theme>.md
current_month: YYYY-MM

## Grading protocol (per open claim)

1. Research the claim's current status. Prioritize primary sources
   (regulator docs, filings, standards bodies, official announcements,
   peer-reviewed work).
2. Assign exactly one grade:
   - `confirmed` — happened materially as stated (source required)
   - `decayed` — trend weakened, stalled, or was overtaken (source required)
   - `falsified` — contradicted by events (source required)
   - `open` — no resolution yet AND resolve-by month not passed (no source needed)
   - `expired` — resolve-by passed with no determinable outcome. Treat as a
     calibration signal: the claim was probably not written falsifiably enough.
3. Append to the claim's Grades list:
   `- YYYY-MM: <grade> — <one sentence> (source: URL, Mon YYYY)`
4. Move claims graded confirmed/decayed/falsified/expired from "Open claims"
   to "Resolved claims". Never rewrite claim text or earlier grades.

## Output — output/YYYY-MM/01-grading/<theme>.md

```text
Scorecard:
- open: N, confirmed: N, decayed: N, falsified: N, expired: N

Grade Details:
- <claim-id>: <grade> — <one-sentence justification> (source: URL, Mon YYYY)

Surprises:
- 1-3 bullets: grades that deviated most from the claim's implied confidence, or None
```

## Calibration pass (once, after ALL themes are graded)

Update `ledger/CALIBRATION.md`:

1. Look for recurring error patterns across this month's grades
   (e.g. "regulatory timelines systematically overestimated",
   "vendor capability announcements decay at high rates").
2. A new heuristic requires >= 2 graded claim IDs as evidence.
3. Re-confirm an existing heuristic only when new grades support it;
   extend its expiry by 3 months.
4. Retire expired or contradicted heuristics (move to Retired, with reason).
5. Respect hard bounds: max 10 active heuristics; every heuristic cites
   claim IDs; every heuristic has an expiry. If the memo is full, a new
   heuristic must displace the weakest-evidenced one or wait.

Heuristics must be falsifiable statements about THIS PIPELINE'S bias —
not general world commentary, not style advice.

## Constraints

- A grade other than `open` without a source is invalid.
- Do not add new claims here (that is evidence-sweep's job).
- Do not edit skills. Calibration is context, not code.
- If a theme's ledger has no open claims, skip it and report "no open claims".
