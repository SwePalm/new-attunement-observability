# Signals ledger, security

Format: see ledger/README.md. Append-only.

## Open claims

### security-2026-02-03
- Claim: Region-specific compliance configurations and contractual liability clauses become normal deployment architecture.
- Horizon: 12–36 months (logged 2026-02, resolve by 2029-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: open
- Grades:
 - 2026-07: open, EU Digital Omnibus (Jun 2026) postponed Annex III obligations to Dec 2027 and Annex I to Aug 2028, slowing the assumed compliance-configuration mechanism (source: https://www.gibsondunn.com/eu-ai-act-omnibus-agreement-postponed-high-risk-deadlines-and-other-key-changes/, Jun 2026)
 - 2026-08-04: open, the AI Omnibus entered into force on 27 Jul 2026 confirming Annex III compliance at Dec 2027 and embedded-product high-risk at Aug 2028, so region-specific configuration is being designed for but is not yet default deployment architecture (source: https://digital-strategy.ec.europa.eu/en/news/ai-omnibus-enters-force, Jul 2026)

### security-2026-02-04
- Claim: Oversight roles and escalation pathways become formalized in operating models rather than ad hoc responses.
- Horizon: 12–36 months (logged 2026-02, resolve by 2029-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: open
- Grades:
 - 2026-07: open, early corroboration (agent gateways, HITL playbooks) but formalization not yet the operating norm; most orgs lack agent visibility (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-ai-agent-governance-framework-gap-20260403/, Apr 2026)
 - 2026-08-04: open, IBM Cost of a Data Breach 2026 (Jul 2026) reports only about one in four organisations have adopted AI and automation in security operations and just 18% point agents at vulnerability management, so escalation pathways remain partially formalised at best (source: https://newsroom.ibm.com/2026-07-29-ibm-study-one-in-four-malicious-breaches-are-ai-enabled,-costing-companies-6-million-on-average, Jul 2026)

### security-2026-07-02
- Claim: Agent-skill marketplaces adopt mandatory signing/review: a major marketplace requires cryptographic signing or pre-publication review for all skills by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://blog.cyberdesserts.com/ai-agent-security-risks/, Feb 2026
- Status: open
- Grades:
 - 2026-08-04: open, no major marketplace yet mandates signing or pre-publication review; NVIDIA is only experimenting with cryptographic signing for its own published skills (May 2026) and the official MCP registry still performs no scanning, with resolve-by 2027-09 not passed (source: https://developer.nvidia.com/blog/nvidia-verified-agent-skills-provide-capability-governance-for-ai-agents/, May 2026)

### security-2026-07-03
- Claim: The autonomous-agent share of reported AI breaches rises above 1 in 5 in the next annual threat-landscape report.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-07)
- Source: https://foresiet.com/blog/ai-security-incidents-attack-paths-april-2026/, Apr 2026
- Status: open
- Grades:
 - 2026-08-04: open, the two major annual reports published since logging (Check Point AI Security Report 2026, Jul 2026; IBM Cost of a Data Breach 2026, Jul 2026) report AI-enabled breach shares (one in four malicious breaches AI-enabled) but neither breaks out an autonomous-agent share, so the metric is not yet reported and resolve-by 2027-07 has not passed (source: https://newsroom.ibm.com/2026-07-29-ibm-study-one-in-four-malicious-breaches-are-ai-enabled,-costing-companies-6-million-on-average, Jul 2026)

### security-2026-08-01
- Claim: The European Commission's AI Office takes its first publicly reported formal Chapter V step against a named GPAI model provider (a request for information, a model evaluation, or a corrective or risk-mitigation measure).
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-05)
- Source: https://www.wsgr.com/en/insights/eu-ai-act-enforcement-phase-begins.html, Aug 2026
- Status: open
- Grades:
  - none yet

### security-2026-08-02
- Claim: METR and Redwood Research publish their promised joint report on the OpenAI evaluation-escape incident, stating the terms of engagement, scope and findings.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-01)
- Source: https://openai.com/index/hugging-face-model-evaluation-security-incident/, Jul 2026
- Status: open
- Grades:
  - none yet

### security-2026-08-03
- Claim: Anthropic publishes the redacted transcripts of the three cybersecurity-evaluation incidents it disclosed on 30 Jul 2026.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-02)
- Source: https://www.anthropic.com/news/investigating-incidents-cybersecurity-evals, Jul 2026
- Status: open
- Grades:
  - 2026-08-13: open, the self-imposed one-week deadline for the lightly redacted PyPI transcript (pledged 30 Jul 2026) lapsed around 6 Aug 2026 with no transcript on the Anthropic newsroom as of 13 Aug 2026, and a House oversight letter to CEO Dario Amodei dated 10 Aug 2026 now presses for the incident material, so publication is slipping while resolve-by 2027-02 has not passed (source: https://www.anthropic.com/news/investigating-incidents-cybersecurity-evals, Jul 2026)

### security-2026-08-04
- Claim: The MCP maintainers publish a protocol revision or registry policy that makes server identity cryptographically verifiable, removing the current specification statement that serverInfo is self-reported, unverified, and must not be used for security decisions.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-06)
- Source: https://modelcontextprotocol.io/specification/2026-07-28/server/discover, Aug 2026
- Status: open
- Grades:
  - none yet

## Resolved claims

### security-2026-07-01
- Claim: A second largely-autonomous attack campaign (AI executing majority of tactical operations) is publicly documented by a government agency or major vendor by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://blog.barracuda.com/2026/02/27/agentic-ai--the-2026-threat-multiplier-reshaping-cyberattacks/, Feb 2026
- Status: confirmed
- Grades:
 - 2026-08-04: confirmed, Check Point Research's AI Security Report 2026 documents a campaign against nine Mexican government agencies in which one operator's AI tools executed 5,317 commands across 34 sessions with minimal human direction between steps, a second largely-autonomous campaign documented by a major vendor 13 months before resolve-by (source: https://www.checkpoint.com/press-releases/check-point-research-ai-has-crossed-from-assistant-to-operator-rewriting-the-rules-of-autonomous-ai-cyber-attack-and-defense/, Jul 2026)

### security-2026-02-01
- Claim: Bounded AI-assisted workflows expand with stronger pre-deployment control checks in higher-impact contexts.
- Horizon: 0–12 months (logged 2026-02, resolve by 2027-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: confirmed
- Grades:
 - 2026-07: confirmed, 80.9% of technical teams past planning into agent testing/deployment with productized control patterns, though containment controls (37-40%) lag adoption; claim vague enough to be near-unfalsifiable (source: https://www.okta.com/newsroom/articles/ai-agents-at-work-2026-agentic-enterprise-security/, 2026)

### security-2026-02-02
- Claim: Governance and legal teams gain earlier authority in implementation and procurement decisions.
- Horizon: 0–12 months (logged 2026-02, resolve by 2027-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: confirmed
- Grades:
 - 2026-07: confirmed, procurement routinely requires governance evidence and audit rights; 77% of orgs building formal AI governance programs; same vagueness caveat (source: https://prefactor.tech/learn/ai-governance-compliance-statistics, 2026)
