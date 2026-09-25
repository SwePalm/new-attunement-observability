# Signals ledger, memory

Format: see ledger/README.md. Append-only.

## Open claims

### memory-2026-02-03
- Claim: Region-specific compliance configurations and contractual liability clauses become normal deployment architecture.
- Horizon: 12–36 months (logged 2026-02, resolve by 2029-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: open
- Grades:
 - 2026-07: open, EU Digital Omnibus (Jun 2026) postponed Annex III obligations to Dec 2027 and Annex I to Aug 2028, slowing the assumed compliance-configuration mechanism (source: https://www.gibsondunn.com/eu-ai-act-omnibus-agreement-postponed-high-risk-deadlines-and-other-key-changes/, Jun 2026)
 - 2026-08-04: open, v1 seeded boilerplate retired from delta reporting per CLAUDE.md and status-noted only; EU AI Act Article 50 transparency duties became applicable on 2 Aug 2026 while Annex III high-risk duties stay deferred to Dec 2027, so region-specific configuration pressure is real but partial, and the 2029-02 horizon is far from resolution (source: https://ai-act-service-desk.ec.europa.eu/en/ai-act/timeline/timeline-implementation-eu-ai-act, Aug 2026)

### memory-2026-02-04
- Claim: Oversight roles and escalation pathways become formalized in operating models rather than ad hoc responses.
- Horizon: 12–36 months (logged 2026-02, resolve by 2029-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: open
- Grades:
 - 2026-07: open, early corroboration (agent gateways, HITL playbooks) but formalization not yet the operating norm; most orgs lack agent visibility (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-ai-agent-governance-framework-gap-20260403/, Apr 2026)
 - 2026-08-04: open, v1 seeded boilerplate retired from delta reporting per CLAUDE.md and status-noted only; July 2026 practitioner analysis still finds most organisations have policies, committees and vendor reviews but not accountable roles, decision rights and escalation pathways as an operating model (source: https://govagentic.ai/insights/2026-07-16-ai-governance-operating-model, Jul 2026)

### memory-2026-07-01
- Claim: A data-protection authority (EU DPA or state AG) issues formal guidance or opens an inquiry specifically on persistent AI assistant memory by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://lumichats.com/blog/chatgpt-memory-vs-claude-memory-vs-gemini-personal-intelligence-2026-which-ai-actually-knows-you, 2026
- Status: open
- Grades:
 - none yet
 - 2026-08-04: open, no EU DPA or state AG action naming persistent assistant memory as its subject; the closest instrument is the 42-state AG subpoena of OpenAI (12 Jun 2026) covering user data, retention, health data and minors in general terms, and no EDPB or national DPA memory-specific guidance has issued, with resolve-by 2027-09 still ahead (source: https://www.reuters.com/business/openai-under-investigation-by-coalition-state-attorneys-general-wsj-reports-2026-06-12/, Jun 2026)
 - 2026-09-25: open, re-checked EU DPA, EDPB, Garante and state AG channels for 13 Aug to 25 Sep 2026 and found no action naming persistent assistant memory as its subject; the 42-state AG subpoena of OpenAI (Jun 2026) remains general in scope and the Italian ChatGPT file has passed to the Irish DPC as lead authority after the Rome tribunal annulled the Garante fine (Mar 2026), resolve-by 2027-09 (source: https://www.cnbc.com/2026/06/12/openai-says-its-engaging-constructively-with-state-ags-.html, Jun 2026)

### memory-2026-07-03
- Claim: A documented incident where leaked or subpoenaed assistant memory data causes material harm to a named individual surfaces by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://www.dume.ai/blog/top-10-ai-assistants-with-memory-in-2026, 2026
- Status: open
- Grades:
 - none yet
 - 2026-08-04: open, near misses but no match: the OpenMemory unauthenticated-memory-access CVEs and the MemGhost false-memory attack (Jul 2026) are vulnerabilities without a named victim, the Krafton Delaware opinion (Mar 2026) used chat logs rather than memory data and named no individual, and the Del Rosario case involved the memory feature working as designed rather than leaked or subpoenaed memory (source: https://thehackernews.com/2026/07/new-memghost-attack-plants-persistent.html, Jul 2026)
 - 2026-09-25: open, no documented case of leaked or subpoenaed assistant memory data harming a named individual surfaced; discovery and court-evidence coverage through Aug 2026 still concerns chat logs (the 20 million de-identified log order upheld 5 Jan 2026) rather than persistent memory entries, and no memory-layer vendor disclosed a breach, resolve-by 2027-09 (source: https://www.jdsupra.com/legalnews/when-chats-become-evidence-court-7484440/, Jan 2026)

### memory-2026-08-02
- Claim: OpenAI or Anthropic documents a deletion-propagation guarantee in official help documentation, stating that deleting a source conversation also deletes the memories derived from that conversation.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-06)
- Source: https://www.techtimes.com/articles/317840/20260605/chatgpt-memory-dreaming-update-openai-rewrites-personalization-engine-limits-audit-trail.htm, Jun 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, counter-signal hardened: both named vendors now document the negation, Claude's help centre stating that when a conversation expires or is deleted related memory entries are not removed, and OpenAI's Memory FAQ stating that deleting a chat does not necessarily delete a saved memory created from it; no guarantee documented, but documentation can still change before 2027-06 (source: https://support.claude.com/en/articles/11817273-use-claude-s-chat-search-and-memory-to-build-on-previous-context, Sep 2026)

### memory-2026-08-03
- Claim: The Model Context Protocol publishes a specification release dated after 2026-07-28 that adds a memory or persistent-state primitive, as a spec section or an officially listed extension covering agent memory storage, transfer, or provenance.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-05)
- Source: https://blog.modelcontextprotocol.io/posts/2026-07-28/, Jul 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, no MCP specification release after 2026-07-28 (GitHub releases list checked), no memory or persistent-state extension among the org's ext- repositories, and the 22 Aug 2026 roadmap post omits memory entirely while restating that protocol-level sessions were removed so servers hold no state, a direction running against the claim (source: https://blog.modelcontextprotocol.io/posts/mcp-roadmap/, Aug 2026)

### memory-2026-08-04
- Claim: A named enterprise memory-layer vendor (Mem0, Letta, Zep, Supermemory, or Engram) publicly discloses a security incident involving unauthorised access to customer memory stores in a production or hosted deployment, or CISA adds a memory-layer component CVE to the Known Exploited Vulnerabilities catalog.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-06)
- Source: https://nvd.nist.gov/vuln/detail/CVE-2026-59705, Jul 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, no memory-store security incident disclosed by Mem0, Letta, Zep, Supermemory or Engram, their GitHub advisory lists are empty for the window, and CISA KEV additions from 17 Aug to 25 Sep 2026 include no memory-layer component (the nearest AI-stack entries are MLflow, Ray and LiteLLM) (source: https://www.cisa.gov/sites/default/files/feeds/known_exploited_vulnerabilities.json, Sep 2026)

### memory-2026-08-05
- Claim: Anthropic documents agent memory store content in the Claude Compliance API, as a retrieval or deletion endpoint covering memory stores or memory entries, in the platform compliance documentation or the platform release notes.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-02)
- Source: https://platform.claude.com/docs/en/manage-claude/compliance-content-data, Aug 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, the Compliance API reference lists chats, files, generated files, projects, artifacts and local and remote session endpoints with no memory endpoint, and platform release notes through 24 Sep 2026 extend compliance coverage to Claude in Chrome, Claude Science and Office agent transcripts but not to memory stores (source: https://platform.claude.com/docs/en/api/compliance/apps, Sep 2026)

### memory-2026-08-06
- Claim: AWS publishes a further GitHub security advisory for the strands-agents-tools package affecting one of its memory tools (agent_core_memory, mem0_memory, mongodb_memory or elasticsearch_memory).
- Horizon: 0–12 months (logged 2026-08, resolve by 2026-12)
- Source: https://github.com/strands-agents/tools/security/advisories, Aug 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, one further strands-agents/tools advisory was published in the window (GHSA-qc8m-4887-8wwh, 25 Aug 2026) but it concerns the python_repl consent gate, not a memory tool, so the memory-scoped count stays at two with resolve-by 2026-12 (source: https://github.com/strands-agents/tools/security/advisories, Sep 2026)

### memory-2026-08-07
- Claim: Letta (letta-ai/letta) or LangMem (langchain-ai/langmem) publishes a GitHub security advisory concerning unauthorised cross user, cross agent or cross tenant access to stored memory.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-02)
- Source: https://github.com/letta-ai/letta/security/advisories, Aug 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, letta-ai/letta and langchain-ai/langmem still show zero published GitHub security advisories as queried through the GitHub API on 2026-09-25 (source: https://github.com/letta-ai/letta/security/advisories, Sep 2026)

### memory-2026-08-08
- Claim: Anthropic replaces the manual copy and paste memory export flow with a structured memory export, a downloadable file produced from settings or the account data export flow, documented in the Claude help centre.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-03)
- Source: https://support.claude.com/en/articles/12123587-import-and-export-your-memory-from-claude, Aug 2026
- Status: open
- Grades:
  - none yet
  - 2026-09-25: open, the Claude help centre export flow is unchanged: export still means asking Claude to write out memories verbatim and copying the text into a local file, and import is still described as experimental and in active development (source: https://support.claude.com/en/articles/12123587-import-and-export-your-memory-from-claude, Sep 2026)

## Resolved claims

### memory-2026-08-01
- Claim: A major agent or assistant platform (OpenAI, Anthropic, Microsoft, or OpenClaw) ships a user-visible memory-write provenance or confirmation control, documented in official product or developer documentation, showing the originating source of each persistent memory entry and/or requiring explicit confirmation before an agent writes to persistent memory.
- Horizon: 0–12 months (logged 2026-08, resolve by 2027-04)
- Source: https://thehackernews.com/2026/07/new-memghost-attack-plants-persistent.html, Jul 2026
- Status: confirmed
- Grades:
  - none yet
  - 2026-08-13: confirmed, Microsoft already ships an explicit confirmation control before persistent memory writes and documents it officially: the Visual Studio Copilot Memories post (15 Jan 2026) states that whenever Copilot is ready to save a new memory or update an existing one the user gets a confirmation nudge to review, accept or adjust before preferences are updated, and the Microsoft 365 Copilot memory support page states that Copilot asks the user whether to save information it judges worth remembering; the qualifying documentation predates the claim's own 2026-08 logging month by roughly seven months, so this confirmation measures retrieval coverage rather than foresight (CAL-004) (source: https://devblogs.microsoft.com/visualstudio/copilot-memories/, Jan 2026)

### memory-2026-07-02
- Claim: Memory portability becomes product: a major assistant vendor ships native memory export/import compatible with a competitor, or an open memory-exchange format gains two major implementations, by mid-2027.
- Horizon: 0–12 months (logged 2026-07, resolve by 2027-09)
- Source: https://plurality.network/blogs/best-universal-ai-memory-extensions-2026/, 2026
- Status: confirmed
- Grades:
 - none yet
 - 2026-08-04: confirmed, and confirmed by events that predate the claim being logged: Anthropic shipped native Claude memory import and export across providers (2 Mar 2026, documented in Claude's own help centre) and Google shipped Gemini Import Memory and Import Chat History from ChatGPT and Claude (26 Mar 2026), so two major assistant vendors already ship competitor-compatible memory portability (source: https://support.claude.com/en/articles/12123587-import-and-export-your-memory-from-claude, Aug 2026; https://9to5mac.com/2026/03/02/free-claude-users-can-now-use-memory-and-import-context-from-rivals/, Mar 2026)

### memory-2026-02-01
- Claim: Bounded AI-assisted workflows expand with stronger pre-deployment control checks in higher-impact contexts.
- Horizon: 0–12 months (logged 2026-02, resolve by 2027-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: confirmed
- Grades:
 - 2026-07: confirmed, 80.9% of technical teams past planning into agent testing/deployment with productized control patterns, though containment controls (37-40%) lag adoption; claim vague enough to be near-unfalsifiable (source: https://www.okta.com/newsroom/articles/ai-agents-at-work-2026-agentic-enterprise-security/, 2026)

### memory-2026-02-02
- Claim: Governance and legal teams gain earlier authority in implementation and procurement decisions.
- Horizon: 0–12 months (logged 2026-02, resolve by 2027-02)
- Source: none, seeded from pre-ledger 2026-02 run (method v1, ungrounded)
- Status: confirmed
- Grades:
 - 2026-07: confirmed, procurement routinely requires governance evidence and audit rights; 77% of orgs building formal AI governance programs; same vagueness caveat (source: https://prefactor.tech/learn/ai-governance-compliance-statistics, 2026)
