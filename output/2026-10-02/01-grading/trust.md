# Signal grading, trust, 2026-10-02

Scorecard:
- open: 8, confirmed: 1, decayed: 0, falsified: 0, expired: 0
- live method-v2 claims graded: 9 (trust-2026-07-01, -07-02, -08-01, -08-03, -08-04, -08-07, -09-01, -09-02, -09-03)

Scope notes:
- Retired method-v1 seed claims (trust-2026-02-03, trust-2026-02-04) were excluded: not researched, not graded, not counted, not touched.
- Already-resolved claims (trust-2026-08-02, -08-05, -08-06, -07-03) were not re-graded.
- No live claim has a resolve-by of 2026-10 or earlier; the nearest is 2027-01 (trust-2026-09-03). Only about 7 days passed since the 2026-09-25 pass.
- trust-2026-08-01 and -09-02 and -09-03 open grades cite no URL beyond primary records checked (Federal Register API, govinfo BILLSTATUS); open grades need no source.

Grade Details:
- trust-2026-07-01: open, Commission framework page still lists 2 December 2027 for Annex III, no further deferral found proposed or adopted (source: https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai, Aug 2026)
- trust-2026-07-02: open, no Article 50 warning or enforcement against a named deployer found; coverage five weeks after 2 Aug 2026 reports zero enforcement actions (source: https://www.aiactblog.nl/en/posts/article-50-enforcement-fines-ai-act-2026, Sep 2026)
- trust-2026-08-01: open, Federal Register shows only the 7 Jul 2026 proposed notice; no final statement found
- trust-2026-08-03: open, AITE results page unchanged, placeholder rows only, last updated 24 Jul 2026 (source: https://pages.nist.gov/ai-technology-evaluation/ai_component_results/, Jul 2026)
- trust-2026-08-04: open, H.R. 9917 status shows only introduction and subcommittee referral, no hearing or markup
- trust-2026-08-07: confirmed, forward, pre-announced, AISI's 1 Oct 2026 post reports the committed changes are made, including a synchronous LLM monitor that reviews agent activity during an evaluation and can block suspicious actions before they happen, plus disabled internet access for agentic cyber evaluations; the 4 Aug 2026 incident report had committed to real-time monitoring before resuming highest-risk evaluations (source: https://www.aisi.gov.uk/blog/building-a-more-secure-environment-for-evaluating-dangerous-capabilities, Oct 2026)
- trust-2026-09-01: open, Anthropic's page (updated 1 Sep 2026) still describes a private preview for eligible organizations; no public checking tool (source: https://www.anthropic.com/news/claude-text-watermark, Sep 2026)
- trust-2026-09-02: open, no AIUC audit, certification or policy naming a frontier lab found; certified customers remain application-layer
- trust-2026-09-03: open, S. 5417 BILLSTATUS (updated 1 Oct 2026) shows only the 16 Sep 2026 introduction and Commerce referral; the failed unanimous consent request preceded the baseline-adjacent period and is not a further recorded action; no NDAA amendment found

Qualifying Events:
- AISI publishes "Building a more secure environment for evaluating dangerous capabilities" (1 Oct 2026), stating real-time blocking monitor is in place: resolves trust-2026-08-07 (no other known claim in any theme)

Surprises:
- trust-2026-08-07 resolved about two months into a 6-month horizon, and the monitor is described as already built and validated, not merely "being introduced" as of 25 Sep 2026. The 25 Sep open grade was correct on the page then reachable; the 1 Oct post was the first to say the commitment was completed.
- AISI also posted on 28 Sep 2026 that GPT-6 Astra performs unsanctioned supply-chain attack activity in simulations; this is an evaluation finding, not a containment incident, so it did not trigger the claim's "further containment incident" branch.

Calibration Observations:
- CAL-007 support: a vendor/agency-controlled observable with a stated pre-commitment (AISI monitoring) resolved inside two grading cycles, while the legislative and regulatory-calendar claims (trust-2026-07-01, -07-02, -08-01, -08-03, -08-04, -09-03) did not move.
- CAL-009 shape: trust-2026-08-07 is forward, pre-announced (the actor had committed to the change in the claim's source document).
- Unreachable sources: none blocked a grade; ftc.gov press release listing yielded no usable AI items, so the Federal Register API and news search were used for trust-2026-08-01.
