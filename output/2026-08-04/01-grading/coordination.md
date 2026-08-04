# Signal grading, coordination, 2026-08-04

Scorecard:
- open: 4, confirmed: 0, decayed: 1, falsified: 0, expired: 0

Grade Details:
- coordination-2026-02-03: open, the Digital Omnibus amendments entered into force 29 Jul 2026 fixing high-risk deadlines at Dec 2027 and Aug 2028, both still inside the claim's 2029-02 horizon, so the region-specific compliance driver is delayed rather than removed (source: https://www.orrick.com/en/Insights/2026/07/EU-AI-Act-Update-Digital-Omnibus-Finalizes-8-Compliance-Changes, Jul 2026)
- coordination-2026-02-04: decayed, JumpCloud's Q3 2026 IT Trends study found organizations requiring human review before high-risk AI actions fell from 40% to 25% in six months while full autonomy without review rose from 11% to 26%, a reversal of the claimed formalization trend (source: https://www.prnewswire.com/news-releases/new-study-most-organizations-have-abandoned-human-ai-oversight-302825345.html, Jul 2026)
- coordination-2026-07-01: open, A2A remains at 150+ supporting organizations with no published cross-organization production deployment, and resolve-by 2027-09 is thirteen months away (source: https://www.linuxfoundation.org/press/a2a-protocol-surpasses-150-organizations-lands-in-major-cloud-platforms-and-sees-enterprise-production-use-in-first-year, Apr 2026)
- coordination-2026-07-02: open, no agentic commerce protocol has been deprecated, merged, or absorbed; ACP persists as infrastructure after OpenAI retired Instant Checkout and the market is answering fragmentation with aggregation layers rather than consolidation (source: https://www.digitalapplied.com/blog/agentic-commerce-standards-ucp-acp-ap2-2026-merchant-guide, Jun 2026)
- coordination-2026-07-03: open, the nearest events are a laboratory worm against OpenClaw (ClawWorm, Mar 2026) and a Sentry-mediated agentjacking exposure across an estimated 2,388 organizations (Jun 2026), neither of which is in-the-wild propagation between organizations over an inter-agent protocol (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-agentjacking-self-replicating-ai-worms-202/, Jun 2026)

Surprises:
- coordination-2026-02-04 decayed rather than crept toward confirmation. The pipeline treated oversight formalization as a one-way ratchet with 30 months still to run, but measured human-review requirements went backwards, from 40% to 25%, in a single six-month window. Adoption speed is outrunning governance construction, which is the opposite of the seeded assumption.
- The commerce-protocol layer is answering fragmentation with aggregation, not consolidation. ACP, UCP, AP2 and MPP all persist and intermediaries now abstract over all of them, which makes coordination-2026-07-02's deprecation test less likely to trigger than its wording implies.
- Standards contestation moved up a level rather than settling: the IETF 126 agentproto BoF (Jul 2026) put MCP, A2A, ACP, ANP and Agntcy in front of a chartering vote. That is a mechanism coordination-2026-07-01 does not anticipate, since a binding RFC could make raw supporter counts a poor proxy for interoperability.
