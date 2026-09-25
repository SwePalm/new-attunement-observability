---
name: orchestrator
description: Execute one fortnightly cohort run of the observatory loop, grade, sweep, dedupe, select, deep-dive, with PROGRESS.md tracking and resumability. The only entry point for runs.
---

# orchestrator

## Purpose

Execute one run (Phases A–D) for one cohort of 11 themes. Maintain
`output/YYYY-MM-DD/PROGRESS.md` for resumability. The outlook (Phase E) is NOT
part of this loop; it runs monthly and manually after human review, covering
both cohort runs of the month.

Output folders are keyed to the calendar day the run happens, so every run
gets its own folder and compounds on earlier runs via the ledger.

## Workflow

0. **Base and cohort.**
 - Ledger continuity: if the previous run's branch has not been merged, build
 this run on top of it rather than on `main`, otherwise the append-only
 ledger forks. Record the base in PROGRESS.md.
 - Cohort: read `themes/THEMES.md` (Cohorts) and the most recent run folders.
 This run takes the cohort whose most recent run is older; if neither
 cohort has run under METHOD_VERSION 2.2, take cohort A. Record the cohort
 and the reason in PROGRESS.md.

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
 - Header: METHOD_VERSION (from CLAUDE.md), current git SHA, base branch,
 cohort, previous run of this cohort.
 - Phase A checklist: the cohort's 11 themes.
 - Phase B checklist: the cohort's 11 themes, plus "dedupe and ledger append".
 - Phase C: pending/done.
 - Phase D checklist: filled in after selection, selected themes only.
 - States: `[ ]` pending, `[/]` in progress, `[x]` done, `[!]` blocked.

3. **Phase A, signal-grading**, per cohort theme:
 - Themes whose ledger has no live claims: mark `[x]` with note
 "no open claims".
 - Grading requires web research; run each theme as a research subagent.

4. **Phase A wrap-up**: after all cohort themes are graded, run the
 calibration pass of `signal-grading` once, updating `ledger/CALIBRATION.md`
 within its hard bounds.

5. **Phase B, evidence-sweep** for the cohort's 11 themes.
 Enforce the citation gate on each file before accepting it, mechanically
 (a script that counts dated source blocks per bullet), not by eye. On
 failure, regenerate (max 2 retries), then mark `[!]` blocked and continue.
 Sweeps write Ledger Candidates into their sweep file only; they do not
 touch the ledger.

6. **Phase B wrap-up, dedupe and ledger append** (orchestrator, once):
 - Collect every Ledger Candidate from this run's sweeps.
 - Compare them with each other and with every open claim in all 22 ledger
 files (both cohorts). Two claims are duplicates when the same actor's same
 observable event would resolve both.
 - For each duplicate group keep one candidate, in the theme whose open
 claims are closest to the event; drop the others. Drop any candidate that
 duplicates an existing open claim. Append a `Dedupe:` line to each
 affected sweep file naming what was dropped and why.
 - Append the surviving candidates to their theme ledgers under "Open
 claims" with the next unused `<theme>-YYYY-MM-NN` IDs, in the ledger
 README format. Appends only.
 - Record in PROGRESS.md: candidates proposed, dropped as duplicates,
 appended.

7. **Phase C, theme-selection** over this run's cohort. Write `SELECTION.md`;
 append the selected themes (4, plus any coverage overflow) to the Phase D
 checklist in PROGRESS.md.

8. **Phase D, deep dive**, for each selected theme, strictly in order:
 structural-question → theme-exploration → pestle-analysis →
 forces-feelings → scenario-generator → scenario-eval.
 Each step's output file must exist before the next step starts.

9. Done when every checklist item is `[x]` or `[!]`. Report all `[!]` items
 and the Phase A scorecard summary to the human. If this is the month's
 second cohort run, remind them that `outlook-generator` and `delta-report`
 await their review trigger for the month.

## Execution guidance

- Run subagents in waves of at most 11 (one cohort phase at a time). A cohort
 run is sized to fit inside one session's usage window; do not start Phase D
 before Phase B's ledger append is committed, so a usage-limit stop leaves a
 clean resume point.
- Commit after each phase. Subagents never run git commands, not even
 read-only ones.
- Give research subagents the fallback below in their instructions. The
 session-wide WebSearch budget can run out mid-run and Brave Search
 rate-limits. Subagents cannot run script files from a scratchpad (the
 permission classifier blocks them), but an inline one-liner works. For
 discovery only; every cited page must still be opened and its date checked:

 ```text
 python3 -c 'import sys,urllib.parse as P,urllib.request as R,xml.etree.ElementTree as E;u="https://www.bing.com/news/search?"+P.urlencode({"q":sys.argv[1],"format":"rss","setlang":"en-us","cc":"us"});r=E.fromstring(R.urlopen(R.Request(u,headers={"User-Agent":"Mozilla/5.0"}),timeout=25).read());[print(i.findtext("pubDate"),"|",i.findtext("title"),"|",P.parse_qs(P.urlparse(i.findtext("link")).query).get("url",[i.findtext("link")])[0]) for i in list(r.iter("item"))[:12]]' "query"
 ```

- Verify every ledger diff before committing: every deleted line must be a
 `Status:` update or part of a claim block moved intact to "Resolved claims".

## Constraints

- Steps within a theme are sequential; different themes may run in parallel
 subagents within the same phase.
- Never edit skill files or CALIBRATION bounds (see CLAUDE.md learning contract).
- Overwrite same-day step files if this exact date's run is resumed; never
 touch a previous run's folder (any other `YYYY-MM-DD/`), even one from
 earlier in the same month.
- Ledger changes are appends only.
- File names: lowercase theme name, spaces replaced with hyphens.
