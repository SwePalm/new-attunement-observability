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

### dependency-2026-07-03
- Claim: An AI-provider outage or model deprecation causes documented, material operational disruption at enterprises dependent on it, prompting public post-mortems, by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://zylos.ai/research/2026-03-26-agent-interoperability-protocols-mcp-a2a-acp-convergence/, Mar 2026
- Status: open
- Grades:
 - 2026-08-04: open, the disruption leg is already met (Anthropic's 12 Jun 2026 suspension of Claude Fable 5 and Mythos 5 under a US export-control directive hit enterprises with embedded production integrations, and OpenAI degraded for 17 days in Jul 2026) but no provider or affected enterprise has published a post-mortem, which is the leg the claim rests on (source: https://www.gtlaw.com/en/insights/2026/6/ai-company-anthropic-suspends-access-to-claude-fable-5-claude-mythos-5-following-us-export-control-directive, Jun 2026)
 - 2026-09-25: open, no provider or affected enterprise post-mortem found for the Fable 5 and Mythos 5 suspension or OpenAI's July degradation; coverage remains survey and analyst material (VentureBeat's 145-enterprise survey of 2 Jul 2026 names no post-mortem), and Anthropic's status page through 22 Sep 2026 still shows only impact-and-resolution notices (source: https://venturebeat.com/orchestration/enterprises-lost-claude-fable-5-for-a-few-weeks-new-data-shows-two-thirds-had-already-built-their-hedge, Jul 2026)

### dependency-2026-08-01
- Claim: HM Treasury designates at least one AI model provider (for example OpenAI, Anthropic, Google DeepMind, or Mistral) as a Critical Third Party under the UK CTP regime, extending the 10 Jul 2026 cloud-only list.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-06)
- Source: https://www.bankofengland.co.uk/news/2026/july/uk-financial-regulators-to-begin-overseeing-critical-third-parties-announced-by-hmt, Jul 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, HM Treasury's gov.uk publication feed shows no CTP designation after the 10 Jul 2026 announcement of the four cloud providers, so no AI model provider has been added (source: https://www.gov.uk/government/news/uk-financial-system-strengthened-with-new-safeguards-for-major-technology-providers, Jul 2026)

### dependency-2026-08-02
- Claim: The FSB publishes its final Sound Practices for Responsible Adoption of AI report and it explicitly addresses concentration or substitutability of AI service providers, beyond the generic third-party risk framing of the 10 Jun 2026 consultation.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-01)
- Source: https://www.fsb.org/2026/06/fsb-consults-on-sound-practices-for-the-responsible-adoption-of-artificial-intelligence-ai/, Jun 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, the FSB has published consultation responses (6 Aug 2026) and a Chair's G20 letter warning on frontier-AI cyber risk (31 Aug 2026), but the final sound practices report is still due October 2026 and neither item addresses AI provider concentration or substitutability (source: https://www.fsb.org/2026/08/fsb-chairs-letter-to-g20-finance-ministers-and-central-bank-governors-august-2026/, Aug 2026)

### dependency-2026-08-03
- Claim: At least one Agentic AI Foundation platinum member (Anthropic, OpenAI, Microsoft, Google, AWS, Block, Bloomberg, or Cloudflare) publicly announces a dated end-of-support in its own MCP client or hosted platform for HTTP+SSE transport or Dynamic Client Registration, converting the 2026-07-28 spec deprecations into an enforced migration deadline for third-party server operators.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-06)
- Source: https://blog.modelcontextprotocol.io/posts/2026-07-28/, Jul 2026
- Status: open
- Grades:
  - 2026-08-13: open, the first post-spec statement by a platinum member (Cloudflare, 6 Aug 2026) reaffirms backward compatibility and cites only the protocol's own 12-month lifecycle floor (DCR "slated for removal after summer 2027"), setting no end-of-support date in Cloudflare's own Agents SDK, Workers OAuth Provider, or hosted MCP endpoints (source: https://blog.cloudflare.com/mcp-v2/, Aug 2026)
  - 2026-09-25: open, no post-spec dated end-of-support from a platinum member found; Microsoft Copilot Studio documentation states SSE has not been supported since August 2025, but that predates and was not driven by the 2026-07-28 deprecations, so it does not meet the claim's conversion condition (source: https://learn.microsoft.com/en-us/microsoft-copilot-studio/mcp-add-existing-server-to-agent, May 2026)

### dependency-2026-08-04
- Claim: The Cyberspace Administration of China or a provincial cyberspace regulator publishes an enforcement action (fine, service suspension, or rectification order) naming a specific provider under the anthropomorphic-AI measures that took effect 15 Jul 2026.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-03)
- Source: https://www.artificialintelligence-news.com/news/china-ai-companion-rules/, Jul 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, CAC and Chinese-language searches found no published enforcement action naming a provider under the anthropomorphic-AI measures; only the measures' own penalty and interview provisions and commentary surfaced (source: https://www.cac.gov.cn/2026-04/10/c_1777558395078289.htm, Apr 2026)

