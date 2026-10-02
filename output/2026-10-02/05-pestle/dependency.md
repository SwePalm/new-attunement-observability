# PESTLE analysis, dependency, 2026-10-02

Sources are the 2026-10-02 sweep unless marked as ledger or grading provenance. Items marked "inference" are not in any source.

### Political
Core Shift Thesis:
Supervisors have named single-provider dependence as a risk but have not yet drawn model providers into their perimeters, so the politics of continuity is conducted through provider deprecation pages and one-off bilateral decisions rather than through public rules.

Forces:
1. The UK Critical Third Parties regime holds only four designated cloud providers (AWS, Google Cloud, Microsoft, Oracle) after the 10 Jul 2026 announcement, and the Treasury Committee's end-of-2026 recommendation for further designations is unmet (ledger dependency-2026-08-01, open; grading file 2026-10-02; source: https://www.mofo.com/resources/insights/260716-uk-announces-list-of-first-critical-third-parties, Jul 2026). On the record of slipping regulatory calendars, a model provider designation inside the horizon is a minority outcome (inference).
2. The European Supervisory Authorities' first DORA list of 19 critical ICT providers (19 Nov 2025) contains no foundation-model API provider and no second list or date has been announced (ledger dependency-2026-09-03, open; source: https://www.esma.europa.eu/press-news/esma-news/european-supervisory-authorities-designate-critical-ict-third-party-providers, Nov 2025).
3. The FSB's final Sound Practices for Responsible Adoption of AI is still described as due in October 2026, and its 10 Jun 2026 consultation already lists supply chain concentration inside its third-party practice, so the open question is whether the final text names substitutability (ledger dependency-2026-08-02, open; grading file 2026-10-02).
4. State action can itself be the outage: Anthropic's 12 Jun 2026 suspension of Claude Fable 5 and Mythos 5 followed a US export-control directive, and no provider or affected enterprise post-mortem has been published since (ledger dependency-2026-07-03, open; source: https://www.gtlaw.com/en/insights/2026/6/ai-company-anthropic-suspends-access-to-claude-fable-5-claude-mythos-5-following-us-export-control-directive, Jun 2026).

### Economic
Core Shift Thesis:
The price of leaving is set by the calendar of the party being left, so a customer's cost of continuity depends on notice periods, ownership questions and channel choices that were not part of the purchase decision.

