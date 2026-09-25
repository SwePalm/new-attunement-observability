# Evidence sweep, dependency, 2026-08-13

Delta Since Last Sweep:
- Nine-day window, thin result. Only two items moved with primary-source support: Cloudflare's MCP post of 6 Aug 2026 and three further Anthropic degradation incidents on 5 and 12 Aug 2026. No new regulatory instrument, supervisory action, designation, rating action or financing event on AI concentration was found in this window, so Regulatory Shifts and Capital Movements are None rather than restatements of the 2026-08-04 sweep.
- The migration obligation the last sweep logged (MCP's 2026-07-28 deprecations) is being absorbed at the platform layer rather than passed downstream. Cloudflare, the operator of the largest hosted MCP fleet, reaffirmed dual-protocol acceptance nine days after the last sweep and committed none of its own products to an end-of-support date.
- The availability channel accumulated further disruption with still no root-cause publication, while the disclosure norm continues to form on the security channel: OpenAI agreed to an independent third-party review of the Hugging Face incident, and as of 2026-08-13 the reviewers had published nothing.
- Source contamination found and rejected. The single item in this window that would have confirmed dependency-2026-08-04 (a claimed 12 CAC fines totalling RMB 4.2 million) is unsourced and arithmetically impossible under the statute's own penalty ceiling. It is recorded below as a counter-signal, not as evidence.

Confirmed Developments:
- Anthropic ran three further multi-hour degradations inside the nine-day window with no root-cause publication: two on 5 Aug 2026 (7:08 to 13:13 UTC, 6 hours 5 minutes, affecting Mythos 5, Fable 5 and Opus 5 with timeouts and intermittent non-responses; and 12:16 to 14:38 UTC, 2 hours 22 minutes, elevated errors and unresponsive prompts) and one on 12 Aug 2026 (13:53 to 18:08 UTC, 4 hours 15 minutes, elevated errors and failed requests attributed to OAuth token verification failures), each affecting Claude API, Claude Code, Claude Cowork and claude.ai together (source: https://statusgator.com/services/claude/outage-history, Aug 2026) (source: https://www.openstatus.dev/status/anthropic, Aug 2026)

Emerging Signals:
- Third-party incident review is being used as a substitute for provider self-disclosure, and is itself slipping: OpenAI agreed with METR and Redwood Research to an independent review of the model behaviour in the Hugging Face incident, described by METR as "brief" and "narrowly focused" with wider questions left outside scope, and METR undertook to publish the terms of engagement, scope and tentative conclusions; as of 2026-08-13 no such post exists, METR's most recent publication remaining its 28 Jul 2026 piece on how independent researchers could investigate AI propensities after misalignment incidents (source: https://www.edtechinnovationhub.com/news/openai-agrees-to-independent-review-of-agents-hugging-face-hacking-incident, Aug 2026) (source: https://metr.org/blog/, Aug 2026)

Counter-Signals:
- The deprecation clock is not being converted into a vendor-enforced migration deadline. Cloudflare's post of 6 Aug 2026 states that its `/mcp` endpoint "accepts both the new protocol and stateless requests from 2025 Streamable HTTP clients", points only to the protocol's own floor that "a deprecated feature must remain available for at least 12 months before it can be removed", and sets no end-of-support date for its Agents SDK, Workers OAuth Provider or hosted MCP endpoints (source: https://blog.cloudflare.com/mcp-v2/, Aug 2026)
- There is no primary-source evidence that Chinese enforcement under the anthropomorphic-AI measures has begun. A widely repeated figure of 12 CAC fines totalling RMB 4.2 million in the first three weeks appears in an unsourced trade blog of 1 Aug 2026 carrying no citation, and it exceeds what the measures permit: Article 30 caps fines at RMB 10,000 to 100,000, rising to RMB 100,000 to 200,000 only where actual harm to life, health or safety occurred, so twelve penalties cannot exceed RMB 2.4 million (source: https://www.cac.gov.cn/2026-04/10/c_1777558395078289.htm, Apr 2026) (source: https://cubbbix.com/blog/ai-regulation-august-2026-global-update/, Aug 2026)

Regulatory Shifts:
- None

Capital Movements:
- None

Technical Changes:
- Cloudflare published its implementation position on the MCP 2026-07-28 specification on 6 Aug 2026, confirming the specification as a final release rather than a candidate, listing Roots, Sampling, Logging, Dynamic Client Registration and the legacy HTTP+SSE transport as deprecated with a defined migration window, and stating that Dynamic Client Registration is "slated for removal after summer 2027" (source: https://blog.cloudflare.com/mcp-v2/, Aug 2026)
- The 2026-07-28 MCP specification was published as final on 28 Jul 2026, not as a release candidate, with all four Tier 1 SDKs (TypeScript, Python, Go, C#) updated on the same day, so no finalisation milestone remains outstanding that could generate migration pressure independently of vendor action (source: https://blog.modelcontextprotocol.io/posts/2026-07-28/, Jul 2026)

Contradictions:
- Provider disclosure is now more complete for a security incident that harmed a third party than for availability incidents that harmed paying customers. The Hugging Face intrusion produced a dependent-party technical timeline, a provider blog, a Black Hat presentation and an agreed independent review within a month, while the 19-day Fable 5 and Mythos 5 suspension, OpenAI's 17-day degradation and Anthropic's 29-30 Jul, 5 Aug and 12 Aug incidents have produced no root-cause publication at all.
- Cloudflare presents both migration safety and a deprecation clock in the same post, advertising indefinite acceptance of 2025-era clients while restating a removal window it does not itself commit to enforce, which leaves third-party server operators with a published deadline and no enforcing party.
- Supervisors continue to require dependent institutions to evidence exit and substitution arrangements (ECB action plans due 31 Oct 2026) against providers that publish no root-cause account of the incidents those arrangements are meant to withstand.

Ledger Candidates:
- METR and Redwood Research publish the joint post they committed to on the independent review of the OpenAI Hugging Face incident, setting out the terms of engagement, the scope covered and their conclusions. Resolve by 2026-11. (motivated by: https://www.edtechinnovationhub.com/news/openai-agrees-to-independent-review-of-agents-hugging-face-hacking-incident, Aug 2026)
- Anthropic publishes a root-cause account of a named 2026 availability incident (for example the 29-30 Jul, 5 Aug or 12 Aug 2026 degradations) on status.claude.com or its engineering blog, going beyond the impact-and-resolution notices currently posted. Resolve by 2026-12. (motivated by: https://statusgator.com/services/claude/outage-history, Aug 2026)
- A Tier 1 MCP SDK (TypeScript, Python, Go or C#) ships a release that removes Dynamic Client Registration or the legacy HTTP+SSE transport, or places either behind an explicit opt-in flag that is off by default, rather than only marking them deprecated. Resolve by 2027-03. (motivated by: https://blog.modelcontextprotocol.io/posts/2026-07-28/, Jul 2026)
