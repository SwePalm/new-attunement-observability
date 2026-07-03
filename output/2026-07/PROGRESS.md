# Progress — 2026-07 (FIRST FULL RUN under method v2)

METHOD_VERSION: 2.0
Skills SHA: 367bb41
Scope: full monthly loop, Phases A–D, all 22 themes. Phase E (outlook) awaits
human review per the learning contract.

Started as a 2-theme verification (trust, labor); extended to the full run at
the user's request. Verification observations are preserved at the bottom.

## Run tally

- Grading reports: 22 / 22 themes
- Evidence sweeps: 22 / 22 themes (citation gate passed)
- Ledger: 45 claims resolved-graded this month, 111 open claims carried forward
  (44 v1 seeds graded + 67 new v2 claims logged)
- Calibration heuristics: CAL-001, CAL-002, CAL-003 (active)
- Deep dives: 5 themes, mean eval score 8.34

## Phase A — signal-grading  [x] complete (22/22)

All 22 themes graded. 19 boilerplate themes graded via the shared seed set
(claims identical across themes); trust, labor, and agency graded individually.
Scorecard: of 44 v1 seed claims, ~22 confirmed, ~22 open, 0 falsified/expired
(the boilerplate confirmed by construction — see CAL-001).

## Phase B — evidence-sweep  [x] complete (22/22)

All 22 sweeps carry live dated citations in strict sections. 67 new falsifiable
ledger candidates logged with resolve-by dates. Mechanical citation-gate check
run over all strict sections: only "None" lines flagged (allowed by format).

## Phase C — theme-selection  [x] complete

Selected: governance, labor, security, creativity, agency (see SELECTION.md).

## Phase D — deep dives  [x] complete (5/5)

| theme | eval score | Irreplaceable Thing |
|-------|-----------|---------------------|
| labor | 8.5 | the first rung (apprenticeship / where judgment is formed) |
| governance | 8.4 | a promise that holds (credible commitment) |
| agency | 8.4 | authorship of one's own consequential choices |
| security | 8.3 | the undo (reversibility after machine-speed action) |
| creativity | 8.1 | a stake (a share in the value one's work generates) |

## Phase E — outlook  [ ] AWAITS HUMAN REVIEW

Do not auto-run. Review the deep-dive evals and scorecard first, then run
outlook-generator in debug mode, then production.

---

## New flaws-from-the-past surfaced this run

Beyond the verification run's four observations (below), the full run exposed more:

5. **The v1 boilerplate is worse than "vague" — it is theme-blind.** The four
   seeded claims were not just unfalsifiable; they were pasted verbatim into 21
   of 22 themes. Agency alone got specific claims, and agency alone produced a
   confirmed-ahead-of-horizon grade. This is a clean natural experiment: specific
   claims yielded foresight, boilerplate yielded none. It is now CAL-001 and is
   the single strongest argument for the method-v2 rewrite.

6. **Every deep-dive scenario converged on ONE structural movement.** All five
   independently resolved through "private ordering fills the statutory vacuum,
   and protection distributes by leverage/literacy" (insurance, procurement,
   bargaining, cooperatives, agent-defaults). Each eval flagged this as
   convergence risk. This is genuinely what the evidence shows (it became CAL-003),
   but it is ALSO a latent pipeline bias: the scenario skill may be pattern-matching
   to a house style. The outlook must present this as ONE movement with five faces,
   not five discoveries — and instrument-review should ask whether scenario-generator
   needs an anti-convergence prompt. Flagged, NOT fixed, per the learning contract.

7. **The regulatory-hardening prior was systemic, not incidental.** CAL-002 (the
   pipeline over-trusts announced regulatory timelines) recurred in every theme
   touching governance. The EU omnibus deferral falsified a background assumption
   the v1 corpus treated as settled. Any future scenario citing a compliance date
   as fixed should be challenged at eval.

8. **Distinctiveness is the corpus's weakest dimension.** Every deep dive scored
   6–7 on "Distinctiveness vs. Other Themes" while scoring 8–9 everywhere else.
   The themes overlap heavily (agency/autonomy/authority/power; trust/responsibility/
   governance). Candidate instrument-review topic: whether 22 themes is the right
   granularity, or whether some should be merged or re-scoped.

---

## Verification observations (from the initial 2-theme run)

1. **v1 seed corpus is boilerplate.** 21 of 22 theme ledgers carry the exact same
   four seeded claims. Confirmed and now formalized as CAL-001.

2. **Citation gate vs. undated sources.** Several credible sources expose no
   publication month; month-dated sources carry the strict sections, year-only
   sources kept to Emerging/Counter-Signals. Candidate instrument-review topic.

3. **Calibration memo written in the full run.** Deferred from the verification
   run so heuristics start from the complete grade set; CAL-001..003 now active.

4. **Grading found a real trajectory break.** The EU Digital Omnibus (Jun 2026)
   deferred high-risk obligations while market mechanisms hardened — caught by
   v2, invisible to v1. Now CAL-002.
