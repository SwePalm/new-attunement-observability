# Signal grading, intelligence, 2026-08-04

Scorecard:
- open: 3, confirmed: 1, decayed: 1, falsified: 0, expired: 0

Grade Details:
- intelligence-2026-02-03: open, v1 seed retired from scoring per CLAUDE.md; the 12-36 month horizon runs to 2029-02 and no decisive movement was found this month
- intelligence-2026-02-04: open, v1 seed retired from scoring per CLAUDE.md; the 12-36 month horizon runs to 2029-02 and no decisive movement was found this month
- intelligence-2026-07-01: confirmed, independent leaderboards now show frontier models above 50% on Humanity's Last Exam (Claude Fable 5 at 53.3%, Claude Opus 5 at 52.6%), roughly 13 months ahead of the resolve-by date (source: https://artificialanalysis.ai/evaluations/humanitys-last-exam, Aug 2026)
- intelligence-2026-07-02: open, no credible audit yet reports frontier-model production success above 80%, and the largest new production telemetry sample points the other way (56.6% success across 4.5M runs on 6,259 deployed agents), with 13 months still on the horizon (source: https://www.foundra.ai/key-reads/ai-agent-production-reliability-testing-2026, Jul 2026)
- intelligence-2026-07-03: decayed, US procurement evaluation is consolidating inside government rather than around an independent third party: EO 14409 (Jun 2026) created a classified benchmarking process under the NSA director and halted CAISI's public model-evaluation reporting, while GSA's proposed AI clause reserves government self-assessment against its own benchmarks rather than citing an external evaluator (source: https://www.budd.senate.gov/2026/06/30/budd-calls-for-caisi-to-resume-publishing-research-on-frontier-ai-models/, Jun 2026)

Surprises:
- intelligence-2026-07-01 confirmed one month after being logged with a 13-month horizon. The claim was written as a stretch target and was already close to met at logging time (Gemini 3 Pro era leaderboards were near 38-45%); the July sweep appears to have anchored on the AI Index snapshot rather than on live leaderboards.
- intelligence-2026-07-03 decayed against evidence that predates the claim. EO 14409 was signed 2026-06-02 and GSA's self-assessment clause was proposed 2026-03-06, both before the claim was logged in 2026-07, so the sweep logged a claim whose central mechanism was already being displaced by state-run and classified evaluation.
- The reliability picture moved backwards, not forwards. Foundra's July 2026 telemetry (56.6% task success over 4.5M production runs) is materially worse than the ~67% baseline the claim was built on, and tau-bench style multi-attempt decay (about 60% single-attempt falling to about 25% over eight consecutive attempts) suggests the 80% target is further away than the claim implies.
