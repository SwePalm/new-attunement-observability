---
name: theme-selection
description: Rank the run's cohort (11 themes) by evidence delta and pick 4 for this run's deep dives, enforcing the 4-month coverage rule. Phase C of the loop.
---

# theme-selection

## Purpose

Concentrate deep-dive effort where the evidence actually moved, while
guaranteeing every theme a deep dive at least once per 4-month cycle.

## Input

grading_reports: output/YYYY-MM-DD/01-grading/*.md (this run's cohort)
sweeps: output/YYYY-MM-DD/02-sweep/*.md (this run's cohort)
history: SELECTION.md files from all previous runs (for deep-dive dates)

## Scoring (per cohort theme)

Score each theme 0–5 on each dimension and sum (max 20). Every score must be
reproducible from the files by another reader.

- **Grade surprises.** Points per claim resolved this run, using the timing
 tags in the grading file: falsified or decayed, forward 3; confirmed,
 forward 2; confirmed, forward, pre-announced 1; any retrodiction 0. When one
 real-world event resolves several claims (the grading file's Qualifying
 Events), that event's points are counted once and split equally across the
 themes it touches. Score = min(5, round(points)).
- **Evidence delta.** Count Confirmed Developments plus Regulatory Shifts whose
 qualifying event is dated after the theme's previous sweep. 0 → 0, 1 → 1,
 2–3 → 2, 4–5 → 3, 6–7 → 4, 8 or more → 5.
- **Contradiction density.** Count bullets in Counter-Signals and
 Contradictions that record a tension in the evidence itself: two named
 actors, instruments or data series pulling in different directions. Do not
 count items marked unverified or caught as contamination, outlets
 disagreeing on a date, count or forum, or notes about the pipeline's own
 grading or claim construction. Score = min(5, max(0, count − 1)).
- **Staleness.** Days from the theme's last deep dive under method v2 to the
 run date (never-dived themes count from 2026-07-03, the first v2 run):
 under 30 → 0, 30–59 → 1, 60–74 → 2, 75–89 → 4, 90 or more → 5.

## Coverage rule

Every theme must be deep-dived at least once per 4 months. A cohort theme
whose staleness is 90 days or more is **forced**: it is selected regardless of
score, because the cohort's next run (about four weeks later) would otherwise
break the rule.

## Selection rule (deterministic)

1. Select all forced themes.
2. Fill to 4 themes by total score. These are the evidence-driven slots;
 at steady state about two per run.
3. Tie-break, in order: higher staleness, higher grade surprises, higher
 evidence delta, alphabetical.
4. Exactly 4, except that forced themes are never dropped: if more than 4
 are forced, select all of them and flag the overflow in SELECTION.md.

Why 4: with one run per cohort every four weeks, a cohort gets about four runs
per 4-month cycle, 16 slots for 11 themes. At 3 per run nearly every slot is
forced and forced themes overflow; at 4 per run, simulated from the 2026-09
dive history, nothing overflows and about 30 of 64 slots per 8 months stay
evidence-driven.

## Output, output/YYYY-MM-DD/SELECTION.md

```text
Cohort: <A or B>

Selected Themes (4):
- <theme>, score N (forced | by score), one-line rationale citing specific sweep or grading items

Not Selected:
- <theme>, score N, one-line reason

Scoring Table:
| theme | surprises | evidence | contradiction | staleness | total |

Coverage Status (all 22 themes):
| theme | cohort | last deep dive | days since | forced at next cohort run? |
```

## Constraints

- Exactly 4 themes (plus forced overflow).
- Rationale must cite actual evidence items (claim IDs, sweep bullets),
 not general impressions.
- Deterministic: the same inputs must produce the same selection.