Forces:
1. Notice periods run on very different clocks: Anthropic notified Sonnet 4.5's retirement on 30 Sep 2026 with 61 days (retirement 30 Nov), against OpenAI's 1 Apr 2027 and 6 Jan 2027 removals notified on 1 Oct 2026, and a shortest recorded OpenAI notice of 20 days (11 Sep, per the 2026-09-25 sweep); the spread is about nine to one (source: https://platform.claude.com/docs/en/about-claude/model-deprecations, Sep 2026) (source: https://developers.openai.com/api/docs/deprecations, Oct 2026).
2. A provider can end access for a named customer for ownership reasons: OpenAI's 28 Aug 2026 notice to Cursor ends model access on 12 Nov 2026 after SpaceX's acquisition of Cursor's parent, and bring-your-own-key access remains but loses native features (source: https://bdtechtalks.com/2026/09/04/openai-cursor-ban/, Sep 2026). The Cursor chief executive's figure of about 5% of traffic shows that a well-hedged customer prices this as a small loss.
3. Consumer-facing retirements have dated cliffs of their own: OpenAI's 14 Oct 2026 retirement of GPT-5.5 in ChatGPT, ChatGPT Work and Codex has not been postponed in any coverage found (ledger dependency-2026-09-01, open; source: https://www.businesstoday.in/technology/artificial-intelligence/story/openai-to-retire-gpt-5-5-from-chatgpt-work-and-codex-on-october-14-what-changes-to-expect-555782-2026-09-16, Sep 2026).
4. A standing second provider is a recurring cost with no visible return until the day it is needed, so it competes with every other budget line; whether insurers or procurement scorecards begin to price exit readiness is an open question (inference).

### Social
Core Shift Thesis:
Exposure is widely felt and poorly mapped, and the people who carry it are practitioners who read notices on behalf of organisations whose leaders believe the current model simply works.

Forces:
1. The IBM Institute for Business Value and Oxford Economics study, as cited by the Cloud Security Alliance on 19 Sep 2026, finds 91% of executives do not fully understand their AI dependencies; the German-language account of 22 Jun 2026 adds that 81% of firms would face severe disruption from a one-week provider outage and 71% find switching difficult (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-triple-ai-outage-concentration-risk-202609/, Sep 2026) (source: https://www.business-punk.com/tech/grosser-ki-blackout-warum-81-prozent-der-firmen-zittern/, Jun 2026).
2. Checklist culture reaches the operations desk: the CSA note recommends dependency inventories, synthetic monitoring of AI endpoints, multi-provider gateways and incident-notification clauses, which gives staff something to do and, in inference, something to mistake for readiness.
3. Teams build tuned behaviour around a specific model identifier, so a retirement removes a known system and replaces it with an unknown one; the migration is felt as a loss before it is felt as an upgrade (inference).
4. Users of a cut-off product face a degraded alternative: Cursor users retain bring-your-own-key access but lose native features after 12 Nov 2026 (source: https://bdtechtalks.com/2026/09/04/openai-cursor-ban/, Sep 2026).

### Technological
Core Shift Thesis:
Dependence is deepening toward provider-managed runtimes while the portable layer, the protocol, is being actively pruned, so the cheap exit is getting narrower at the same time as the checklists say to build one.

Forces:
1. Provider channels disagree on the same model: Google's Gemini Developer API page (updated 1 Oct 2026) lists no shutdown date for Gemini 2.5 Pro, Flash and Flash-Lite, while the Vertex AI page lists 20 Oct 2026, and gemini-2.5-flash-image has a fixed 2 Oct 2026 shutdown (source: https://ai.google.dev/gemini-api/docs/deprecations, Oct 2026) (source: https://docs.cloud.google.com/vertex-ai/generative-ai/docs/learn/model-versions, Oct 2026).
2. OpenAI released GPT-6.1 Sol on 29 Sep 2026 and moved Computer Use into the Agents API, extending the managed-runtime pattern of 10 Sep; the new Ultrafast mode of GPT-6 Astra lacks EU regional inference (source: https://developers.openai.com/api/docs/changelog, Sep 2026).
3. The MCP specification of 28 Jul 2026 deprecated HTTP+SSE transport and Dynamic Client Registration, and the TypeScript SDK v2 (27 Jul 2026) removed the SSE server transport, leaving a frozen opt-in bridge package (ledger dependency-2026-08-07, confirmed; source: https://github.com/modelcontextprotocol/typescript-sdk/blob/main/docs/migration/upgrade-to-v2.md, Jul 2026). No platinum member has yet published a dated end-of-support (ledger dependency-2026-08-03, open).
4. Outage visibility is thin: Anthropic's status API shows a Major incident on 29 Sep 2026 and a model-error incident on 22 Sep, each with impact-and-resolution text only, which pushes customers toward their own synthetic monitoring (source: https://status.claude.com/api/v2/incidents.json, Oct 2026).

### Legal
Core Shift Thesis:
The binding instruments that govern continuity are mostly contracts and terms of service, with regulatory guidance arriving as expectation rather than duty, so rights to notice and to exit assistance are what a customer negotiates rather than what it is owed.

Forces:
1. APRA's 30 Apr 2026 letter to all APRA-regulated entities found heavy dependence on a single AI provider across several use cases with untested exit strategies and set an expectation of active management of concentration risk; it is guidance, not a binding duty (ledger dependency-2026-07-01, confirmed; source: https://www.apra.gov.au/apra-letter-to-industry-on-artificial-intelligence-ai, Apr 2026).
2. Terms of service function as the legal ground for cutoffs: OpenAI cited doubt that SpaceX would use its technology within OpenAI's terms when ending Cursor's access (source: https://bdtechtalks.com/2026/09/04/openai-cursor-ban/, Sep 2026).
3. Region-specific legal regimes force region-specific rebuilds: China's anthropomorphic-AI measures took effect on 15 Jul 2026 and led ByteDance and Alibaba to withdraw and rebuild companion features by region, while no enforcement action naming a provider has been published (ledger dependency-2026-02-03 and dependency-2026-08-04, open; source: https://english.news.cn/20260715/4bf39cb3c4db42babc10ed37932cfd94/c.html, Jul 2026).
4. Incident-notification clauses and exit-assistance terms are the contractual tools the CSA note recommends; whether providers concede them at standard-contract scale is not observed in the sweep (inference).

### Environmental
Core Shift Thesis:
Dependence has a physical geography of regions, shared hosting and capacity, and when that geography fails or is rationed the failure arrives at several providers at once.

Forces:
1. The 3 Sep 2026 triple outage took ChatGPT, Claude and Grok down together, and no shared-cause explanation has appeared; a common infrastructure layer is a hypothesis, not a finding (source: https://www.marketscale.com/industries/software-and-technology/chatgpt-claude-and-grok-went-down-together-and-continuity-planning-just-got-real, Sep 2026).
2. The UK designations list four cloud providers whose regions carry the model services, so concentration at the hosting layer is already inside the supervisory perimeter while concentration at the model layer is not (ledger dependency-2026-08-01, open; source: https://www.mofo.com/resources/insights/260716-uk-announces-list-of-first-critical-third-parties, Jul 2026).
3. Regional availability is a capacity decision: GPT-6 Astra's Ultrafast mode launched without EU regional inference (source: https://developers.openai.com/api/docs/changelog, Sep 2026), so a customer with a data-location obligation can be unable to adopt the faster mode.
4. Capacity is finite, and keeping retired generations running competes with serving newer ones; retirement schedules may partly reflect that allocation (inference, no source in the sweep).
