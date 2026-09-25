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

Scorecard (final, after one correction during Phase B): 43 confirmed,
3 falsified, 0 decayed, 0 expired, 167 open. As first graded: 42 confirmed,
168 open. perception-2026-08-04 was corrected open to confirmed (forward) after
the Phase B sweep found Instagram's 31 Aug 2026 distribution limit on undisclosed
AI-generated profiles, which the grading pass missed because it looked only for
friction on labeled content. Recorded as an appended grade line.
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

Complete. All 22 sweeps written and validated mechanically by the orchestrator
(section order; two dated sources on every Confirmed bullet; one on every
Regulatory, Capital, Technical, Emerging and Counter bullet; zero em-dashes).
71 new claims appended (IDs <theme>-2026-09-NN); ledger diff re-checked, no
deletions other than Status updates and intact block moves. Live open claims:
167 + 71 = 238.

Each sweep ran the CAL-004 pre-check (search for the qualifying event before
logging) and several dropped candidates that had already happened. Sweeps caught
contamination again in most themes, notably AI-generated pages naming OpenAI,
Anthropic and Google as recipients of the Commission's 29 Aug 2026 information
requests (the Commission named no one), a Council of Europe convention "adopted
16 Sep 2026" (adopted 2024), and fabricated EU KIDS Act provisions. Each is
recorded under Contradictions as unverified, not used as evidence.

Duplicate claims across themes (CAL-008 firing inside this run). Sweeps run in
parallel cannot see each other's candidates, so six events were logged more than
once, 13 claims for 6 events; 71 claims watch about 64 distinct events. The
ledger is append-only, so these stay, and graders should grade each group once
and cross-reference:
- Amazon or Meta sues the other over Muse: agency-2026-09-01, desire-2026-09-02, responsibility-2026-09-01
- state AG action against OpenAI over the Hugging Face incident: authority-2026-09-03, responsibility-2026-09-02
- Senate frontier duty-of-care bill introduced: authority-2026-09-01, governance-2026-09-01
- California kill-switch bill introduced: authority-2026-09-04, governance-2026-09-03
- lawsuit against California SB 1119: belonging-2026-09-01, desire-2026-09-03
- Anthropic opens its watermark detector beyond private preview: trust-2026-09-01, truth-2026-09-03


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

Six selected, cut at the fifth-ranked total (16) with ties included, the rule
the 2026-08 runs used: intelligence 19, perception 19, learning 18, identity 17,
agency 16, belonging 16. First alternate: meaning 15. Five of the six come from
the never-dived backlog; agency is the only re-dive (last dived 2026-07-03).
Two backlog themes remain (dependency, meaning), due 2026-12; the next run
should take both regardless of score.

Grade surprises were scored with retrodictions at 0 (CAL-004), pre-announced
confirmations at 1 (CAL-009), and shared-event clusters split across themes
(CAL-008). Contradiction density was scored on substantive tensions only,
excluding unverified-source notes and outlet dating disputes, because a literal
count scores all 22 themes 5. This choice decides slot six: under a literal
count, meaning replaces agency. Recorded in SELECTION.md's sensitivity note and
flagged below for instrument-review.

The first run attempt at Phase C died on a session usage limit before writing
anything; it was rerun from scratch after the reset.

## Phase D, deep dives (selected themes)

- [x] intelligence, six steps
- [x] perception, six steps
- [x] learning, six steps
- [x] identity, six steps
- [x] agency, six steps
- [x] belonging, six steps

All 36 step files written, each step in order. Ledger untouched by Phase D.
No scenario names a calibration heuristic in reader-facing prose.

Each theme was assigned a distinct structural form at the prompt level:
intelligence, one public number revisited at intervals; perception, one
viewer's feeds over a week; learning, one school year term by term from a
student and a parent; identity, one day as a sequence of identity checks;
agency, one disputed agent purchase as a case file; belonging, a year of
messages between two people.

