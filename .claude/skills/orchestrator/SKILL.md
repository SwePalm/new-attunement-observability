---
name: orchestrator
description: Execute the monthly observatory loop, grade, sweep, select, deep-dive, with PROGRESS.md tracking and resumability. The only entry point for monthly runs.
---

# orchestrator

## Purpose

Execute the monthly loop (Phases A–D). Maintain `output/YYYY-MM-DD/PROGRESS.md`
for resumability. The outlook (Phase E) is NOT part of this loop; it runs
manually after human review of the run's artifacts.

Output folders are keyed to the calendar day the loop runs, not just the
month, so a second run within the same month gets its own folder and
compounds on the first via the ledger, instead of overwriting it.

## Workflow

1. Determine today's run date `YYYY-MM-DD`. Create:

 ```text
 output/YYYY-MM-DD/
 01-grading/
 02-sweep/
 03-structural-question/
 04-exploration/
 05-pestle/
 06-forces-feelings/
 07-scenario/
 08-evaluation/
 ```

2. Initialize or resume `output/YYYY-MM-DD/PROGRESS.md`:
 - Header: METHOD_VERSION (from CLAUDE.md) and current git SHA.
 - Phase A checklist: all 22 themes.
 - Phase B checklist: all 22 themes.
 - Phase C: pending/done.
 - Phase D checklist: filled in after selection, selected themes only.
 - States: `[ ]` pending, `[/]` in progress, `[x]` done, `[!]` blocked.

3. **Phase A, signal-grading**, per theme:
 - Themes whose ledger has no open claims: mark `[x]` with note
 "no open claims".
 - Grading requires web research; run each theme as a research subagent
 where possible.

4. **Phase A wrap-up**: after all themes are graded, run the calibration
 pass of `signal-grading` once, updating `ledger/CALIBRATION.md` within
 its hard bounds.

5. **Phase B, evidence-sweep** for all 22 themes.
 Enforce the citation gate on each file before accepting it. On failure,
 regenerate (max 2 retries), then mark `[!]` blocked and continue.

6. **Phase C, theme-selection.** Write `SELECTION.md`; append the selected
 themes to the Phase D checklist in PROGRESS.md.

7. **Phase D, deep dive**, for each selected theme, strictly in order:
 structural-question → theme-exploration → pestle-analysis →
 forces-feelings → scenario-generator → scenario-eval.
 Each step's output file must exist before the next step starts.

8. Done when every checklist item is `[x]` or `[!]`. Report all `[!]` items
 and the Phase A scorecard summary to the human, and remind them that
 `outlook-generator` awaits their review trigger.

## Constraints

- Steps within a theme are sequential; different themes may run in parallel
 subagents within the same phase.
- Never edit skill files or CALIBRATION bounds (see CLAUDE.md learning contract).
- Overwrite same-day step files if this exact date's run is resumed; never
 touch a previous run's folder (any other `YYYY-MM-DD/`), even one from
 earlier in the same month.
- Ledger changes are appends only.
- File names: lowercase theme name, spaces replaced with hyphens.
