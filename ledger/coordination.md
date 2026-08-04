# Signals ledger, coordination

Format: see ledger/README.md. Append-only.

## Open claims

### coordination-2026-02-03
- Claim: Region-specific compliance configurations and contractual liability clauses become normal deployment architecture.
- Horizon: 12–36 months (logged 2026-02, resolve by 2029-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: open
- Grades:
 - 2026-07: open, EU Digital Omnibus (Jun 2026) postponed Annex III obligations to Dec 2027 and Annex I to Aug 2028, slowing the assumed compliance-configuration mechanism (source: https://www.gibsondunn.com/eu-ai-act-omnibus-agreement-postponed-high-risk-deadlines-and-other-key-changes/, Jun 2026)
 - 2026-08-04: open, the Digital Omnibus amendments entered into force 29 Jul 2026 with high-risk deadlines fixed at Dec 2027 and Aug 2028, both still inside this claim's 2029-02 horizon, so the compliance-configuration driver is delayed rather than removed (source: https://www.orrick.com/en/Insights/2026/07/EU-AI-Act-Update-Digital-Omnibus-Finalizes-8-Compliance-Changes, Jul 2026)

### coordination-2026-07-01
- Claim: A2A adoption doubles: 300+ organizations support the protocol, or a major cross-organization production deployment (two companies' agent fleets coordinating) is publicly documented, by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://www.programming-helper.com/tech/agent-to-agent-protocol-2026-google-a2a-standard, Apr 2026
- Status: open
- Grades:
 - 2026-08-04: open, A2A stands at 150+ supporting organizations (up from 50+ at launch) with no named cross-organization production deployment published, and the IETF 126 agentproto BoF (Jul 2026) suggests the standards layer is still contested rather than consolidating; resolve-by 2027-09 is far off (source: https://www.linuxfoundation.org/press/a2a-protocol-surpasses-150-organizations-lands-in-major-cloud-platforms-and-sees-enterprise-production-use-in-first-year, Apr 2026)

### coordination-2026-07-02
- Claim: The commerce-protocol layer consolidates: at least one of ACP/UCP/MPP is deprecated, merged, or absorbed by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://opascope.com/insights/ai-shopping-assistant-guide-2026-agentic-commerce-protocols/, 2026
- Status: open
- Grades:
 - 2026-08-04: open, no protocol has been deprecated, merged, or absorbed; ACP survives as infrastructure after OpenAI retired Instant Checkout (Mar 2026), UCP went self-serve on Shopify (Jun 2026), and the market is answering fragmentation with aggregation layers such as Adyen Agentic rather than consolidation (source: https://www.digitalapplied.com/blog/agentic-commerce-standards-ucp-acp-ap2-2026-merchant-guide, Jun 2026)

### coordination-2026-07-03
- Claim: A documented multi-org incident propagates through inter-agent protocols (an agent-to-agent cascade failure or attack) by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://blog.cyberdesserts.com/ai-agent-security-risks/, Feb 2026
- Status: open
- Grades:
 - 2026-08-04: open, the closest events remain research demonstrations (ClawWorm, a lab worm against OpenClaw, Mar 2026) and a data-source compromise affecting an estimated 2,388 organizations (Agentjacking via Sentry, Jun 2026), neither of which is propagation between organizations over an inter-agent protocol (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-agentjacking-self-replicating-ai-worms-202/, Jun 2026)

### coordination-2026-08-01
- Claim: The IESG approves a charter for an IETF working group on AI agent communication protocols (agentproto or a renamed successor), visible as a chartered WG on datatracker.ietf.org, by 2027-03.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-03)
- Source: https://datatracker.ietf.org/doc/minutes-126-agentproto-202607230700/, Jul 2026
- Status: open
- Grades:
  - none yet

### coordination-2026-08-02
- Claim: Public UCP conformance monitoring reports at least 100 verified UCP stores exposing a payment capability, up from zero of 11,414 verified stores on 7 Jul 2026, by 2027-02.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-02)
- Source: https://ucpchecker.com/blog/state-of-agentic-commerce-july-2026, Jul 2026
- Status: open
- Grades:
  - none yet

### coordination-2026-08-03
- Claim: Senator Mark Warner formally introduces the AI AGENT Act as a numbered bill in the US Senate, with a congress.gov record, by 2027-03.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-03)
- Source: https://www.warner.senate.gov/newsroom/press-releases/warner-unveils-discussion-draft-of-legislation-to-create-innovative-market-for-secure-artificial-intelligence-agents/, Jun 2026
- Status: open
- Grades:
  - none yet

### coordination-2026-08-04
- Claim: NIST publishes on csrc.nist.gov a draft Special Publication or Internal Report on software and AI agent identity and authorization that supersedes the 5 Feb 2026 concept paper, by 2027-03.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-03)
- Source: https://csrc.nist.gov/pubs/other/2026/02/05/accelerating-the-adoption-of-software-and-ai-agent/ipd, Aug 2026
- Status: open
- Grades:
  - none yet

## Resolved claims

### coordination-2026-02-04
- Claim: Oversight roles and escalation pathways become formalized in operating models rather than ad hoc responses.
- Horizon: 12–36 months (logged 2026-02, resolve by 2029-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: decayed
- Grades:
 - 2026-07: open, early corroboration (agent gateways, HITL playbooks) but formalization not yet the operating norm; most orgs lack agent visibility (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-ai-agent-governance-framework-gap-20260403/, Apr 2026)
 - 2026-08-04: decayed, the trend reversed over six months: organizations requiring human review before high-risk AI actions fell from 40% to 25% while full autonomy without review rose from 11% to 26%, and only 44% keep AI-specific incident response procedures (source: https://www.prnewswire.com/news-releases/new-study-most-organizations-have-abandoned-human-ai-oversight-302825345.html, Jul 2026)

### coordination-2026-02-01
- Claim: Bounded AI-assisted workflows expand with stronger pre-deployment control checks in higher-impact contexts.
- Horizon: 0–12 months (logged 2026-02, resolve by 2027-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: confirmed
- Grades:
 - 2026-07: confirmed, 80.9% of technical teams past planning into agent testing/deployment with productized control patterns, though containment controls (37-40%) lag adoption; claim vague enough to be near-unfalsifiable (source: https://www.okta.com/newsroom/articles/ai-agents-at-work-2026-agentic-enterprise-security/, 2026)

### coordination-2026-02-02
- Claim: Governance and legal teams gain earlier authority in implementation and procurement decisions.
- Horizon: 0–12 months (logged 2026-02, resolve by 2027-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: confirmed
- Grades:
 - 2026-07: confirmed, procurement routinely requires governance evidence and audit rights; 77% of orgs building formal AI governance programs; same vagueness caveat (source: https://prefactor.tech/learn/ai-governance-compliance-statistics, 2026)
