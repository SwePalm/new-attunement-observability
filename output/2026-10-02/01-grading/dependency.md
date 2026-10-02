# Signal grading, dependency, 2026-10-02

Scorecard:
- open: 9, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- live method-v2 claims graded: 9 (dependency-2026-07-03, -08-01, -08-02, -08-03, -08-04, -08-06, -09-01, -09-02, -09-03)
- forward confirmations: 0; retrodicted confirmations: 0

Scope notes:
- The retired 2026-02 seed claims (dependency-2026-02-03 and -02-04 in Open claims) were excluded: not researched, not graded, not counted, left untouched.
- dependency-2026-07-01, -07-02, -08-05 and -08-07 were already resolved (confirmed) and were not re-graded.
- Only about 7 days passed since the 2026-09-25 pass, so most claims were expected to stay open. Each live claim got one appended grade line dated 2026-10-02. No claim moved to Resolved claims.
- Sources checked: OpenAI deprecations page (developers.openai.com), Anthropic status API and engineering blog index, pingoru incident mirror, law-firm and press coverage of the UK CTP designations, FSB consultation coverage, ESA DORA list coverage, news.cn and CAC-related Chinese search results.
- Not opened: openai.com pages (GPT-5.5 retirement was checked via secondary coverage only); fsb.org publications index was not re-fetched, so "final report not yet published" rests on search results that still describe an October 2026 target.

Grade Details:
- dependency-2026-07-03: open. No provider or affected-enterprise post-mortem found for the Fable 5 and Mythos 5 suspension or OpenAI's July degradation. Anthropic status incidents of 29 Sep and 1 Oct 2026 are resolution-only.
- dependency-2026-08-01: open. Coverage (Mofo, Lewis Silkin, Jul 2026) still lists only AWS, Google Cloud, Microsoft and Oracle as CTPs. No later designation found. (source: https://www.mofo.com/resources/insights/260716-uk-announces-list-of-first-critical-third-parties, Jul 2026)
- dependency-2026-08-02: open. The final FSB report is still described as due October 2026; none found yet. The 10 Jun consultation already lists supply chain concentration in its third-party practice, so the final text should be graded as soon as published (literal-text risk: the claim asks for more than the consultation's generic framing). This is the most likely claim to resolve next run.
- dependency-2026-08-03: open. No dated end-of-support from a platinum member after the 2026-07-28 spec; only non-member notices (Keboola, Atlassian) surfaced.
- dependency-2026-08-04: open. Chinese-language search found only the measures' penalty gradation (warning up to CNY 10,000–200,000 fines) and no enforcement action naming a provider. (source: https://www.cac.gov.cn/2026-04/10/c_1777558395023172.htm, Apr 2026)
- dependency-2026-08-06: open. Status API newest incidents (29 Sep, 1 Oct) have no root cause; the engineering blog index lists only the 23 Apr 2026 Claude Code account. A webpronews article claims Anthropic issued a blog post-mortem about 25 Jun 2026 for a 23 Jun outage. I could not corroborate this at Anthropic's own pages (status API holds only Aug 2026 onward incidents; engineering index has no such post), the outlet looks low-reliability, and the event would predate the claim's logging (retrodiction) and not be one of the claim's example incidents, though "a named 2026 availability incident" is literally open-ended. Left open; worth a direct check of anthropic.com/news at the next pass.
- dependency-2026-09-01: open. 14 Oct 2026 retirement not yet reached; no postponement or restoration reported in newsbytes, borncity or aiidelist coverage.
- dependency-2026-09-02: open. The deprecations page shows notices dated 1 Oct 2026 with shutdowns 1 Apr 2027 and 6 Jan 2027, both well beyond 30 days. (source: https://developers.openai.com/api/docs/deprecations, Oct 2026)
- dependency-2026-09-03: open. Only the 19 Nov 2025 first DORA CTPP list (19 providers, none a foundation-model API provider) found; no second list. (source: https://www.esma.europa.eu/press-news/esma-news/european-supervisory-authorities-designate-critical-ict-third-party-providers, Nov 2025)

Qualifying Events:
- None this run. No event resolved any claim in this theme.

Surprises:
- None. A uniformly open scorecard fits the 7-day interval. The one anomaly is an uncorroborated secondary-source claim of a June 2026 Anthropic post-mortem, which may indicate another CAL-004-style negative stated without checking Anthropic's own news feed.

Calibration Observations:
- CAL-007 re-confirmation: dependency-2026-08-01 and -08-02 are blocked by institutional calendars (HM Treasury end-2026, FSB October 2026), not by world change.
- CAL-004 watch: dependency-2026-08-06 states a negative (no Anthropic root-cause account) that rests on the status page and engineering index only; Anthropic's news/blog feed was not checked. Treat as unverified until it is.
- CAL-005: openai.com unreachable for primary confirmation of GPT-5.5 plans (dependency-2026-09-01); no negative was inferred from it beyond "no postponement reported".
