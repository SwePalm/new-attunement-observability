# Signals ledger, dependency

Format: see ledger/README.md. Append-only.

## Open claims

### dependency-2026-02-03
- Claim: Region-specific compliance configurations and contractual liability clauses become normal deployment architecture.
- Horizon: 12–36 months (logged 2026-02, resolve by 2029-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: open
- Grades:
 - 2026-07: open, EU Digital Omnibus (Jun 2026) postponed Annex III obligations to Dec 2027 and Annex I to Aug 2028, slowing the assumed compliance-configuration mechanism (source: https://www.gibsondunn.com/eu-ai-act-omnibus-agreement-postponed-high-risk-deadlines-and-other-key-changes/, Jun 2026)
 - 2026-08-04: open, region-specific configuration is hardening faster than the contractual leg (China's anthropomorphic-AI measures effective 15 Jul 2026 forced ByteDance and Alibaba into region-specific withdrawal and rebuild), while the EU's model contractual clauses for AI procurement remain the 2025 baseline rather than a new normal (source: https://english.news.cn/20260715/4bf39cb3c4db42babc10ed37932cfd94/c.html, Jul 2026)

### dependency-2026-02-04
- Claim: Oversight roles and escalation pathways become formalized in operating models rather than ad hoc responses.
- Horizon: 12–36 months (logged 2026-02, resolve by 2029-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: open
- Grades:
 - 2026-07: open, early corroboration (agent gateways, HITL playbooks) but formalization not yet the operating norm; most orgs lack agent visibility (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-ai-agent-governance-framework-gap-20260403/, Apr 2026)
 - 2026-08-04: open, regulators are now pushing formalization explicitly (FSB consultation of 10 Jun 2026 proposes 12 sound practices for organisation-wide AI governance across the lifecycle, final report due Oct 2026), but it is still supervisory expectation rather than observed operating norm (source: https://www.fsb.org/2026/06/sound-practices-for-responsible-adoption-of-artificial-intelligence-ai-consultation-report/, Jun 2026)

### dependency-2026-07-02
- Claim: A major platform introduces usage-pattern interventions for heavy companion users (dose warnings, session limits, human-referral prompts) by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://pmc.ncbi.nlm.nih.gov/articles/PMC12928748/, 2026
- Status: open
- Grades:
 - 2026-08-04: open, the intervention is now mandated in China (CAC-led measures effective 15 Jul 2026 require reminders after two hours of continuous use plus dependency and distress intervention) but the two largest incumbents, Doubao and Qwen, withdrew companion features instead of shipping usage-pattern controls, so no major platform has yet introduced them (source: https://english.news.cn/20260715/4bf39cb3c4db42babc10ed37932cfd94/c.html, Jul 2026)

### dependency-2026-07-03
- Claim: An AI-provider outage or model deprecation causes documented, material operational disruption at enterprises dependent on it, prompting public post-mortems, by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://zylos.ai/research/2026-03-26-agent-interoperability-protocols-mcp-a2a-acp-convergence/, Mar 2026
- Status: open
- Grades:
 - 2026-08-04: open, the disruption leg is already met (Anthropic's 12 Jun 2026 suspension of Claude Fable 5 and Mythos 5 under a US export-control directive hit enterprises with embedded production integrations, and OpenAI degraded for 17 days in Jul 2026) but no provider or affected enterprise has published a post-mortem, which is the leg the claim rests on (source: https://www.gtlaw.com/en/insights/2026/6/ai-company-anthropic-suspends-access-to-claude-fable-5-claude-mythos-5-following-us-export-control-directive, Jun 2026)

### dependency-2026-08-01
- Claim: HM Treasury designates at least one AI model provider (for example OpenAI, Anthropic, Google DeepMind, or Mistral) as a Critical Third Party under the UK CTP regime, extending the 10 Jul 2026 cloud-only list.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-06)
- Source: https://www.bankofengland.co.uk/news/2026/july/uk-financial-regulators-to-begin-overseeing-critical-third-parties-announced-by-hmt, Jul 2026
- Status: open
- Grades:
  - none yet

### dependency-2026-08-02
- Claim: The FSB publishes its final Sound Practices for Responsible Adoption of AI report and it explicitly addresses concentration or substitutability of AI service providers, beyond the generic third-party risk framing of the 10 Jun 2026 consultation.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-01)
- Source: https://www.fsb.org/2026/06/fsb-consults-on-sound-practices-for-the-responsible-adoption-of-artificial-intelligence-ai/, Jun 2026
- Status: open
- Grades:
  - none yet

### dependency-2026-08-03
- Claim: At least one Agentic AI Foundation platinum member (Anthropic, OpenAI, Microsoft, Google, AWS, Block, Bloomberg, or Cloudflare) publicly announces a dated end-of-support in its own MCP client or hosted platform for HTTP+SSE transport or Dynamic Client Registration, converting the 2026-07-28 spec deprecations into an enforced migration deadline for third-party server operators.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-06)
- Source: https://blog.modelcontextprotocol.io/posts/2026-07-28/, Jul 2026
- Status: open
- Grades:
  - none yet

### dependency-2026-08-04
- Claim: The Cyberspace Administration of China or a provincial cyberspace regulator publishes an enforcement action (fine, service suspension, or rectification order) naming a specific provider under the anthropomorphic-AI measures that took effect 15 Jul 2026.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-03)
- Source: https://www.artificialintelligence-news.com/news/china-ai-companion-rules/, Jul 2026
- Status: open
- Grades:
  - none yet

## Resolved claims

### dependency-2026-07-01
- Claim: A regulator or standards body issues formal guidance on "AI concentration risk" (dependence on single AI providers) for critical sectors by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://www.theactuary.com/2026/06/25/price-proof-insurance-policies-ai-enabled-world, Jun 2026
- Status: confirmed
- Grades:
 - 2026-08-04: confirmed, APRA's 30 Apr 2026 letter to all APRA-regulated entities (banking, insurance, superannuation) found entities heavily dependent on a single AI provider across multiple use cases with untested exit strategies and set an expectation of "active management of concentration risk" over critical AI providers, which is formal regulatory guidance on AI concentration risk in a critical sector and predates the claim's logging (source: https://www.apra.gov.au/apra-letter-to-industry-on-artificial-intelligence-ai, Apr 2026)

### dependency-2026-02-01
- Claim: Bounded AI-assisted workflows expand with stronger pre-deployment control checks in higher-impact contexts.
- Horizon: 0–12 months (logged 2026-02, resolve by 2027-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: confirmed
- Grades:
 - 2026-07: confirmed, 80.9% of technical teams past planning into agent testing/deployment with productized control patterns, though containment controls (37-40%) lag adoption; claim vague enough to be near-unfalsifiable (source: https://www.okta.com/newsroom/articles/ai-agents-at-work-2026-agentic-enterprise-security/, 2026)

### dependency-2026-02-02
- Claim: Governance and legal teams gain earlier authority in implementation and procurement decisions.
- Horizon: 0–12 months (logged 2026-02, resolve by 2027-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: confirmed
- Grades:
 - 2026-07: confirmed, procurement routinely requires governance evidence and audit rights; 77% of orgs building formal AI governance programs; same vagueness caveat (source: https://prefactor.tech/learn/ai-governance-compliance-statistics, 2026)
