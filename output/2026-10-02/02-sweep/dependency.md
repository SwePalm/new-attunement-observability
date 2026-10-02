# Evidence sweep, dependency, 2026-10-02

Delta Since Last Sweep:
- Forced migration moved back to the model-ID level at Anthropic. On 30 Sep 2026 Anthropic notified developers that claude-sonnet-4-5-20250929 is deprecated with retirement on 30 Nov 2026 (61 days), about 12 months after its 29 Sep 2025 release. The 2026-09-25 sweep's Counter-Signal that every model released since mid-2025 was still Active no longer holds (source: https://platform.claude.com/docs/en/about-claude/model-deprecations, Sep 2026)
- OpenAI posted two further deprecations dated 1 Oct 2026: gpt-5.3-codex, gpt-5.4-nano and gpt-5.1 leave the API on 1 Apr 2027 (six months), and four text-to-speech models leave on 6 Jan 2027 (at least three months). Neither is a short-notice case, so the 9x notice-period spread recorded on 2026-09-25 stands with a 20-day low of 11 Sep (source: https://developers.openai.com/api/docs/deprecations, Oct 2026)
- Google reversed a scheduled shutdown on one channel only. The Gemini Developer API deprecations page (last updated 1 Oct 2026) now lists "No shutdown date announced" for gemini-2.5-pro, gemini-2.5-flash and gemini-2.5-flash-lite and says they "will continue to be served until further notice", where a 16 Oct 2026 date was cited in July. Vertex AI still lists 20 Oct 2026 for the same models (source: https://ai.google.dev/gemini-api/docs/deprecations, Oct 2026) (source: https://docs.cloud.google.com/vertex-ai/generative-ai/docs/learn/model-versions, Oct 2026)
- Pre-window item missed by earlier dependency sweeps: on 28 Aug 2026 OpenAI told Cursor it will end Cursor's access to its models on 12 Nov 2026 after SpaceX's acquisition of Cursor's parent. It is the first recorded case in this ledger of a provider cutting a named downstream customer for ownership reasons, and the cutoff is still ahead. Listed as context, not as a new-window event (source: https://bdtechtalks.com/2026/09/04/openai-cursor-ban/, Sep 2026) (source: https://www.marketscale.com/industries/software-and-technology/chatgpt-claude-and-grok-went-down-together-and-continuity-planning-just-got-real, Sep 2026)

Confirmed Developments:
- Google's two channels for the Gemini 2.5 family now disagree. The Gemini Developer API page (last updated 1 Oct 2026) shows no shutdown date for gemini-2.5-pro, 2.5-flash and 2.5-flash-lite and calls them "not deprecated", while access is limited to projects that used them before. The Vertex AI model-versions page lists 20 Oct 2026 for the same three models, and only gemini-2.5-flash-image has a fixed shutdown of 2 Oct 2026 on the Developer API (source: https://ai.google.dev/gemini-api/docs/deprecations, Oct 2026) (source: https://docs.cloud.google.com/vertex-ai/generative-ai/docs/learn/model-versions, Oct 2026)
- OpenAI notified Cursor on 28 Aug 2026 that model access ends on 12 Nov 2026, citing doubt that SpaceX will use its technology within OpenAI's terms. Cursor's CEO put OpenAI models at about 5% of user traffic, Cursor said it was discussing the decision, and bring-your-own-key access remains possible but loses native features. The cutoff had not been reversed or confirmed completed in any source found (source: https://bdtechtalks.com/2026/09/04/openai-cursor-ban/, Sep 2026) (source: https://www.marketscale.com/industries/software-and-technology/chatgpt-claude-and-grok-went-down-together-and-continuity-planning-just-got-real, Sep 2026)

Emerging Signals:
- Claude availability incidents continue with impact-and-resolution text only. A Major incident on 29 Sep 2026 hit claude.ai, Claude Code, Claude Cowork and the API from 14:00 UTC, with a second sign-in failure and recovery by 14:59 UTC, and a Major model-error incident ran on 22 Sep 2026 (00:50 to 02:10 UTC). Neither carries a root-cause account, and no shared-cause explanation of the 3 Sep triple outage has appeared (source: https://status.claude.com/api/v2/incidents.json, Oct 2026)
- Lock-in framing now reaches practitioners as an operational checklist. A Cloud Security Alliance research note of 19 Sep 2026 on the 3 Sep outage recommends dependency inventories, synthetic monitoring of AI endpoints, multi-provider gateways and incident-notification clauses in vendor contracts. It cites the IBM survey figure that 91% of executives do not fully understand their AI dependencies (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-triple-ai-outage-concentration-risk-202609/, Sep 2026)
- German-language coverage carries the same survey into a sovereignty argument. Business Punk's piece of 22 Jun 2026 on the IBM Institute for Business Value and Oxford Economics study says 81% of firms would face severe disruption from a one-week provider outage and 71% find switching difficult (non-English source, pre-window background) (source: https://www.business-punk.com/tech/grosser-ki-blackout-warum-81-prozent-der-firmen-zittern/, Jun 2026)

Counter-Signals:
- Google's removal of the Developer API shutdown date for Gemini 2.5 is a forced-migration reversal, even if partial. Users are told the models "will continue to be served until further notice", though restricted to existing users, and the Vertex channel did not follow in the pages checked (source: https://ai.google.dev/gemini-api/docs/deprecations, Oct 2026)
- Anthropic's Sonnet 4.5 notice kept to its stated 60-day minimum floor (61 days) and the deprecations page still carries floors of not sooner than 1 Sep 2027 for the newest Mythos and Fable models, so the cadence stays slower than OpenAI's short-notice cases (source: https://platform.claude.com/docs/en/about-claude/model-deprecations, Sep 2026)

Regulatory Shifts:
- None

Capital Movements:
- None

Technical Changes:
- OpenAI deprecated gpt-5.3-codex, gpt-5.4-nano and gpt-5.1 on 1 Oct 2026 for removal on 1 Apr 2027, and tts-1, tts-1-hd and two gpt-4o-mini-tts snapshots for removal on 6 Jan 2027, with gpt-realtime-2.1-mini as replacement (source: https://developers.openai.com/api/docs/deprecations, Oct 2026)
- Anthropic deprecated claude-sonnet-4-5-20250929 on 30 Sep 2026 with retirement on 30 Nov 2026 and claude-sonnet-5-5 as replacement. claude-opus-4-5-20251101 (floor 24 Nov 2026) and claude-haiku-4-5-20251001 (floor 15 Oct 2026) are listed Active (source: https://platform.claude.com/docs/en/about-claude/model-deprecations, Oct 2026)
- OpenAI released GPT-6.1 Sol on 29 Sep 2026 and moved Computer Use into the Agents API, which extends the managed-runtime pattern from 10 Sep. GPT-6 Astra's new Ultrafast mode lacks EU regional inference (source: https://developers.openai.com/api/docs/changelog, Sep 2026)

Contradictions:
- The 2026-09-25 sweep's Counter-Signal that every Anthropic model released since mid-2025 is still Active is superseded by the 30 Sep 2026 Sonnet 4.5 deprecation.
- Third-party calendars lag Google's own pages. Vorp Labs' snapshot of 7 Sep 2026 lists 16 Oct 2026 for Gemini 2.5, a date the Developer API page no longer shows, and flags a conflicting 20 Oct on Vertex. A Firebase doc page says 2.5 models "will shut down for all projects in October 2026" on the Agent Platform API. Which date a given customer faces depends on channel and is not settled. (Unverified: undated Firebase page; Vorp Labs is a secondary aggregator.)
- Unverified: several secondary pages (aiweekly.co on Sonnet 4.5, kingy.ai on Gemini 2.5 Pro, CNBC on Cursor) returned HTTP 403 and were not opened. A Retell deprecation page for Sonnet 4.5 and a DevOps.com Cursor story returned 404. Nothing from them was used.

Ledger Candidates:
- OpenAI and Cursor (or SpaceX on Cursor's behalf) publicly announce an agreement, extension or reversal that keeps OpenAI first-party models available inside Cursor beyond 12 Nov 2026 (beyond BYOK), by 2026-11.
 Not yet true as of 2026-10-02: no extension or reversal found; the 12 Nov 2026 cutoff stands and Cursor says only that it is discussing it (source: https://bdtechtalks.com/2026/09/04/openai-cursor-ban/, Sep 2026)
- Google's Vertex AI / Gemini Enterprise Agent Platform model-versions page (docs.cloud.google.com) replaces the 20 Oct 2026 retirement date for gemini-2.5-pro with a later date or "no shutdown date announced", by 2026-11.
 Not yet true as of 2026-10-02: the Vertex page lists 20 Oct 2026 for gemini-2.5-pro, 2.5-flash and 2.5-flash-lite, while the Developer API page already shows none (source: https://docs.cloud.google.com/vertex-ai/generative-ai/docs/learn/model-versions, Oct 2026)
- Anthropic marks claude-haiku-4-5-20251001 or claude-opus-4-5-20251101 as Deprecated, with a dated retirement, on its model-deprecations page, by 2026-12. Sonnet 4.5 was notified the day after its stated 29 Sep floor, which makes the 15 Oct (Haiku) and 24 Nov (Opus) floors live.
 Not yet true as of 2026-10-02: both models are listed Active with tentative retirement floors of 15 Oct 2026 and 24 Nov 2026 (source: https://platform.claude.com/docs/en/about-claude/model-deprecations, Oct 2026)

Dedupe: no candidates dropped; all appended.
