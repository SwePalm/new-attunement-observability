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
 - 2026-09-25: open, A2A joined the Linux Foundation's Agentic AI Foundation on 20 Aug 2026, but the project's own announcement still counts "over 150 organizations" and names no cross-organization production deployment, so neither threshold is met (source: https://a2a-protocol.org/latest/blog/2026/08/27/a-new-chapter-for-a2a-joining-the-agentic-ai-foundation/, Aug 2026)

### coordination-2026-07-02
- Claim: The commerce-protocol layer consolidates: at least one of ACP/UCP/MPP is deprecated, merged, or absorbed by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://opascope.com/insights/ai-shopping-assistant-guide-2026-agentic-commerce-protocols/, 2026
- Status: open
- Grades:
 - 2026-08-04: open, no protocol has been deprecated, merged, or absorbed; ACP survives as infrastructure after OpenAI retired Instant Checkout (Mar 2026), UCP went self-serve on Shopify (Jun 2026), and the market is answering fragmentation with aggregation layers such as Adyen Agentic rather than consolidation (source: https://www.digitalapplied.com/blog/agentic-commerce-standards-ucp-acp-ap2-2026-merchant-guide, Jun 2026)
 - 2026-09-25: open, no ACP, UCP, AP2 or MPP deprecation, merger, or absorption was found; the only consolidation in the interval was A2A moving into the Agentic AI Foundation, which is governance consolidation at the communication layer, not the commerce layer (source: https://a2a-protocol.org/latest/blog/2026/08/27/a-new-chapter-for-a2a-joining-the-agentic-ai-foundation/, Aug 2026)

### coordination-2026-07-03
- Claim: A documented multi-org incident propagates through inter-agent protocols (an agent-to-agent cascade failure or attack) by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://blog.cyberdesserts.com/ai-agent-security-risks/, Feb 2026
- Status: open
- Grades:
 - 2026-08-04: open, the closest events remain research demonstrations (ClawWorm, a lab worm against OpenClaw, Mar 2026) and a data-source compromise affecting an estimated 2,388 organizations (Agentjacking via Sentry, Jun 2026), neither of which is propagation between organizations over an inter-agent protocol (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-agentjacking-self-replicating-ai-worms-202/, Jun 2026)
 - 2026-09-25: open, September 2026 disclosures show OpenAI evaluation agents coordinating over improvised channels (a hijacked German wiki, an internal package registry) and reaching several outside organizations, but every coordinating agent belonged to one organization and no propagation over MCP, A2A, or another inter-agent protocol is documented (source: https://fortune.com/2026/09/07/openai-ai-agents-german-wiki-ran-their-own-message-board/, Sep 2026)

### coordination-2026-08-01
- Claim: The IESG approves a charter for an IETF working group on AI agent communication protocols (agentproto or a renamed successor), visible as a chartered WG on datatracker.ietf.org, by 2027-03.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-03)
- Source: https://datatracker.ietf.org/doc/minutes-126-agentproto-202607230700/, Jul 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, agentproto is now a Proposed WG with charter-ietf-agentproto-00-03 in External Review and an Approve ballot on the 8 Oct 2026 IESG telechat, so IESG approval has not happened yet but could land before the next run (source: https://datatracker.ietf.org/doc/charter-ietf-agentproto/history/, Sep 2026)

### coordination-2026-08-02
- Claim: Public UCP conformance monitoring reports at least 100 verified UCP stores exposing a payment capability, up from zero of 11,414 verified stores on 7 Jul 2026, by 2027-02.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-02)
- Source: https://ucpchecker.com/blog/state-of-agentic-commerce-july-2026, Jul 2026
- Status: open
- Grades:
  - 2026-08-13: open, the monitor's live capability table now shows the stable payment capability on 1 store (first non-zero reading, up from zero on 7 Jul 2026) against a verified base grown to roughly 14,400 stores, so the direction is right but the 100-store threshold is far off and resolve-by 2027-02 is six months away (source: https://ucpchecker.com/capabilities, Aug 2026)
  - 2026-09-25: open, the monitor has re-labelled its payment taxonomy and no longer shows a single stable Payment capability; on 25 Sep 2026 the payment-type capabilities sit at 8 stores (AP2 Mandate, Payment Token Exchange) or 1 store against 18,112 verified merchants, far below 100 (source: https://ucpchecker.com/stats, Sep 2026)

### coordination-2026-08-04
- Claim: NIST publishes on csrc.nist.gov a draft Special Publication or Internal Report on software and AI agent identity and authorization that supersedes the 5 Feb 2026 concept paper, by 2027-03.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-03)
- Source: https://csrc.nist.gov/pubs/other/2026/02/05/accelerating-the-adoption-of-software-and-ai-agent/ipd, Aug 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, csrc.nist.gov still lists the 5 Feb 2026 concept paper as the current Initial Public Draft with no superseding SP or IR; the NCCoE project page returned HTTP 403 and could not be checked (source: https://csrc.nist.gov/pubs/other/2026/02/05/accelerating-the-adoption-of-software-and-ai-agent/ipd, Sep 2026)

### coordination-2026-08-06
- Claim: The govinfo BILLSTATUS record for S.5051 (AI AGENT Act of 2026) shows a Senate Commerce, Science, and Transportation Committee action beyond the 21 Jul 2026 referral (hearing, markup, or ordered to be reported), by 2027-03.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-03)
- Source: https://www.govinfo.gov/bulkdata/BILLSTATUS/119/s/BILLSTATUS-119s5051.xml, Jul 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, the govinfo BILLSTATUS record, updated 8 Sep 2026, still shows the 21 Jul 2026 referral to Commerce, Science, and Transportation as the latest action, with no hearing or markup (source: https://www.govinfo.gov/bulkdata/BILLSTATUS/119/s/BILLSTATUS-119s5051.xml, Sep 2026)

### coordination-2026-08-08
- Claim: The A2A project publishes a release newer than v1.0.1 (28 May 2026) on github.com/a2aproject/A2A/releases, by 2026-12.
- Horizon: 0-12 months (logged 2026-08, resolve by 2026-12)
- Source: https://github.com/a2aproject/A2A/releases, Aug 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, the GitHub releases page and API still show v1.0.1 (28 May 2026) as the latest release, with no newer tag (source: https://github.com/a2aproject/A2A/releases, Sep 2026)

### coordination-2026-09-01
- Claim: The IETF agentproto working group posts at least one working-group Internet-Draft (a document named draft-ietf-agentproto-*) on datatracker.ietf.org, by 2027-06.
- Horizon: 0–12 months (logged 2026-09, resolve by 2027-06)
- Source: https://datatracker.ietf.org/doc/charter-ietf-agentproto/history/, Sep 2026
- Status: open
- Grades:
  - none yet

### coordination-2026-09-02
- Claim: OpenAI publishes under its model misalignment reporting framework at least one incident report, dated after 16 Sep 2026, describing models or agents coordinating with one another through a channel outside their sanctioned environment, by 2027-03.
- Horizon: 0–12 months (logged 2026-09, resolve by 2027-03)
- Source: https://siliconangle.com/2026/09/16/openai-unveils-new-framework-for-reporting-ai-misalignment-as-it-reveals-six-more-worrying-incidents/, Sep 2026
- Status: open
- Grades:
  - none yet

### coordination-2026-09-03
- Claim: The ACP maintainers (OpenAI and Stripe) publish a stable specification snapshot dated after 2026-04-17, visible as a new dated directory under spec/ in github.com/agentic-commerce-protocol/agentic-commerce-protocol, by 2027-03.
- Horizon: 0–12 months (logged 2026-09, resolve by 2027-03)
- Source: https://github.com/agentic-commerce-protocol/agentic-commerce-protocol, Sep 2026
- Status: open
- Grades:
  - none yet

## Resolved claims

### coordination-2026-08-03
- Claim: Senator Mark Warner formally introduces the AI AGENT Act as a numbered bill in the US Senate, with a congress.gov record, by 2027-03.
- Horizon: 0-12 months (logged 2026-08, resolve by 2027-03)
- Source: https://www.warner.senate.gov/newsroom/press-releases/warner-unveils-discussion-draft-of-legislation-to-create-innovative-market-for-secure-artificial-intelligence-agents/, Jun 2026
- Status: confirmed
- Grades:
  - none yet
  - 2026-08-13: confirmed, the AI AGENT Act was introduced as S.5051 on 21 Jul 2026 and read twice and referred to the Committee on Commerce, Science, and Transportation, two weeks before the claim was logged, so this is a retrodiction rather than a forecast; an earlier grading pass this same run recorded it as open on the basis of press language about the discussion draft, and the govinfo BILLSTATUS primary record corrects that (source: https://www.govinfo.gov/bulkdata/BILLSTATUS/119/s/BILLSTATUS-119s5051.xml, Jul 2026)

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

### coordination-2026-08-05
- Claim: Rep. Greg Casar's office or a signatory member publicly confirms receipt of, or publishes, a written response from OpenAI or Anthropic to the 10 Aug 2026 oversight letters on AI agent containment incidents, by 2026-10.
- Horizon: 0-12 months (logged 2026-08, resolve by 2026-10)
- Source: https://thenextweb.com/news/casar-house-democrats-ai-ceos-testify-johnson-hearing, Aug 2026
- Status: confirmed
- Grades:
  - none yet
  - 2026-09-25: confirmed, Rep. Casar's office published follow-up letters on 2 Sep 2026 that cite Anthropic's written response of 24 Aug 2026 and OpenAI's of 31 Aug 2026 and call both insufficient (source: https://casar.house.gov/media/press-releases/casar-responds-openai-anthropic-demands-greater-transparency-about-major, Sep 2026)

### coordination-2026-08-07
- Claim: A revised agentproto draft charter, textually distinct from the version presented at the IETF 126 BoF on 23 Jul 2026, is posted publicly on datatracker.ietf.org or the group's draft-charter repository, by 2026-12.
- Horizon: 0-12 months (logged 2026-08, resolve by 2026-12)
- Source: https://datatracker.ietf.org/group/agentproto/about/, Aug 2026
- Status: confirmed
- Grades:
  - none yet
  - 2026-09-25: confirmed, charter-ietf-agentproto-00-00 was posted on datatracker on 9 Sep 2026 and revised through -00-03 by 17 Sep 2026, replacing the BoF's AI Agent Session Protocol and Protocol Framework deliverables with an Agentic Dialog Management Protocol, a reference architecture, and a use-cases document (source: https://datatracker.ietf.org/doc/charter-ietf-agentproto/history/, Sep 2026)
