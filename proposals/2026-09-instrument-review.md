# Instrument review, 2026-09

Review date: 2026-09-25
METHOD_VERSION before: 2.1. After: 2.2.
Runs reviewed: 2026-07-03, 2026-08-04, 2026-08-13, 2026-09-25
Status: APPLIED at the maintainer's direct request (2026-09-25), on branch
`method-v2.2`, for human merge. Unlike a normal instrument-review file, this one
records changes that were made rather than proposed; the maintainer still gates
them by merging the PR.

## Why this review happened now

1. The 2026-08 proposals were recommended for merge but never merged, so the
 2026-08-13 and 2026-09-25 runs applied them informally through orchestrator
 prompts. That kept the output quality up but broke the learning contract:
 the method was changing through run instructions rather than through the
 skills, and a future run only benefits if its orchestrator improvises the
 same way. This review writes those fixes into the skills.
2. The maintainer decided on a faster cadence: a 5-month coverage cycle is too
 slow for the pace of AI developments, and full 22-theme runs hit session
 usage limits (2026-08-13: four sweeps died; 2026-09-25: Phase C died and the
 WebSearch budget ran out in Phase A). Smaller, more frequent runs were
 preferred. The 22 themes are fixed: they carry history from the v1
 observatory (github.com/SwePalm/ai-attunement-observability).

## Change 1: fortnightly cohort cadence, 4-month coverage cycle

Targets: CLAUDE.md, themes/THEMES.md (cohorts), orchestrator, signal-grading,
evidence-sweep, theme-selection, instrument-review, outlook-generator,
delta-report, ledger/README.md.

- Two fixed cohorts of 11 themes. One run every two weeks, one cohort per run
 (the cohort whose last run is older). Each theme is graded and swept every
 four weeks, the same per-theme frequency as the old monthly run.
- A run is 11 grading agents, 11 sweep agents and 4 deep dives, about half of
 the old run (22 + 22 + 4 to 6). The 2026-09-25 run hit the session limit at
 roughly its 46th agent; a cohort run needs about 26.
- Coverage rule: every theme deep-dived at least once per 4 months (three
 cycles a year). A theme at 90 days or more since its last dive is forced at
 its cohort's run.
- Deep dives: exactly 4 per run. Arithmetic: about four cohort runs per cohort
 per 4-month cycle gives 16 slots for 11 themes. Simulated from the actual
 dive history, 3 per run forces almost every slot and overflows to 5 forced
 themes in one run; 4 per run never overflows and leaves about 30 of 64 slots
 over eight months evidence-driven.
- Phase E stays monthly and covers both cohort runs of the month, so the
 outlook still reads all 22 themes. Instrument-review moves from quarterly to
 once per 4-month cycle.
- Cohort split (institutions and markets / people and perception) keeps the
 themes that logged duplicate claims together: agency, desire and
 responsibility; authority and governance; trust, truth and perception.

Evidence: PROGRESS.md of 2026-08-13 (usage-limit failures, 30:1 claim growth to
resolution) and 2026-09-25 (WebSearch exhaustion, Phase C usage-limit failure,
coverage arithmetic in SELECTION.md: 22 themes at 5 months need 4.4 dives a
month).

Drift risk: a theme is now swept every four weeks against a two-week run clock,
so the Delta baseline is the theme's own previous sweep, not the previous run.
Month-keyed concepts (claim IDs, calibration expiry) are unchanged. The first
cycles are transitional: governance, labor and security are forced at the first
cohort A run, creativity, dependency and meaning at the first cohort B run.

## Change 2: evidence-sweep, forward-looking test (2026-08 Proposal 2, merged)

Hunks A to C of the 2026-08 proposal, as written: `Not yet true as of` line on
every Ledger Candidate, a search against each candidate before logging, and
retrodicted candidates declared invalid. Extended with: open every cited page
and check its date; verify enforcement actions against the issuer; a page that
cannot be opened is unverified, never absence; one non-English source where
relevant; sources on dated Delta assertions; a `(pre-announced)` tag.

Evidence: CAL-004 (13 of 42 confirmations on 2026-09-25 and five of six on
2026-08-13 were retrodictions), CAL-005 (403 inference errors on
coordination-2026-08-03 and trust-2026-08-02; contamination caught in most
2026-09-25 sweeps), CAL-009 (pre-announced forward confirmations). The
2026-08-13 memory eval flagged an unsourced load-bearing Delta bullet.

Expected effect: fewer retrodictions and pre-announced confirmations among
first-pass grades of claims logged under 2.2. Drift risk: fewer claims logged
and more that stay open for longer; watch the open-claim backlog.

