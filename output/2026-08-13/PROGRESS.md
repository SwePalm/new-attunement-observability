# Run progress, 2026-08-13

METHOD_VERSION: 2.1
Git SHA: 1e556ec88cb8d78b6d257cb3eb62410eaf4f8a9a
Run date: 2026-08-13
Previous run: 2026-08-04 (9 days earlier)

States: `[ ]` pending, `[/]` in progress, `[x]` done, `[!]` blocked

Run note: this is the second run inside calendar month 2026-08. The previous run
closed on 2026-08-04 and graded every open claim then. Per the run instruction,
Phase A this run grades only claims whose resolve-by month has arrived or whose
status is meaningfully updatable by evidence dated after 2026-08-04. Claims with
no material movement in the intervening nine days are reported as unchanged in
the grading file and receive no new ledger grade line, so the ledger is not
padded with 183 no-change entries. The 2026-02 method-v1 seed claims are retired
and are not re-graded.

## Phase A, signal-grading (22 themes)

Complete. All 22 themes researched. 136 live method-v2 claims open, 4 confirmed,
1 decayed, 0 falsified, 0 expired. 42 retired method-v1 seed claims are still
parked under "Open claims" in the ledgers and were not graded; they are excluded
from every count above.

Confirmed: agency-2026-08-04 (EC officials confirmed on 31 Jul 2026 that OpenAI
and Anthropic had both briefed the Commission bilaterally on their agent
containment incidents), desire-2026-07-02 (France's Autorite de la concurrence
published an own-initiative sector inquiry into AI agents on 17 Jul 2026),
desire-2026-08-01 (the AI AGENT Act was introduced as S.5051 on 21 Jul 2026),
memory-2026-08-01 (Microsoft ships a documented confirm-before-memory-write
control). Decayed: autonomy-2026-08-06 (Article 73 serious-incident guidance is
still the Sep 2025 consultation draft and its 2 Aug 2026 date has passed).

Three of the four confirmations are retrodictions: the qualifying event predated
the claim's own logging date. This is the run's central finding and drove the
calibration pass.

Scorecard normalisation: desire, intelligence and responsibility originally
counted retired v1 seeds inside their open totals. Their scorecards were
corrected to the convention used by the other 19 themes. No grade line, claim
text or ledger entry was altered by that correction.

Calibration pass: CAL-002, CAL-003 and CAL-004 re-confirmed and extended.
CAL-005 (retrieval coverage bias and source contamination), CAL-006 (claims
named on the slowest actor), CAL-007 (claim clock slower than run clock) added.
Seven active heuristics, inside the bound of 10.

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

Complete. All 22 sweeps written and validated against the citation gate
mechanically, not by eye: two independent sources on every Confirmed Development
bullet, one on every other cited bullet. 78 new falsifiable claims appended.
213 live claims now open, plus 42 retired v1 seeds still parked in the ledgers.

meaning, responsibility, trust and truth failed on the first pass when the
session hit a usage limit. They wrote nothing at all, so no partial state needed
cleaning up, and all four were rerun to completion after the limit reset.

Sweeps wrote `None` freely where nine days produced nothing. That is the correct
outcome for this interval and was instructed rather than tolerated.

Two Phase A grades were corrected during this phase, both in the same direction
and both found by sweeps checking a primary registry the grading pass had only
inferred:

- coordination-2026-08-03, open to confirmed. S.5051 was introduced 21 Jul 2026.
  The grading pass read accurate press language as loose wording about the
  discussion draft, because congress.gov returns 403 to automated fetching.
- trust-2026-08-02, open to confirmed. OpenAI published its technical account on
  openai.com on 21 Jul 2026 and a follow-up on 4 Aug 2026. The grading pass
  inferred the absence rather than checking it, because openai.com also returns
  403.

Both corrected claims were satisfied before their own logging date, so the run's
retrodiction count rises from three of four confirmations to five of six.

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

Selected, all five from the never-dived backlog, cut mechanical at score >= 18:
autonomy 18, desire 18, memory 18, power 18, truth 18. First alternate: meaning 17.

Staleness was held at the nine-day interval rather than recomputed as a month, so
the five themes dived on 2026-08-04 (responsibility, alignment, authority,
coordination, trust) scored 0 or 1 and none reached the cut. No theme has reached
month 5, so the coverage rule forced no selection. This run consumes one of the
remaining rounds before the 2026-12 coverage deadline; seven never-dived themes
now remain for four rounds.

