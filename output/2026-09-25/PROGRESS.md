# Run progress, 2026-09-25

METHOD_VERSION: 2.1
Git SHA: d1b3ad23f1c1dd8145e9550978a6f5d68153e389
Run date: 2026-09-25
Previous run: 2026-08-13 (43 days earlier)
Branch: observatory-2026-09, stacked on observatory-2026-08 (PR #2, unmerged at run start)

States: `[ ]` pending, `[/]` in progress, `[x]` done, `[!]` blocked

Run notes:
- PR #2 (the 2026-08-13 run) was still open when this run started, so main did
  not carry that run's ledger grades or its 78 new claims. Branching from main
  would have forked the append-only ledger and re-graded a stale state. This run
  therefore branches from observatory-2026-08 and its PR targets that branch.
- The scheduled-task instruction names METHOD_VERSION 2.0 and an
  output/YYYY-MM/ folder. CLAUDE.md on the working branch is METHOD_VERSION 2.1
  with per-day folders, and CLAUDE.md is the method contract, so this run writes
  to output/2026-09-25/ and stamps 2.1.
- The 2026-02 method-v1 seed claims are retired and are not re-graded.

## Phase A, signal-grading (22 themes)

Complete. All 22 themes researched; every one of the 213 live method-v2 claims
received one ledger grade line dated 2026-09-25 (the 43-day interval justified a
full pass, unlike the nine-day interval last run). Retired 2026-02 seeds were not
graded and are excluded from every count.

Scorecard: 42 confirmed, 3 falsified, 0 decayed, 0 expired, 168 open.
Falsified: labor-2026-08-03 and labor-2026-08-05 (August Challenger report),
power-2026-08-05 (FERC abeyance moved PJM's filing past the resolve-by).

Retrodiction check (CAL-004): 13 of 42 confirmations were satisfied before their
own logging date, down from five of six on 2026-08-13. Of the 29 forward
confirmations, 10 trace to just four events (CAL-008) and most of the rest track
pre-announced plans or scheduled procedural steps (CAL-009). The three
falsifications are the run's cleanest foresight signal, all three genuine misses.

Ledger integrity verified mechanically: every deleted diff line in ledger/ is a
Status line update or a claim block moved intact to Resolved claims.

Calibration pass: CAL-002 through CAL-007 re-confirmed with expiries extended.
CAL-008 (correlated cross-theme confirmations) and CAL-009 (forward but
pre-announced confirmations) added. Nine active heuristics, inside the bound of
10. Two below-bar patterns recorded on a non-active watch list.

Tooling note: the session-wide WebSearch budget ran out during Phase A and Brave
Search rate-limited. Later graders fell back to direct page fetches and a Bing
News RSS discovery query; a helper script for it was blocked by the permission
classifier for most agents and was not worked around. Three graders ran one
read-only `git diff --stat` against instructions; nothing was changed by it.


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

- [ ] agency
- [ ] alignment
- [ ] authority
- [ ] autonomy
- [ ] belonging
- [ ] coordination
- [ ] creativity
- [ ] dependency
- [ ] desire
- [ ] governance
- [ ] identity
- [ ] intelligence
- [ ] labor
- [ ] learning
- [ ] meaning
- [ ] memory
- [ ] perception
- [ ] power
- [ ] responsibility
- [ ] security
- [ ] trust
- [ ] truth

## Phase C, theme-selection

- [ ] SELECTION.md

## Phase D, deep dives (selected themes)

(filled in after selection)

## Blocked items

## Flag for human review

## Phase E, not run

outlook-generator and delta-report are the human review gate and were not run.
