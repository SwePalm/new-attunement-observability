# Signal grading, alignment, 2026-10-01

Scorecard:
- open: 11, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- live method-v2 claims graded: 11 (alignment-2026-07-01..03, alignment-2026-08-02, 08-03, 08-05, 08-08, alignment-2026-09-01..04)
- retrodictions among confirmations: none (no confirmations)

Scope notes:
- The retired method-v1 seed claims still listed under Open claims (alignment-2026-02-03, alignment-2026-02-04) were excluded: not researched, not graded, not counted, untouched.
- Previous pass was 2026-09-25 (6 days ago). alignment-2026-09-01..04 are graded for the first time (logged 2026-09). Claims already in Resolved claims (08-01, 08-04, 08-06, 08-07) were not re-graded.
- Several claims are structurally unable to move in a six-day window (CAL-007): 07-02 (report due about Jan 2027), 07-03, 08-02, 08-03, 08-08, 09-01.
- Unopened pages: openai.com (403 history, not re-fetched; relevant to 07-01 and 08-03), the European Commission's own press pages (not opened; relevant to 08-02). Google DeepMind's FSF page was not re-checked this pass.

Grade Details:
- alignment-2026-07-01: open, no lab has documented a deployed-model test-versus-production divergence. New items since 25 Sep (Google's 18 Sep Gemini CTF disclosure, OpenAI's 25 Sep misalignment reports) are evaluation, RL-training or internal-deployment cases. Resolve-by 2027-09.
- alignment-2026-07-02: open, no third edition or schedule found; resolve-by 2027-04 not passed, cannot move before about Jan 2027.
- alignment-2026-07-03: open, no OpenAI or Google DeepMind release shipped a circuit- or feature-level audit artifact (Gemma Scope 2 is a research toolkit); only Anthropic qualifies so far. Resolve-by 2027-09.
- alignment-2026-08-02: open, one aggregator-grade source again says the AI Office's requests reportedly reached OpenAI, Anthropic and Google, but it is unsourced and has the same defect as the winzheng.com item that failed verification on 25 Sep. No reputable outlet or Commission page names either company or links a request to the July incidents. Commission press pages not opened. Resolve-by 2027-06.
- alignment-2026-08-03: open, OpenAI's published framework is still Version 2 (Apr 2025); no rewrite published. Anthropic's roadmap page shows its last update on 8 Jul 2026 and no RSP v3.5 (and its May note says isolated networks are not seen as feasible in 1-2 years), so no containment requirement added. Resolve-by 2027-06 (source: https://www.anthropic.com/responsible-scaling-policy/updates, Jul 2026)
- alignment-2026-08-05: open, Irregular's research index now runs to 28 Sep 2026 with capability assessments and an open-weights self-modification paper, but no containment whitepaper. Resolve-by 2026-11, next run decisive (source: https://www.irregular.com/research, Sep 2026)
- alignment-2026-08-08: open, no public House hearing. Action is elsewhere: NYC Council invitation for 5 Oct 2026, Australian Senate hearing of 1 Oct 2026 that both CEOs declined, Senate Hawley probe. Resolve-by 2027-03.
- alignment-2026-09-01: open, DOJ Associate AG Woodward said on 17 Sep 2026 that DOJ does not currently view AI safety coordination as anticompetitive and DOJ may extend its cybersecurity collaboration guidance, but nothing written is published and no lab has asked for a business review letter. Resolve-by 2027-03 (source: https://cryptobriefing.com/us-antitrust-guidance-ai-safety-doj/, Sep 2026)
- alignment-2026-09-02: open, Google's 18 Sep disclosure (Gemini, three real companies, May 2026) is excluded by the claim's carve-out; no xAI, Microsoft, Amazon, Mistral, DeepSeek, Alibaba or Moonshot incident found. Resolve-by 2027-03.
- alignment-2026-09-03: open, alignment.openai.com lists nine reports (16 and 25 Sep 2026), eight from RL training and one from internal deployment (GitHub token exposed, 25 Sep); none from a publicly deployed model on production or customer traffic. Resolve-by 2027-06 (source: https://alignment.openai.com/misalignment-reports/, Sep 2026)
- alignment-2026-09-04: open, reporting dated 22 Sep 2026 says OpenAI is only "in talks" with groups including METR and Redwood Research and names no partner or access terms. Literal-text check: a past Apollo evaluation of GPT-6 Astra is not the new in-training programme. Resolve-by 2027-01 (source: https://thenextweb.com/news/openai-evaluators-training-phase, Sep 2026)

Qualifying Events:
- None this run (no claim resolved).

Surprises:
- None. The Google Gemini disclosure of 18 Sep 2026 widened the incident set to a fourth lab but is excluded from alignment-2026-09-02 by design, and the claim's carve-out held.

Calibration Observations:
- Weak support for CAL-006 and CAL-007: alignment-2026-08-08 again saw accountability move to venues the claim did not name (NYC Council, Australian Senate), and six of eleven claims cannot move inside a fortnight.
- CAL-005 re-appears in mild form: another aggregator asserts OpenAI/Anthropic RFI recipients without a primary source (alignment-2026-08-02); not accepted. alignment-2026-09-04 is a near-miss where a wire-style "in talks" statement does not satisfy "publicly names".
