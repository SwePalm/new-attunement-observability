---
name: signal-grading
description: Grade open ledger claims against reality using web research, append grades, and maintain the bounded calibration memo. Phase A of the loop, run for the run's cohort (11 themes).
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
current_run_date: YYYY-MM-DD

## Scope

Grade every live claim in the theme's ledger under "Open claims" (claims
logged under method v2). Retired method-v1 seed claims (`<theme>-2026-02-NN`)
are not graded and not counted. Each live claim gets exactly one grade line
per run, including `open` ones (one sentence on what was checked).

## Grading protocol (per open claim)

1. Research the claim's current status. Prioritize primary sources
 (regulator docs, filings, standards bodies, official announcements,
 peer-reviewed work). Open every page you cite and check its date; never
 grade from a search-result title.
2. Literal-text check: before grading `open`, ask whether any event, through
 any mechanism or actor, satisfies the claim's words as written, not only
 the mechanism the claim had in mind. Search the claim's observable, not just
 its intended channel.
3. Unreachable primary source: a page that returns HTTP 403, a paywall or a
 timeout is not evidence the event did not happen. Check reputable secondary
 coverage and non-English primary sources; if still unverifiable, grade
 `open` and name the page that could not be opened.
4. Assign exactly one grade:
 - `confirmed`, happened materially as stated (source required)
 - `decayed`, trend weakened, stalled, or was overtaken (source required)
 - `falsified`, contradicted by events (source required)
 - `open`, no resolution yet AND resolve-by month not passed (no source needed)
 - `expired`, resolve-by passed with no determinable outcome. Treat as a
 calibration signal: the claim was probably not written falsifiably enough.
5. Append to the claim's Grades list:
 `- YYYY-MM-DD: <grade>, <one sentence> (source: URL, Mon YYYY)`
6. Tag every non-open grade in the grading file with its timing against the
 claim's logging date: `retrodiction` (qualifying event dated before logging),
 `forward, pre-announced` (after logging, but the actor had already announced
 or scheduled it), or `forward`.
7. Move claims graded confirmed/decayed/falsified/expired from "Open claims"
 to "Resolved claims". Never rewrite claim text or earlier grades.

## Output, output/YYYY-MM-DD/01-grading/<theme>.md

```text
Scorecard:
- open: N, confirmed: N, decayed: N, falsified: N, expired: N

Grade Details:
- <claim-id>: <grade>, <timing tag>, <one-sentence justification> (source: URL, Mon YYYY)

Qualifying Events:
- one line per real-world event that resolved a claim this run, listing every
 claim ID (in any theme you know of) that it resolves, so one event is not
 read as several independent confirmations

Surprises:
- 1-3 bullets: grades that deviated most from the claim's implied confidence, or None
```

## Calibration pass (once, after ALL themes are graded)

Update `ledger/CALIBRATION.md`:

1. Look for recurring error patterns across this run's grades
 (e.g. "regulatory timelines systematically overestimated",
 "vendor capability announcements decay at high rates").
2. A new heuristic requires >= 2 graded claim IDs as evidence.
3. Re-confirm an existing heuristic only when new grades support it;
 extend its expiry by 3 months.
4. Retire expired or contradicted heuristics (move to Retired, with reason).
5. Respect hard bounds: max 10 active heuristics; every heuristic cites
 claim IDs; every heuristic has an expiry. If the memo is full, a new
 heuristic must displace the weakest-evidenced one or wait.
6. Patterns below the evidence bar may be kept under a `Watch list (below the
 evidence bar, not active)` heading, each citing the claim IDs seen so far.
 Watch-list items are never read as heuristics by other skills.

Heuristics must be falsifiable statements about THIS PIPELINE'S bias, 
not general world commentary, not style advice.

## Constraints

- A grade other than `open` without a source is invalid.
- Do not add new claims here (that is evidence-sweep's job).
- Do not edit skills. Calibration is context, not code.
- If a theme's ledger has no open claims, skip it and report "no open claims".
