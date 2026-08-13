# Signal grading, identity, 2026-08-13

Scorecard:
- open: 6, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- unchanged since 2026-08-04 (not re-graded): 6

Scope note: the previous grading pass ran on 2026-08-04, nine days ago. No open
claim's resolve-by month has arrived, and research found no evidence dated after
2026-08-04 that materially moves any claim. The ledger was therefore not touched
this pass. Every claim below was researched; none earned a grade line.
Two further entries still listed under "Open claims" in the ledger,
identity-2026-02-03 and identity-2026-02-04, are retired method-v1 seed claims
and were not re-graded, per the method note that from 2026-08 only claims logged
under method v2 are graded.

Grade Details:
- identity-2026-07-01: open (unchanged, no ledger append), no named bank or payment network has publicly deprecated voice or video verification. Trade coverage in the window describes a layered retreat rather than a deprecation event: roughly 91 percent of US banks are reconsidering voice biometrics while moving to FIDO2 passkeys, synthetic-speech classifiers and liveness checks alongside voice rather than announcing its retirement. Resolve-by is 2027-09 (source: https://www.bankinfosecurity.com/ai-deepfakes-push-banks-beyond-voice-authentication-a-32388, Aug 2026)
- identity-2026-07-03: open (unchanged, no ledger append), no data-protection authority has opened a formal inquiry framed around persistent AI memory profiles. The nearest motion remains the Belgian APD conversational-app investigation already recorded on 2026-08-04, plus the EU AI Act chatbot transparency obligations that became enforceable on 2 Aug 2026, which are a disclosure duty rather than a memory-profile inquiry. The Italian Garante's earlier ChatGPT decision was annulled by the Court of Rome in Mar 2026, which weakens rather than advances the enforcement channel. Resolve-by is 2027-09 (source: https://www.mydatapath.com/news/compliance-news-2026-08-05/, Aug 2026)
- identity-2026-08-01: open (unchanged, no ledger append), the OpenID Foundation member vote is scheduled for 16 to 30 Sep 2026 and has not begun. The Foundation's news feed carries nothing on the Ephemeral Subject Identifier after the 17 Jul 2026 public-review announcement. Nothing is gradeable before the vote window closes; resolve-by is 2026-11 (source: https://openid.net/news/, Aug 2026)
- identity-2026-08-02: open (unchanged, no ledger append), no consolidated MCP interoperability results have been published and no participant vendors are named publicly. Research did surface the event's internal schedule, which was not in the ledger claim: implementers had to commit by 10 Aug 2026, must demonstrate at least one successful cross-partner test by 16 Oct 2026, and results are to be presented by OIDF and Gartner at the Gartner Identity and Access Management Summit. That schedule is consistent with the claim's 2027-01 resolve-by but does not resolve it (source: https://openid.net/call-for-participation-demonstrate-mcp-based-ai-agent-security-with-open-identity-standards-2/, Jul 2026)
- identity-2026-08-03: open (unchanged, no ledger append), Okta Agent Gateway is still offered as a request-access research release. The Okta "What's New in Okta for AI Agents" page carries July 2026 entries for other capabilities (agent-to-agent connections, import integrations) and no Agent Gateway general-availability entry. Resolve-by is 2027-03 (source: https://support.okta.com/help/s/article/what-s-new-in-okta-for-ai-agents, Aug 2026)
- identity-2026-08-04: open (unchanged, no ledger append), the EDPB draft guidelines on anonymisation (adopted Jul 2026 plenary) and on web scraping for generative AI (Guidelines 03/2026) remain in public consultation until 30 Oct 2026, so no final version can exist yet. Resolve-by is 2027-06 (source: https://www.edpb.europa.eu/public-consultations/guidelines-032026-on-web-scraping-in-the-context-of-generative-ai_en, Jul 2026)

Surprises:
- A nine-day interval produced zero gradeable movement across six open claims, which is the expected result and worth recording as a baseline. It also exposes a scheduling mismatch: four of the six claims (identity-2026-08-01 through 04) were logged with resolution events that are calendared for Sep 2026 through Jun 2027, so any grading pass before those dates can only restate the calendar. The value of a mid-month pass on this theme is close to zero.
- identity-2026-07-01's failure mode is sharpening rather than resolving. The August coverage shows the substantive prediction (voice trust collapsing for high-value transactions) is broadly correct while the claim's chosen observable, a public deprecation announcement, remains something institutions actively avoid doing. This is a second consecutive pass where the mechanism moves and the observable does not, which raises the odds of an `expired` grade at 2027-09 despite a directionally right thesis.
- CAL-004 (retrodiction risk) reads differently for this theme's newest claims. identity-2026-08-01 through 04 are all anchored to future-dated, calendared institutional events rather than to conditions already in the public record, so they are structurally immune to the retrodiction failure that produced identity-2026-07-02's discounted confirmation. The correction from the previous pass appears to have taken hold in Phase B's claim writing.
