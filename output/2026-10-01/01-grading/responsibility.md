# Signal grading, responsibility, 2026-10-01

Scorecard:
- open: 12, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- live method-v2 claims graded: 12 (responsibility-2026-07-03, responsibility-2026-08-01 to -08-06, responsibility-2026-08-08, responsibility-2026-09-01 to -09-04)
- retrodictions among non-open grades: 0 of 0

Scope notes:
- The retired method-v1 seed claims (responsibility-2026-02-03 and -02-04 parked under "Open claims", plus the resolved -02-01 and -02-02) were not researched, graded, counted or touched. responsibility-2026-08-07 is already resolved and was not re-graded.
- The last pass was 2026-09-25 (6 days ago). responsibility-2026-09-01 to -09-04 had never been graded, so this is their first pass. No claim has a resolve-by of 2026-09 or 2026-10, so none was eligible for `expired`.
- Ledger edits: one grade line appended per live claim; the `none yet` placeholder replaced by the grade line for -09-01 to -09-04. No claim moved.
- Unopened or unreliable pages: the San Francisco Superior Court register (webapps.sftc.org, HTTP 403 on the prior pass, not retried; affects -08-01 and -08-05); the CourtListener docket page (HTTP 403) and its API (returned unusable dates; affects -08-08); nysenate.gov via curl (HTTP 403, read through WebFetch instead); legiscan.com (HTTP 403); faz.net (fetch blocked; affects -09-03); justice.gov (not opened; affects -08-02). Per CAL-005 these open grades mean "not found", not "not happened".
- Source-reliability note: one WebFetch summary of nysenate.gov/legislation/bills/2025/S9051/amendment/B described S9051B as "signed by Governor". A second fetch of the main bill page returned the full action history ending at 5 Jun 2026 with no delivery, signature or chapter entry, and Pluribus News and the Transparency Coalition describe the bill as awaiting action. The first summary was treated as an error.

Grade Details:
- responsibility-2026-07-03: open, no new court decision applying component-part liability to a frontier model provider; JCCP 5431 only just opened discovery and Lawsuit Informer (30 Sep 2026) reports no ruling on OpenAI's liability (source: https://lawsuitinformer.com/openai-lawsuits, Sep 2026)
- responsibility-2026-08-01: open, no ruling on whether ChatGPT is a "product"; Case Management Order No. 2 (reported 30 Sep 2026) opened discovery, with amended complaints due 16 Nov and the next hearing on 13 Nov 2026 (source: https://lawsuitinformer.com/openai-lawsuits, Sep 2026)
- responsibility-2026-08-02: open, no new Task Force suit or intervention; the only September DOJ AI activity found was the 2 Sep 2026 fair-use statement of interest in New York Times v. OpenAI, which is not a state-law challenge (source: https://www.washingtonpost.com/technology/2026/09/02/doj-urges-judge-rule-openai-microsoft-ny-times-lawsuit/, Sep 2026 [discovery listing only, not opened])
- responsibility-2026-08-03: open, the Commission's AI Act policy page (news through 1 Oct 2026) lists no final Article 73 guidance or template (source: https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai, Oct 2026)
- responsibility-2026-08-04: open, no affirmative AI liability form from Verisk/ISO or a named top-10 US carrier; reporting still shows exclusions from the admitted market and affirmative cover from specialty players (source: https://vorplabs.com/ai-insurance-exclusions, Jul 2026)
- responsibility-2026-08-05: open, no OpenAI demurrer or equivalent is reported; responsive pleadings follow the 16 Nov 2026 amended complaints, and the court register could not be opened (source: https://lawsuitinformer.com/openai-lawsuits, Sep 2026)
- responsibility-2026-08-06: open, the NY Senate action history ends at passage on 5 Jun 2026 with no delivery to the Governor, signature or chapter; the deadline is 31 Dec 2026 (source: https://www.nysenate.gov/legislation/bills/2025/S9051, Oct 2026)
- responsibility-2026-08-08: open, no merits order since Amazon's 21 Sep 2026 amended complaint; the docket itself was not opened (HTTP 403), so this is "not found" (source: https://thenextweb.com/news/amazon-blocks-muse-perplexity-amended-complaint, Sep 2026)
- responsibility-2026-09-01: open, Amazon blocked Muse from amazon.com on 20 Sep 2026 citing its Conditions of Use, but no lawsuit against Meta was found; the block is the contractual and technical path, not litigation (source: https://gizmodo.com/amazon-brings-down-the-hammer-on-metas-muse-ai-agent-2000814878, Sep 2026)
- responsibility-2026-09-02: open, Alabama (subpoena, 24 Aug 2026) and a 15-state coalition remain at investigation stage; no civil enforcement action, settlement or assurance of voluntary compliance (source: https://www.insurancejournal.com/news/southeast/2026/08/26/882967.htm, Aug 2026)
- responsibility-2026-09-03: open, the bill had its first reading (4 Mar 2026) and committee hearing (13 Apr 2026); as of 25 Aug 2026 coverage, second and third readings had not occurred, and no promulgation was found (source: https://www.bundestag.de/ausschuesse/recht-verbraucherschutz/sitzungen/1156420-1156420, Apr 2026)
- responsibility-2026-09-04: open, Newsom signed AB 2 on 10 Sep 2026 (the trigger for a challenge), but no NetChoice complaint was found (source: https://www.gov.ca.gov/2026/09/10/governor-newsom-signs-the-strongest-child-safety-chatbot-and-social-media-laws-in-the-nation/, Sep 2026)

Qualifying Events:
- None. No event this run resolved any claim in any theme. Near-misses recorded for context only: Newsom's signing of AB 2 (10 Sep 2026) enables but does not satisfy responsibility-2026-09-04; Amazon's block of Muse (20 Sep 2026) is an adjacent event to responsibility-2026-09-01 but not a lawsuit.

Surprises:
- AB 2 was signed on 10 Sep 2026, before responsibility-2026-09-04 was logged (its source was NetChoice's 1 Sep veto request). The claim is about a suit, not the signing, so nothing is wrong, but the signing date means the clock for a NetChoice filing started 3 weeks ago. NetChoice's usual pattern is to sue ahead of the effective date, so this is the claim most likely to move before the 2027-03 resolve-by.
- The JCCP 5431 timetable (amended complaints 16 Nov, next hearing 13 Nov) pushes any demurrer past the Dec 2026 run's likely window, so responsibility-2026-08-05 (resolve-by 2026-12) may expire rather than resolve.

Calibration Observations:
- CAL-004 and CAL-009: nothing new this pass (no non-open grades).
- CAL-005 (unreachable sources) re-confirmed: five of twelve open grades rest partly on pages that returned HTTP 403 or blocked fetches (sftc register, CourtListener, nysenate via curl, legiscan, faz.net). One summarizer error (the "signed by Governor" mislabel on the NY Senate page) was caught only by a second read of the primary page, which suggests reading primary legislative pages twice or requiring the action-history text before grading.
- CAL-007 (slow institutional clocks) re-confirmed: all twelve claims remained open after 6 days, consistent with the 43-day pass on 2026-09-25 where nothing resolved either.