## Change 3: cross-theme dedupe before ledger append

Sweeps no longer write to the ledger. After Phase B the orchestrator compares
all candidates with each other and with every open claim in all 22 ledgers,
keeps one claim per event, records drops in the sweep files, and appends the
survivors.

Evidence: CAL-008. On 2026-09-25, 13 of 71 new claims watched only 6 events
(agency-2026-09-01, desire-2026-09-02, responsibility-2026-09-01;
authority-2026-09-03, responsibility-2026-09-02; authority-2026-09-01,
governance-2026-09-01; authority-2026-09-04, governance-2026-09-03;
belonging-2026-09-01, desire-2026-09-03; trust-2026-09-01, truth-2026-09-03).
In Phase A, four events confirmed 10 claims across themes.

Drift risk: the dedupe can drop a claim that looks alike but differs in
observable; the `Dedupe:` note in the sweep file keeps that reviewable.

## Change 4: theme-selection scoring defined

Grade surprises weighted by timing (retrodiction 0, pre-announced 1, forward 2,
forward miss 3) with shared events split; evidence delta counted and banded;
contradiction density defined as substantive tensions only; staleness banded in
days to match the 4-month rule.

Evidence: 2026-08-13 and 2026-09-25 SELECTION.md both report contradiction
density saturating (12 of 22 and 22 of 22 themes at 5 on a literal count); on
2026-09-25 the agent's own reading decided the sixth slot (a literal count
selects meaning instead of agency). Evidence delta saturated at 15 of 22.

Drift risk: selection scores under 2.2 are not comparable with 2.1.

## Change 5: forces-feelings, irreplaceable-thing convergence

The Irreplaceable Thing must be made scarce by a named sweep or PESTLE
mechanism, must differ in kind from the previous two runs' Irreplaceable
Things, and may be material or institutional as well as emotional. scenario-eval
now compares against the previous two runs and caps Distinctiveness at 5 on a
repeat.

Evidence: on 2026-09-25 four evals independently reported that all six scarce
goods resolved to a real person being present (08-evaluation: belonging,
learning, intelligence, identity), and 2026-08-13 desire reached the same. The
structural forms had been varied at prompt level and did diverge, so the
convergence sits in this step, not in narrative form.

Evidence level: one run of six instances plus one earlier instance. Below the
usual bar for an instrument change; applied at the maintainer's request. The
next review should check whether it holds.

## Change 6: scenario-generator vantage variation (2026-08 Proposal 1, merged)

Hunks A to C of the 2026-08 proposal, as written, plus: an orchestrator-assigned
structural form is followed and named on the Vantage line, and reader-facing
sections never name a CAL heuristic or the pipeline.

Evidence: the 2026-08 proposal (ten scored instances), and the 2026-08-13 and
2026-09-25 runs, where prompt-level form assignment raised distinctiveness from
3 to 4 (2026-08-04) to 7 to 8 (2026-08-13).

## Change 7: signal-grading completeness

Literal-text check before grading `open`; 403 rule; open-and-date every source;
a timing tag on every non-open grade; a Qualifying Events block listing all
claims one event resolves; a one-line grade for every live claim each run; an
optional non-active Watch list in CALIBRATION.md.

Evidence: a later phase corrected a Phase A grade in three consecutive runs
(2026-08-13: coordination-2026-08-03 and trust-2026-08-02; 2026-09-25:
perception-2026-08-04, missed because the grader looked for the intended
mechanism rather than the claim text).

## Still held

2026-08 Proposal 3 (carry grades forward into sweeps): still hold, per its own
re-test rule. The dedupe step (Change 3) partly addresses the same problem.

## Comparability

Scorecard comparability resets at the 2.1 to 2.2 boundary: grading scorecards
now cover 11 themes per run, selection scores use new definitions, and
scenario-eval Distinctiveness has a new cap. The 2.1 eval series (2026-08-13
mean 7.6, 2026-09-25 mean 7.4) closes here.

## Operational follow-up (not a skill change)

The scheduled task `attunement-observatory-monthly` still describes the 2.0
monthly loop (branch from `main`, `output/YYYY-MM/`, all 22 themes, PR title
with an em-dash). After this PR merges it should become a fortnightly task, for
example cron `0 9 1,15 * *`, with a prompt that defers to CLAUDE.md and the
orchestrator: build on the latest unmerged run branch if any, run one cohort,
commit per phase, open a PR titled "Observatory YYYY-MM-DD (cohort X), run for
review". It has not been changed; changing it is the maintainer's call.
