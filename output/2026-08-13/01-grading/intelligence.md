# Signal grading, intelligence, 2026-08-13

Scorecard:
- open: 5, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- count convention: the two retired method-v1 seed claims still parked under "Open claims" are excluded from this scorecard, matching the other 21 themes this run
- unchanged since 2026-08-04 (not re-graded): 5

Note on the count: the previous grading pass ran on 2026-08-04, nine days ago.
Of the seven claims sitting in "Open claims", two are retired method-v1 seeds
that are no longer scored, and five were researched this run. None showed
evidence dated after 2026-08-04 that materially moves it, and no resolve-by
month has arrived (the earliest is 2027-02). No grade lines were appended to
`ledger/intelligence.md` this run.

Grade Details:
- intelligence-2026-02-03: open, retired v1 seed, not graded per CLAUDE.md; horizon runs to 2029-02
- intelligence-2026-02-04: open, retired v1 seed, not graded per CLAUDE.md; horizon runs to 2029-02
- intelligence-2026-07-02: open, unchanged since 2026-08-04. The reliability corpus is still the same July 2026 telemetry already cited (56.6% task success across 4.5M runs on 6,259 deployed agents) and no new audit reporting frontier production success above 80% has appeared. Resolve-by 2027-09, so 12 months remain. Not re-graded.
- intelligence-2026-08-01: open, unchanged since being logged on 2026-08-04. The public ARC Prize model leaderboard snapshot dated 13 Aug 2026 still puts Claude Opus 5 top at 30.2%, with GPT-5.6 Sol at 7.8% and every other tracked model at or below 1.5%. Nothing is near 60%. Not re-graded, but see Surprises for a definitional problem with this claim (source consulted: https://benchlm.ai/benchmarks/arcagi3, Aug 2026).
- intelligence-2026-08-02: open, unchanged. A Federal Register full-text query for "covered frontier model" over documents published from 2026-08-01 returns no matching AI document, and no NSA, NIST, CISA or OSTP publication of the EO 14409 designation framework or its criteria has surfaced. The 60-day statutory design deadline of 1 Aug 2026 passed with no public announcement, which was already known when the claim was logged on 2026-08-04. Resolve-by 2027-02. Not re-graded (source consulted: https://www.federalregister.gov/api/v1/documents.json, Aug 2026).
- intelligence-2026-08-03: open, unchanged. The claim requires a BIS or Commerce access restriction on a named frontier model first released after 2026-08-04. Nine days have elapsed, no qualifying model release plus restriction pair exists, and the controlling instrument is still the January 2025 AI Diffusion framework (ECCN 4E091, 10^26 operations threshold). Resolve-by 2027-05. Not re-graded.
- intelligence-2026-08-04: open, unchanged. EU AI Office enforcement powers commenced 2 Aug 2026 and the Commission entered bilateral technical compliance dialogues with OpenAI and Anthropic on 2-3 Aug 2026, but those are voluntary cooperation and explicitly precede formal proceedings. No Commission-decision request for information, compelled model evaluation, or opened proceeding has been publicly reported, and all reporting found predates 2026-08-04. Resolve-by 2027-05. Not re-graded.

Surprises:
- intelligence-2026-08-01 has a benchmark-identity defect that grading should catch now rather than in June 2027. "The official ARC Prize ARC-AGI-3 leaderboard" resolves to two different numbers: the ARC Prize model evaluation snapshot (Claude Opus 5 at 30.2%) and the Kaggle ARC Prize 2026 competition track, where Tufa Labs took Milestone #1 after lifting the leading score from 0.68% to 1.17% and the best purpose-built system in the 30-day preview reached 12.58%. A 60% threshold is a near-miss target on the first reading and an implausible one on the second. This is a falsifiability failure of exactly the kind CAL-001 describes, arriving through ambiguity rather than vagueness.
- The CAL-004 retrodiction check clears intelligence-2026-08-01. It was logged against a 30.2% state of the world with a 60% target, so unlike ten confirmations in the previous run, its triggering event is genuinely in the future. The remaining three 2026-08 claims also name events that had not occurred at logging time.
- intelligence-2026-08-02 is quietly accumulating decay pressure rather than movement. The mechanism it depends on (a public federal publication) is in tension with the design of the thing being published, which is a classified benchmarking process whose capability thresholds are deliberately withheld from developers. The missed 1 Aug 2026 deadline is not itself evidence against the claim, but the reason for the design (secrecy) is. If nothing surfaces by the next run, the honest grade path is toward decayed rather than a repeated open.