Scenario eval scores: intelligence 7.7, perception 7.5, learning 7.5, identity
7.5, belonging 7.2, agency 7.1. Mean 7.4, against 7.6 on 2026-08-13. All six
citation gates pass, each with defects recorded rather than concealed; agency's
includes one load-bearing defect (the agent-drafted mandate is PESTLE inference
stated as present fact). Distinctiveness scored 5 to 7, below last run's 7 to 8.

## Blocked items

None. Every checklist item is [x].

## Flag for human review

1. Stacking. PR #2 (the 2026-08-13 run) was unmerged at run start, so this
   branch is stacked on observatory-2026-08 and its PR targets that branch.
   Merge PR #2 first; GitHub will then retarget this PR to main.

2. The retrodiction rate fell sharply, 13 of 42 confirmations against five of six
   last run, but the forward confirmations are weaker evidence than the number
   suggests. Four events account for 10 of the 29 forward confirmations
   (CAL-008), and most of the rest restate a pre-announced plan or a scheduled
   procedural step (CAL-009). The run's cleanest foresight signal is its three
   falsifications, all genuine forward misses.

3. Duplicate claims, now an instrument problem. Parallel sweeps cannot see each
   other's candidates, so six events were logged 13 times in this run's 71 new
   claims (groups listed under Phase B). The duplicates cannot be removed from an
   append-only ledger. Instrument-review item: a dedupe pass across all sweeps'
   Ledger Candidates before any ledger append, or a shared event registry.

4. A new scenario attractor. The incident-record conclusion flagged twice before
   was avoided in four of six themes; agency touches it and perception sits next
   to it, both recorded in their evals. But four evals independently reported that
   every scarce good this run resolves to the same thing: a real person being
   present (company in the stuck part, being checked by someone who knows you,
   a correspondent who notices silence). Distinctiveness fell to 5 to 7 as a
   result. The forms diverged and the endings did not, which points at the
   forces-feelings "irreplaceable thing" step rather than the narrative form.
   Instrument-review item.

5. Theme-selection instrument. The contradiction-density dimension is undefined
   in the skill, and this run's reading (substantive tensions only) decided the
   sixth slot: a literal count would have selected meaning instead of agency.
   Evidence delta also saturated (15 of 22 themes scored 5 over 43 days).
   Coverage arithmetic is tight: 22 themes at a 5-month rule need about 4.4 dives
   a month, and six re-dives fall due by 2026-12. The next run should take
   dependency and meaning (the last two backlog themes) regardless of score.

6. A later phase corrected a Phase A grade for the third consecutive run
   (perception-2026-08-04, found by the perception sweep). The grading pass
   searched for the claim's intended mechanism, not the literal claim text.

7. Research tooling degraded mid-run. The session-wide WebSearch budget ran out
   during Phase A and Brave Search rate-limited. Later graders fell back to direct
   fetches and a Bing News RSS discovery one-liner; a helper script for it was
   blocked by the permission classifier and was not worked around. Several
   graders say their coverage on specific claims was thinner as a result, and
   their `open` grades there mean "not found" (CAL-005). A session usage limit also
   killed the first Phase C attempt, which was rerun cleanly.

8. Process slips, harmless. Several subagents ran a read-only `git diff --stat`
   against their instructions. Nothing was staged or changed by it.

9. Near-term resolutions worth grading first next run: meaning-2026-08-05 and
   labor-2026-09-01 and meaning-2026-09-01 (California signing deadline 30 Sep
   2026), identity-2026-08-01 (OIDF vote closes 30 Sep), coordination-2026-08-01
   (IESG telechat 8 Oct), dependency-2026-08-02 (FSB report, Oct), learning-
   2026-08-02 (Maryland deadline 22 Oct), authority-2026-07-01 (Colorado hearing
   26 Oct).

## Phase E, not run

outlook-generator and delta-report are the human review gate and were not run.