Selection flagged that contradiction density did almost no discriminating work,
because 12 of 22 themes scored 5 on it: every sweep carries two counter-signals
and three or four contradictions by template. Separation came from staleness and
evidence delta alone. That is an instrument-review item, not a content problem.

## Phase D, deep dives (selected themes)

- [x] autonomy, six steps
- [x] desire, six steps
- [x] memory, six steps
- [x] power, six steps
- [x] truth, six steps

All 30 step files written. Ledger untouched by Phase D, as required.

Scenario eval scores: autonomy 7.8, memory 7.8, power 7.7, desire 7.4, truth 7.2.
Mean 7.6, against the 2026-08-04 run's 6.6 (band 6.2 to 7.3). All five citation
gates pass, three of them with defects recorded rather than concealed.

The template regression flagged for human review on 2026-08-04 is repaired.
Distinctiveness scored 8, 8, 7, 7, 7 this run against 3, 3, 3, 4, 7 last run.
Each theme was assigned a distinct structural form at the prompt level:
institutional artifacts (autonomy), the demand side of a market (desire), one
record revisited across four years (memory), the grid's own timescales (power),
one artifact's chain of custody (truth). None opens on a professional at a desk,
none defaults to 2029, none makes the 2 Aug 2026 EU commencement load-bearing,
and none closes on a named scarce good. This confirms the 2026-08-04 finding
that the cause was prompt-level form rather than the themes or the model.

No scenario names a calibration heuristic in reader-facing prose, which was the
second review item from last run.

## Blocked items

None. Every checklist item is [x].

Four Phase B sweeps (meaning, responsibility, trust, truth) died mid-run on a
session usage limit. They wrote nothing, so no partial state needed repair, and
all four were rerun to completion after the limit reset.

## Flag for human review

1. The retrodiction problem is worse than the 2026-08-04 run measured, and it is
   now the run's central finding. Five of six confirmations were satisfied by
   evidence predating the claim's own logging date. Two of those five were found
   only because a later phase re-checked a grade the grading pass had inferred
   rather than verified. The pipeline is currently better at retrieving what has
   already happened than at naming what will happen next.

2. A specific, fixable mechanism produced both grading errors. Several
   authoritative registries (congress.gov, openai.com, ftc.gov, nature.com,
   courtlistener, cde.ca.gov) return HTTP 403 to automated fetching. In both
   cases a grader converted "I could not reach the registry" into "the event did
   not occur", then reasoned past accurate secondary coverage to defend the
   negative. Recorded as a fourth failure mode under CAL-005. This wants an
   instrument-level fix, not a prompt-level one.

3. Source contamination is now an active hazard rather than a theoretical one.
   Sweeps caught fabricated but citable-looking regulatory actions in seven
   themes, including a claimed EUR 47M in Article 50 penalties appearing on no
   Commission page, a CNIL action against 14 financial institutions, and a CAC
   fine total arithmetically impossible under the statute it cited. Each would
   have wrongly confirmed a live claim. The defence that worked every time was
   opening the primary page and checking its date.

4. The corpus is growing about thirty times faster than it resolves: 78 claims
   added against 7 resolved, with 213 now open. Many are keyed to institutional
   calendars slower than the run cadence. Logged as CAL-007. Worth deciding
   whether the ledger needs a retirement rule as well as an expiry rule.

5. Contradiction density has stopped discriminating in theme-selection: 12 of 22
   themes score the maximum because every sweep carries two counter-signals and
   three or four contradictions by template. Selection is now effectively driven
   by staleness and evidence delta alone. Instrument-review item.

6. Two independent Phase D agents noted that this is the second consecutive run
   whose scenarios converge on the same conclusion, that the record of an AI
   incident is controlled by the party least interested in publishing it, even
   though the narrative forms diverged sharply. If a third run lands there
   again, that is a pipeline attractor rather than three independent findings.

7. The memory evaluation flagged that the mechanism its entire chain rests on
   (server-side memory reorganisation) reaches the run only through a sweep
   Delta bullet with no source URL. The citation gate is scoped to Confirmed
   bullets, so the gate passes on its literal terms while the load-bearing fact
   is unsourced. Worth considering whether the gate should reach dated factual
   assertions in the Delta section.

## Phase E, not run

Per the run instruction, outlook-generator and delta-report were NOT run. They
are the human review gate and the maintainer runs them after reviewing this run.
