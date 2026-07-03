# Attunement Monthly Observatory

METHOD_VERSION: 2.0

Entry skill for monthly runs: `orchestrator` (`.claude/skills/orchestrator/`).
Manual skills: `outlook-generator` (after human review), `instrument-review` (quarterly).

## Mission

Run a monthly foresight loop across 22 Human–AI themes that compounds:
every run grades the previous runs' claims before making new ones.
Deep research is used as re-search — re-interrogating a standing set of
falsifiable claims — not as one-off search.

## The learning contract (three layers, three speeds)

Learning happens at three layers. Each has a different change speed and gate.

1. **State** — `ledger/<theme>.md`
   Changes every run, automatically. Claims are appended, grades are appended.
   Never rewrite or delete past claims or grades.

2. **Calibration** — `ledger/CALIBRATION.md`
   Bounded memo of the pipeline's own observed biases.
   Written ONLY by `signal-grading`. Read by `evidence-sweep`,
   `scenario-generator`, and `scenario-eval` as context.
   Hard bounds: max 10 active heuristics; each must cite >= 2 graded claim IDs;
   each expires after 3 months unless re-confirmed by new grades.
   Calibration NEVER modifies skills.

3. **Instrument** — `.claude/skills/`
   Frozen between versions. Only `instrument-review` (quarterly, manually
   invoked) may propose changes, as diffs written to `proposals/`. A human
   merges and bumps METHOD_VERSION. Agents must never edit skill files
   during a monthly run.

## Global invariants (every skill, every run)

- **Citation gate**: any bullet labeled Confirmed must carry at least one
  source URL and a month+year. No URL + date means the file is invalid and
  must be regenerated, not patched.
- **Falsifiability**: ledger claims must name actor, observable event, and
  resolve-by month specifically enough that a future run can grade them
  confirmed, decayed, or falsified.
- **Append-only history**: ledgers record; they do not rewrite.
- **Version stamping**: every `output/YYYY-MM/PROGRESS.md` records
  METHOD_VERSION and the current git SHA. Scorecards are comparable only
  within a method version.

## Monthly loop

| Phase | Skill | Scope | Output |
|-------|-------|-------|--------|
| A | signal-grading | themes with open claims | `output/YYYY-MM/01-grading/` + ledger grades |
| B | evidence-sweep | all 22 themes | `output/YYYY-MM/02-sweep/` + new ledger claims |
| C | theme-selection | corpus | `output/YYYY-MM/SELECTION.md` |
| D | structural-question, theme-exploration, pestle-analysis, forces-feelings, scenario-generator, scenario-eval | selected 4–6 themes only | `output/YYYY-MM/03-...` to `08-evaluation/` |
| E | outlook-generator | manual, after human review | `output/YYYY-MM/09-outlook/` |

## Folder strategy

```text
output/YYYY-MM/
  01-grading/            one file per theme with open claims
  02-sweep/              one file per theme (22)
  SELECTION.md           selected themes + rationale + coverage table
  03-structural-question/
  04-exploration/
  05-pestle/             selected themes only
  06-forces-feelings/
  07-scenario/
  08-evaluation/
  09-outlook/
  PROGRESS.md
ledger/                  persistent, append-only, cross-month
proposals/               instrument-review output, human-merged
```

Note: the 2026-02 output predates this method (v1) and keeps its original
step-first layout. Its horizon claims were seeded into the ledger, marked
as ungrounded.

## Themes

`themes/THEMES.md` (22 themes). Coverage rule: every theme is deep-dived at
least once per 5 months, enforced by `theme-selection`.
