# Signal grading, authority, 2026-10-01

Scorecard:
- open: 13, confirmed: 0, decayed: 0, falsified: 0, expired: 0

Scope notes:
- Live method-v2 claims graded: 13 (authority-2026-07-01 to 07-03, authority-2026-08-01 to 08-04, 08-06, 08-07, authority-2026-09-01 to 09-04). Every one received one appended grade line dated 2026-10-01.
- The retired method-v1 seed claims authority-2026-02-01 to 02-04 were excluded: not researched, not graded, not counted, and left untouched in the ledger.
- The last grading pass was 2026-09-25, 6 days before this run, so most claims legitimately stayed open. No claim was moved to Resolved claims.
- authority-2026-09-01 to 09-04 are graded for the first time (they were logged 2026-09 and had only "none yet").
- No qualifying event for any claim was found.

Grade Details:
- authority-2026-07-01: open, the xAI v. Weiser docket still shows its last known filing on 27 Apr 2026 (page updated 20 Sep 2026, read in the browser pane) and no Task Force matter has produced a ruling striking or enjoining a state AI law. The trigger events stay behind the 26 Oct 2026 Colorado hearing (source: https://www.courtlistener.com/docket/73171074/x-ai-llc-v-weiser/, Sep 2026)
- authority-2026-07-02: open, a 12 Sep 2026 report describes the four-senator text as a draft with no bill number, the Great American AI Act is a stalled discussion draft, and no chamber has voted on preemption (source: https://aiweekly.co/alerts/senate-draft-puts-a-duty-of-care-on-frontier-ai-builders, Sep 2026)
- authority-2026-07-03: open, no new state repeal or weakening tied to BEAD was found after NTIA's 3 Sep 2026 memo; only earlier pressure episodes (Louisiana bills withdrawn) turned up. The NTIA page was not re-opened this pass (no cited source)
- authority-2026-08-01: open, the Commission has still named no recipient of the first AI Act information requests (more than 30 firms) and no company has confirmed receipt (source: https://www.thestar.com.my/tech/tech-news/2026/09/02/eu-questions-dozens-of-companies-using-new-ai-powers, Sep 2026)
- authority-2026-08-02: open, the Federal Register API lists only the 7 Jul 2026 notice, document 2026-13628, with no final, revised or withdrawn version (source: https://www.federalregister.gov/documents/2026/07/07/2026-13628/policy-statement-concerning-the-suppression-of-accuracy-in-artificial-intelligence-systems, Jul 2026)
- authority-2026-08-03: open, searches found only commentary that a challenge to Illinois SB 315 is anticipated, and no filing by DOJ or an industry plaintiff
- authority-2026-08-04: open, last known filing remains 27 Apr 2026, so the case has neither terminated nor produced a merits ruling (source: https://www.courtlistener.com/docket/73171074/x-ai-llc-v-weiser/, Sep 2026)
- authority-2026-08-06: open, no named-provider action under the DSA, GDPR or consumer law was found after ChatGPT's 31 Aug 2026 VLOSE designation (the only named EU action against a frontier provider found was the January 2026 DSA proceeding against X over Grok, which predates the claim window), and the AI Act requests remain unnamed, so neither branch is met
- authority-2026-08-07: open, the rules remain proposed with the hearing on 26 Oct 2026 and no adoption. The coag.gov page returned no readable content this pass, so status rests on law-firm notices (source: https://www.consumerfinancemonitor.com/2026/09/09/colorado-publishes-draft-admt-regulations-2/, Sep 2026)
- authority-2026-09-01: open, the draft with preemption language had no bill number as of 12 Sep 2026 and no congress.gov record was found; the negotiators face the 3 Nov 2026 midterms (source: https://aiweekly.co/alerts/senate-draft-puts-a-duty-of-care-on-frontier-ai-builders, Sep 2026)
- authority-2026-09-02: open, California AG Bonta opened an investigation into OpenAI on 4 Sep 2026 under consumer protection law and the 2025 memorandum of understanding. An investigation is not a civil action, settlement or penalty citing SB 53 (source: https://aiweekly.co/alerts/california-ag-bonta-probes-openai-over-hugging-face-agent-hack, Sep 2026)
- authority-2026-09-03: open, Alabama's 24 Aug 2026 subpoena and the 15-state preservation letter are investigative only. No lawsuit, settlement or assurance concerning the Hugging Face incident was found; Florida's June 2026 suit concerns child safety (source: https://techcrunch.com/2026/08/24/alabama-launches-investigation-into-openais-hack-of-hugging-face/, Aug 2026)
- authority-2026-09-04: open, Executive Order N-9-26 (18 Sep 2026) only requests kill-switch recommendations by 16 Nov 2026, and no legislator has introduced a bill (source: https://ppc.land/newsom-sets-november-16-deadline-to-study-frontier-ai-kill-switch/, Sep 2026)

Qualifying Events:
- None this pass. Near misses that do not satisfy any claim: Bonta's 4 Sep 2026 OpenAI investigation (authority-2026-09-02 needs a civil action or settlement citing SB 53; also relevant to authority-2026-09-03 only if it concerns a lawsuit or settlement, which it does not) and Executive Order N-9-26 (authority-2026-09-04 needs a legislator's bill).

Surprises:
- The California AG's investigation of OpenAI (4 Sep 2026) rests on consumer protection law and the 2025 restructuring memorandum of understanding, not SB 53, which suggests the SB 53 enforcement claim (09-02) may be reached, if at all, through a different instrument than the one the claim names.
- Sources already hold nearly still: the xAI docket has not moved since 27 Apr 2026, and the Senate text has not been introduced in the three weeks since the 12 Sep report.

Calibration Observations:
- CAL-007 evidence: authority-2026-07-01, 08-04 and 08-07 remain frozen on the single Colorado rulemaking calendar (hearing 26 Oct 2026); a third consecutive pass added no movable observable.
- CAL-009 style risk: authority-2026-09-01 to 09-04 were logged from reporting that was days old (a Reuters-sourced draft, the 18 Sep executive order), so near-term "announced" steps (an investigation, a recommendations deadline of 16 Nov 2026) are easy to mistake for the claimed event. Graded strictly on the claims' words.
- CAL-005 evidence: aggregator outlets again repeat that OpenAI, Anthropic and Google received the AI Act requests; the Commission has named no recipient (Star/Reuters-derived piece), so these were not used.
- Unreachable sources: courtlistener.com via fetch (HTTP 403, read through the browser pane instead), coag.gov/ai (fetch returned no content), euractiv.com and mlex.com (not opened). Opened pages: courtlistener, federalregister API, thestar, and the two aiweekly alerts. The techcrunch, ppc.land and consumerfinancemonitor citations were read as search-result extracts, not opened, and support only open grades.