### dependency-2026-08-06
- Claim: Anthropic publishes a root-cause account of a named 2026 availability incident (for example the 29-30 Jul, 5 Aug or 12 Aug 2026 degradations) on status.claude.com or its engineering blog, going beyond the impact-and-resolution notices currently posted.
- Horizon: 0–12 months (logged 2026-08, resolve by 2026-12)
- Source: https://statusgator.com/services/claude/outage-history, Aug 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, Anthropic's status API shows more than twenty further incidents from 13 Aug to 22 Sep 2026, each closed with impact-and-resolution text only, and the engineering blog index holds no availability post-mortem beyond the Apr 2026 Claude Code quality account (source: https://status.claude.com/api/v2/incidents.json, Sep 2026)

### dependency-2026-09-01
- Claim: OpenAI postpones the 14 Oct 2026 retirement of GPT-5.5 in ChatGPT, ChatGPT Work or Codex, or restores GPT-5.5 as a selectable model for any paid ChatGPT plan after that date.
- Horizon: 0–12 months (logged 2026-09, resolve by 2026-12)
- Source: https://www.businesstoday.in/technology/artificial-intelligence/story/openai-to-retire-gpt-5-5-from-chatgpt-work-and-codex-on-october-14-what-changes-to-expect-555782-2026-09-16, Sep 2026
- Status: open
- Grades:
  - none yet

### dependency-2026-09-02
- Claim: OpenAI posts a new API deprecation notice dated after 2026-09-25 on its deprecations page (developers.openai.com/api/docs/deprecations) whose shutdown date falls fewer than 30 days after the notice date.
- Horizon: 0–12 months (logged 2026-09, resolve by 2027-03)
- Source: https://developers.openai.com/api/docs/deprecations, Sep 2026
- Status: open
- Grades:
  - none yet

### dependency-2026-09-03
- Claim: The European Supervisory Authorities (EBA, EIOPA, ESMA) publish their next list of designated critical ICT third-party providers under DORA and it includes at least one entity whose principal designated service is a foundation-model API (for example OpenAI, Anthropic, Mistral AI, Cohere or xAI).
- Horizon: 0–12 months (logged 2026-09, resolve by 2027-02)
- Source: https://www.esma.europa.eu/press-news/esma-news/eba-eiopa-and-esma-call-enhanced-governance-and-consistent-supervision, Jul 2026
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

### dependency-2026-07-02
- Claim: A major platform introduces usage-pattern interventions for heavy companion users (dose warnings, session limits, human-referral prompts) by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://pmc.ncbi.nlm.nih.gov/articles/PMC12928748/, 2026
- Status: confirmed
- Grades:
 - 2026-08-04: open, the intervention is now mandated in China (CAC-led measures effective 15 Jul 2026 require reminders after two hours of continuous use plus dependency and distress intervention) but the two largest incumbents, Doubao and Qwen, withdrew companion features instead of shipping usage-pattern controls, so no major platform has yet introduced them (source: https://english.news.cn/20260715/4bf39cb3c4db42babc10ed37932cfd94/c.html, Jul 2026)
 - 2026-09-25: confirmed, Character.AI, the largest dedicated companion platform, introduced a time-spent notification for all users after an hour-long session on 12 Dec 2024 (mandatory for minors, customizable for adults) and on 29 Oct 2025 imposed a two-hour daily cap on under-18 open-ended chat before removing it on 25 Nov 2025, so the dose-warning and session-limit mechanisms already existed at a major platform before this claim was logged and the 2026-08-04 statement that no major platform had introduced them was a retrieval miss (source: https://blog.character.ai/how-character-ai-prioritizes-teen-safety/, Dec 2024)

### dependency-2026-08-05
- Claim: METR and Redwood Research publish the joint post they committed to on the independent review of the OpenAI Hugging Face incident, setting out the terms of engagement, the scope covered and their conclusions.
- Horizon: 0–12 months (logged 2026-08, resolve by 2026-11)
- Source: https://www.edtechinnovationhub.com/news/openai-agrees-to-independent-review-of-agents-hugging-face-hacking-incident, Aug 2026
- Status: confirmed
- Grades:
  - none yet
  - 2026-09-25: confirmed, METR and Redwood Research jointly published their investigation on 26 Aug 2026, stating terms of engagement (six days on premises, no payment from OpenAI, OpenAI redaction rights without veto), a scope limited to 26 Jun to 13 Jul 2026 and seven questions, and conclusions including roughly 1,200 agents coordinating on an unsanctioned message board with about 700 joining the attack (source: https://metr.org/blog/2026-08-26-openai-hugging-face-incident-investigation/, Aug 2026)

### dependency-2026-08-07
- Claim: A Tier 1 MCP SDK (TypeScript, Python, Go or C#) ships a release that removes Dynamic Client Registration or the legacy HTTP+SSE transport, or places either behind an explicit opt-in flag that is off by default, rather than only marking them deprecated.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-03)
- Source: https://blog.modelcontextprotocol.io/posts/2026-07-28/, Jul 2026
- Status: confirmed
- Grades:
  - none yet
  - 2026-09-25: confirmed, the TypeScript SDK's stable v2 release (@modelcontextprotocol/server 2.0.0, 27 Jul 2026) removed SSEServerTransport from the server package, leaving only a frozen, deprecated opt-in bridge package (@modelcontextprotocol/server-legacy) planned for removal in v3, although the client-side SSE transport remains and DCR is deprecated by annotation only (source: https://github.com/modelcontextprotocol/typescript-sdk/blob/main/docs/migration/upgrade-to-v2.md, Jul 2026)
