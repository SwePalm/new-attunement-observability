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

- [ ] SELECTION.md

## Phase D, deep dives (selected themes)

Filled in after selection.

## Blocked items

None recorded yet.
