# Run progress, 2026-08-04

METHOD_VERSION: 2.1
Git SHA: e355d24b66812101c899ff336a3cb099dda7e6e3
Run date: 2026-08-04
Previous run: 2026-07-03

States: `[ ]` pending, `[/]` in progress, `[x]` done, `[!]` blocked

## Phase A, signal-grading (22 themes)

Complete. 110 open claims graded: 88 open, 17 confirmed, 5 decayed, 0 falsified, 0 expired.
Calibration pass added CAL-004 (retrodiction bias) and extended CAL-001/002/003 to 2027-01.

- [x] agency
- [x] alignment
- [x] authority
- [x] autonomy
- [x] belonging
- [x] coordination
- [x] creativity
- [x] dependency
- [x] desire
- [x] governance
- [x] identity
- [x] intelligence
- [x] labor
- [x] learning
- [x] meaning
- [x] memory
- [x] perception
- [x] power
- [x] responsibility
- [x] security
- [x] trust
- [x] truth
- [x] calibration pass (once, after all themes)

## Phase B, evidence-sweep (22 themes)

Complete. All 22 sweeps pass the citation gate (verified mechanically: two distinct
sources on every Confirmed Development bullet, one on every other cited section).
95 new falsifiable claims appended to the ledger; 183 claims now open.

autonomy and creativity were regenerated once after a first-pass gate failure. The
first pass had already appended 4 claims to each ledger. Under the append-only
invariant those claims were retained and recorded in the regenerated sweep files,
so autonomy and creativity carry 7 and 8 new claims respectively rather than 4.

45 ledger Source lines were written without the required month and year. All were
backfilled from the date the same URL carries in its own sweep file, or from the
date embedded in the URL path. No dates were inferred or invented.


- [x] agency
- [x] alignment
- [x] authority
- [x] autonomy
- [x] belonging
- [x] coordination
- [x] creativity
- [x] dependency
- [x] desire
- [x] governance
- [x] identity
- [x] intelligence
- [x] labor
- [x] learning
- [x] meaning
- [x] memory
- [x] perception
- [x] power
- [x] responsibility
- [x] security
- [x] trust
- [x] truth

## Phase C, theme-selection

- [x] SELECTION.md

Selected (all five from the never-dived backlog): responsibility 19, alignment 18,
authority 18, coordination 18, trust 18. Cut was mechanical at score >= 18.
Staleness did the work it was designed to do: the four largest evidence deltas in
the corpus (agency 15, security 14, creativity 13, labor 13) all belong to themes
dived in 2026-07 and none reached the cut. First alternate: autonomy 17.

## Phase D, deep dives (selected themes)

- [x] responsibility, six steps
- [x] alignment, six steps
- [x] authority, six steps
- [x] coordination, six steps
- [x] trust, six steps

All 30 step files written. Ledger untouched by Phase D, as required.

Scenario eval scores: alignment 7.3, responsibility 6.8 (repaired, was 5.8),
authority 6.4, trust 6.3, coordination 6.2. Mean 6.6, against the 2026-07-03
run's 8.1-8.5 band. All five citation gates pass.

responsibility was rebuilt from the sweep down on 2026-08-04. The original Phase B
pass dropped the confirmed private-right-of-action evidence from
responsibility-2026-07-02, and the whole deep-dive chain inherited a false thesis.
The rebuild engages that evidence and works the real tension instead: individual
remedy exists in a narrow companion-chatbot lane while the frontier-audit regimes
route around it. Oregon is the only one of 14 state companion-chatbot laws enacted
in 2026 whose text lets a harmed user sue for damages. Ledger unchanged; the theme
keeps its four original claims.

The rebuild also served as a controlled test of the template finding: same theme,
same skill, instructed only to abandon the house form, Distinctiveness moved 3 to 7.
That isolates the cause to prompt-level form rather than to the theme.

## Blocked items

None. Every checklist item is [x].

## Flag for human review

The eval agents independently converged on the same finding, and it is a method
problem rather than a content problem. Distinctiveness vs. Other Themes scored
3 or 4 out of 10 in every one of the five evaluations. All five scenarios open on
a named mid-senior professional at a headcount-specified organisation on a named
weekday in 2029, place a European entity in the corporate structure, use the
2 Aug 2026 EU commencement as a structural force, and close on the same rhetorical
move: reasonable actors, structural outcome, one scarce good named at the end.
The themes' objects are genuinely distinct. The voice and architecture are not.

Two further items for review:

- responsibility, 5.8, omits this run's own confirmed grading evidence
  (Washington HB 2225 private right of action, Oregon SB 1546 statutory damages)
  which contradicts its central thesis that nothing routes remedy to the harmed
  individual. This is the most serious single defect in the run.
- Several scenarios name CAL-002 and CAL-003 in reader-facing prose and, in at
  least two cases, invoke a heuristic as though it were evidence rather than an
  attentional correction.

## Phase E, complete

- [x] 09-outlook/outlook-debug.md, debug draft
- [x] 09-outlook/outlook.md, production essay, 3,767 words
- [x] 09-outlook/delta-report.md, accountability companion, 3,319 words
- [x] LEARNINGS.md, method findings for skill development
- [x] proposals/2026-08-instrument-review.md, three proposals, merge some

The debug draft was reviewed adversarially before production. The review caught two
factual errors: the ten-day figure conflated OpenAI's ignorance window with the
detection window (Hugging Face detected the agents in about 4.5 days), and a claim
that both labs disclosed voluntarily when OpenAI's disclosure followed its victim's.
Both fixed in production.

The delta report rejected the open-claim count it was briefed with (184) and
established 183 by reconciling two independent counts. 184 came from a format
example line in ledger/README.md. 183 is correct.

Run complete. METHOD_VERSION remains 2.1; no skill file was edited at any point.
