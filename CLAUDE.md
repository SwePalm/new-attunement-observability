# Attunement Monthly Observatory

METHOD_VERSION: 2.2

Entry skill for every run: `orchestrator` (`.claude/skills/orchestrator/`).
Manual skills: `delta-report` (monthly), `outlook-generator` (once per 4-month
cycle, drafted on a schedule, published after human review),
`instrument-review` (once per 4-month cycle).

## Mission

Run a fortnightly foresight loop across 22 Human–AI themes that compounds:
every run grades the previous runs' claims before making new ones. The 22
themes are split into two fixed cohorts of 11 (`themes/THEMES.md`); each run
covers one cohort, so every theme is graded and swept every four weeks and
deep-dived at least once per 4-month cycle (three cycles a year).
Deep research is used as re-search, re-interrogating a standing set of
falsifiable claims, not as one-off search.

## The learning contract (three layers, three speeds)

Learning happens at three layers. Each has a different change speed and gate.

1. **State**, `ledger/<theme>.md`
 Changes every run, automatically. Claims are appended, grades are appended.
 Never rewrite or delete past claims or grades.

2. **Calibration**, `ledger/CALIBRATION.md`
 Bounded memo of the pipeline's own observed biases.
 Written ONLY by `signal-grading`. Read by `evidence-sweep`,
 `scenario-generator`, and `scenario-eval` as context.
 Hard bounds: max 10 active heuristics; each must cite >= 2 graded claim IDs;
 each expires after 3 months unless re-confirmed by new grades.
 Calibration NEVER modifies skills.

3. **Instrument**, `.claude/skills/`
 Frozen between versions. Only `instrument-review` (once per 4-month
 cycle, manually invoked) may propose changes, as diffs written to `proposals/`. A human
 merges and bumps METHOD_VERSION. Agents must never edit skill files
 during a run.

## Global invariants (every skill, every run)

- **Citation gate**: any bullet labeled Confirmed must carry at least one
 source URL and a month+year. No URL + date means the file is invalid and
 must be regenerated, not patched.
- **Falsifiability**: ledger claims must name actor, observable event, and
 resolve-by month specifically enough that a future run can grade them
 confirmed, decayed, or falsified.
- **Append-only history**: ledgers record; they do not rewrite.
- **Version stamping**: every `output/YYYY-MM-DD/PROGRESS.md` records
 METHOD_VERSION and the current git SHA. Scorecards are comparable only
 within a method version.
- **No em-dashes**: no artifact may contain the em-dash character. Use commas,
 periods, colons, or parentheses. En-dashes in numeric ranges are fine.

## Two reader-facing outputs (Phase E)

Two distinct documents, on different clocks, and they must stay distinct:

- **The Outlook** (`outlook-generator`): a forward-looking narrative essay,
 once per 4-month cycle, when all 22 themes have a fresh deep dive behind it.
 Storytelling, human-centered, no self-audit. This is the published piece.
 Cycles: Oct–Jan, Feb–May, Jun–Sep. Draft on the 25th of the cycle's last
 month, in `output/cycle-YYYY-MM/`.
- **The Delta Report** (`delta-report`): monthly, the accountability
 companion, so scoring keeps pace with the fortnightly runs. How
 past claims graded, what shifted, which claims are on the clock, what the
 pipeline learned. This is where the numbers live.

Keeping the audit out of the essay was a deliberate 2026-07 decision: the
scorecard was destroying the outlook's readability. Do not merge them back.

## Fortnightly loop

One run every two weeks, one cohort per run (the cohort whose last run is
older). A run is about half the work of the old monthly run, which keeps it
inside a single session's usage window.

| Phase | Skill | Scope | Output |
|-------|-------|-------|--------|
| A | signal-grading | this run's cohort (11 themes) | `output/YYYY-MM-DD/01-grading/` + ledger grades |
| B | evidence-sweep, then orchestrator dedupe and ledger append | this run's cohort (11 themes) | `output/YYYY-MM-DD/02-sweep/` + new ledger claims |
| C | theme-selection | this run's cohort | `output/YYYY-MM-DD/SELECTION.md` |
| D | structural-question, theme-exploration, pestle-analysis, forces-feelings, scenario-generator, scenario-eval | selected 4 themes | `output/YYYY-MM-DD/03-...` to `08-evaluation/` |
| E | delta-report (monthly) and outlook-generator (per cycle) | manual publication after human review | delta: `output/YYYY-MM-DD/09-outlook/delta-report.md` in the month's last run folder; outlook: `output/cycle-YYYY-MM/` |

## Folder strategy

```text
output/YYYY-MM-DD/
 01-grading/ one file per cohort theme (11)
 02-sweep/ one file per cohort theme (11)
 SELECTION.md selected themes + rationale + coverage table
 03-structural-question/ selected themes only (4)
 04-exploration/
 05-pestle/ selected themes only
 06-forces-feelings/
 07-scenario/
 08-evaluation/
 09-outlook/
 PROGRESS.md
ledger/ persistent, append-only, cross-month
output/cycle-YYYY-MM/ the cycle Outlook (debug draft, then production)
proposals/ instrument-review output, human-merged
```

Each invocation of the loop gets its own folder keyed to the calendar day it
runs (`YYYY-MM-DD`), not just the month. This is what lets the loop compound:
running it twice in the same month produces two folders instead of one run
overwriting the other, while the ledger and CALIBRATION.md still accumulate
across both. Month-level concepts (the coverage rule, calibration expiry,
ledger claim IDs `<theme>-YYYY-MM-NN`) are unaffected: a claim ID's month
segment still groups by calendar month even if several runs land in it.

Note: the 2026-02 output predates this method (v1) and keeps its original
step-first layout. Its horizon claims were seeded into the ledger, graded once
in the 2026-07 run to mark the "before" picture, and then RETIRED. The v1
boilerplate is not graded again; from 2026-08 the delta report grades only
claims logged under this method. The 2026-02 output stays as archived history.

Note: the first method-v2 run's output lived at `output/2026-07/` before the
per-day folder change (METHOD_VERSION 2.1); it was renamed to
`output/2026-07-03/` to match, since that is the calendar day it actually ran.

## Themes

`themes/THEMES.md` (22 themes in two cohorts of 11). Coverage rule: every
theme is deep-dived at least once per 4-month cycle, enforced by
`theme-selection`. The 22 themes are fixed and carry history from the v1
observatory (github.com/SwePalm/ai-attunement-observability); do not merge,
split or rename them.

Note: METHOD_VERSION 2.2 (2026-09) replaced the monthly all-22 run with the
fortnightly cohort run and tightened the coverage rule from 5 months to 4.
Scorecards, eval scores and selection scores from 2.1 and earlier are not
comparable with 2.2. See `proposals/2026-09-instrument-review.md`.
