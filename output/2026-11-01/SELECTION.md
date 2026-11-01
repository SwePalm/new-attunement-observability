# Theme selection, 2026-11-01

METHOD_VERSION 2.2. Cohort: A (agency, alignment, authority, autonomy, coordination, desire, governance, labor, power, responsibility, security).

Scoring per the theme-selection skill (0-5 on four dimensions, max 20). Inputs: `01-grading/*.md` and `02-sweep/*.md` of this run, and the deep-dive dates read from the `07-scenario/` folders of 2026-07-03, 2026-08-04, 2026-08-13, 2026-09-25, 2026-10-01 and 2026-10-02 (the SELECTION.md files of 2026-10-01 and 2026-10-02 agree). The `output/2026-10-17/` folder holds only empty scaffolding and no SELECTION.md, so it contributes no deep-dive dates. The previous cohort A grading and sweep were 2026-10-01, so the evidence window is about one month.

Selected Themes (4):
- responsibility, score 11 (by score), last deep dive 2026-08-04 (89 days). Three claims resolved forward in one run: responsibility-2026-08-06 (NY S9051B signed as chapter 368 on 28 Oct 2026), responsibility-2026-09-02 (eight state AG suits of 14 Oct 2026 citing the Hugging Face hack) and responsibility-2026-09-03 (German product liability law in BGBl. 2026 I Nr. 321, 27 Oct 2026, pre-announced); Regulatory Shifts add the Trahan CLAIM Act draft of 7 Oct 2026.
- alignment, score 11 (by score), last deep dive 2026-08-04 (89 days). alignment-2026-08-02 confirmed forward (Virkkunen's 14 Oct 2026 statement that the AI Office sent information requests to OpenAI and Anthropic, shared with autonomy-2026-09-03) and alignment-2026-09-04 confirmed forward, pre-announced (METR and Redwood named in OpenAI's 29 Oct 2026 post); sweep Confirmed Developments include the FTC CIDs, the cancelled GPT-6.1 Astra release and Anthropic's S-1 of 26 Oct 2026, with METR's 20 Oct review of the Anthropic Risk Report set against Anthropic's own low-risk reading (Counter-Signals).
- authority, score 11 (by score), last deep dive 2026-08-04 (89 days). authority-2026-10-01 confirmed forward (Anthropic's S-1 of 26 Oct 2026 disclosing the FTC civil investigative demand); 7 Confirmed/Regulatory bullets (eight state AG suits of 14 Oct, Texas petition of 23 Oct, FTC testimony demands of 26 Oct, Super Intelligence Force charter of 15 Oct, EU Scientific Panel of 9 Oct, NY bill of 29 Oct); Counter-Signals set the Commission's "no delay" line against a commentator's view that the Act does not reach development and testing.
- coordination, score 10 (by score), last deep dive 2026-08-04 (89 days). coordination-2026-08-01 confirmed forward, pre-announced (IESG approved the agentproto charter on 8 Oct 2026) and coordination-2026-10-01 confirmed forward (AAIF added four projects on 22 Oct 2026); Counter-Signals show governance outrunning implementation (AP2 Mandate on 37 stores against 17,056 on Checkout; Agent Skills with no tagged release).

Not Selected:
- power, score 8, PJM amended RBP filing of 29 Oct 2026 (power-2026-10-01, pre-announced) and NERC standards of 26 Oct; 80 days since dive, so it is the first candidate to be forced at the next cohort A run.
- security, score 8, 8 Confirmed/Regulatory bullets (Brotli CVE-2026-111497 on the KEV list, NIST/NSA/CISA guidance of 16 Oct) but dived 2026-10-01 (31 days) and only a pre-announced resolution.
- desire, score 7, NY S9051B signed 28 Oct 2026 and ChatGPT ads in 89 countries; no claim resolved; 80 days since dive, so it is a candidate to be forced next run.
- autonomy, score 7, autonomy-2026-09-03 and autonomy-2026-10-03 confirmed, but dived 2026-10-01 (31 days) and one event is shared with alignment.
- agency, score 5, bank blocking of outside agents (7 Confirmed/Regulatory bullets) but no resolutions and dived 2026-09-25 (37 days).
- governance, score 4, dived 2026-10-01; only the pre-announced Clayton appointment resolved.
- labor, score 4, dived 2026-10-01; no claim resolved, Barclays, American Express and Microsoft cuts logged, October Challenger report not yet out.

Scoring Table:
| theme | surprises | evidence | contradiction | staleness | total |
|-------|-----------|----------|---------------|-----------|-------|
| agency | 0 | 4 | 0 | 1 | 5 |
| alignment | 2 | 4 | 1 | 4 | 11 |
| authority | 2 | 4 | 1 | 4 | 11 |
| autonomy | 2 | 4 | 0 | 1 | 7 |
| coordination | 3 | 2 | 1 | 4 | 10 |
| desire | 0 | 3 | 0 | 4 | 7 |
| governance | 1 | 2 | 0 | 1 | 4 |
| labor | 0 | 2 | 1 | 1 | 4 |
| power | 1 | 3 | 0 | 4 | 8 |
| responsibility | 5 | 2 | 0 | 4 | 11 |
| security | 1 | 5 | 1 | 1 | 8 |

Scoring basis (reproducible):
- Grade surprises (points, then score = min(5, round(points))): agency 0 (no resolutions). alignment: alignment-2026-08-02 confirmed forward = 2 points, but the Virkkunen/AI Office requests of 12-14 Oct 2026 also resolved autonomy-2026-09-03, so the event is split equally (1 point each); alignment-2026-09-04 confirmed forward, pre-announced = 1 point; total 2. authority: authority-2026-10-01 confirmed forward, not pre-announced = 2. autonomy: autonomy-2026-09-03 = 1 point (split share); autonomy-2026-10-03 confirmed forward, pre-announced = 1; total 2. coordination: coordination-2026-08-01 confirmed forward, pre-announced = 1; coordination-2026-10-01 confirmed forward = 2; total 3. desire 0. governance: governance-2026-10-02 confirmed forward, pre-announced = 1. labor 0. power: power-2026-10-01 confirmed forward, pre-announced = 1. responsibility: responsibility-2026-08-06 confirmed forward = 2; responsibility-2026-09-02 confirmed forward = 2; responsibility-2026-09-03 confirmed forward, pre-announced = 1; total 5. security: security-2026-10-01 confirmed forward, pre-announced = 1. No falsified or decayed claims, no retrodictions. The grading files' Qualifying Events list no other event shared across themes, so no further splits apply.
- Evidence delta: top-level bullets under Confirmed Developments (C) plus Regulatory Shifts (R) in each 2026-11-01 sweep whose qualifying event is dated after 2026-10-01 (events dated 1 Oct or earlier excluded; duplicate bullets that restate another bullet's event are still counted as bullets). agency 6+1 = 7 (CFPB item dated Aug 2026 excluded); alignment 4+2 = 6 (Hawley bill announced 30 Sep excluded); authority 4+3 = 7; autonomy 5+2 = 7 (California AG subpoena dated 30 Sep excluded; the FTC restatement counted); coordination 2+0 = 2 (MCP 2026-07-28 spec and the Hawley/Murphy announcement of 1 Oct excluded); desire 3+2 = 5; governance 2+1 = 3 (NY DIGIT item of 21 Sep, KI-MIG of July and the RAISE effective-date bullet excluded; the Temu DSA item counted as the skill does not filter by topic); labor 3+0 = 3 (Italy, Netherlands and Connecticut 1 Oct items excluded); power 3+1 = 4 (Senate vote of 30 Sep and Virginia EO of Sep excluded); responsibility 1+2 = 3 (LASST suit 29 Sep and Hawley hearing 30 Sep excluded); security 5+3 = 8. Mapped 8+ -> 5, 6-7 -> 4, 4-5 -> 3, 2-3 -> 2.
- Contradiction density: bullets in Counter-Signals and Contradictions that set two named actors, instruments or data series against each other; unverified items, outlet disagreements on dates, counts or forums, and notes on the pipeline's own grading excluded; score = min(5, max(0, count - 1)). Counts: agency 1 (Jassy's dismissal against Meta's 10 million Muse users), alignment 2 (METR review against Anthropic's risk reading; Trump's "existing laws suffice" against the 30 Sep hearing and bills), authority 2 (voluntary charter against the FTC compulsory process led by the same task-force member; Commission's "no delay" against the commentator on scope), autonomy 1 (White House "must disclose" language against voluntary NIST/NSA/CISA practices), coordination 2 (AAIF hosting against Agent Skills with no release; AP2 Mandate 37 stores against Checkout 17,056), desire 1 (Muse transaction model against ChatGPT ads), governance 1 (charter assigning responsibility to companies against a floated export-control route), labor 2 (Barclays CEO against its finance director on AI attribution; BLS payrolls against the AI-cut announcements), power 1 (watchdog count of 35 TCEQ actions against the governor's office), responsibility 1 (administration self-policing posture against the Hawley and Trahan bills), security 2 (Microsoft "no successful attacks" against Sophos and the CISA KEV listing, counted once although it appears under both headings; Microsoft CVSS 8.1 against Sophos 9.2). This dimension needs reading judgment and is the least mechanical.
- Staleness: days from last v2 deep dive to 2026-11-01: alignment, authority, coordination, responsibility 89 (dived 2026-08-04; score 4); desire and power 80 (dived 2026-08-13; score 4); agency 37 (dived 2026-09-25; score 1); autonomy, governance, labor, security 31 (dived 2026-10-01; score 1).

Selection order check: forced themes none (no cohort A theme reaches 90 days; the maximum is 89). Filled 4 slots by total: responsibility 11, alignment 11, authority 11, coordination 10. The three 11s all make the cut, so the tie-break order (staleness 89 each, then grade surprises: responsibility 5, alignment 2, authority 2, then evidence: alignment 4, authority 4, then alphabetical) only fixes the listing order. The cut falls between coordination (10) and power and security (8), with no tie at the boundary.

Coverage rule: nothing is forced this run. Alignment, authority, coordination and responsibility are one day short of the 90-day limit; the deep dives selected today reset them.

Coverage Status (all 22 themes, after this run's deep dives):
| theme | cohort | last deep dive | days since | forced at next cohort run? |
|-------|--------|----------------|------------|----------------------------|
| agency | A | 2026-09-25 | 37 | no (65 at next A run, about 2026-11-29) |
| alignment | A | 2026-11-01 (this run) | 0 | no |
| authority | A | 2026-11-01 (this run) | 0 | no |
| autonomy | A | 2026-10-01 | 31 | no (59) |
| coordination | A | 2026-11-01 (this run) | 0 | no |
| desire | A | 2026-08-13 | 80 | yes (108) |
| governance | A | 2026-10-01 | 31 | no (59) |
| labor | A | 2026-10-01 | 31 | no (59) |
| power | A | 2026-08-13 | 80 | yes (108) |
| responsibility | A | 2026-11-01 (this run) | 0 | no |
| security | A | 2026-10-01 | 31 | no (59) |
| belonging | B | 2026-09-25 | 37 | no |
| creativity | B | 2026-10-02 | 30 | no |
| dependency | B | 2026-10-02 | 30 | no |
| identity | B | 2026-09-25 | 37 | no |
| intelligence | B | 2026-09-25 | 37 | no |
| learning | B | 2026-09-25 | 37 | no |
| meaning | B | 2026-10-02 | 30 | no |
| memory | B | 2026-08-13 | 80 | yes if the next B run is on or after 2026-11-11 (90 days) |
| perception | B | 2026-09-25 | 37 | no |
| trust | B | 2026-10-02 | 30 | no |
| truth | B | 2026-08-13 | 80 | yes if the next B run is on or after 2026-11-11 (90 days) |

Flag for instrument-review: with no forced themes this run, alignment, authority, coordination and responsibility sit at 89 days and desire and power at 80. At cohort A's next run (about 2026-11-29) all six would reach 117 and 108 days, so up to six themes would be forced against four slots, an overflow of two (the skill never drops forced themes). The four themes selected today (alignment, authority, coordination, responsibility) take their clocks back to 0, so only desire and power (108 days) remain forced at the next cohort A run, which fits inside the four slots with two evidence-driven places left. The cause is that the previous cohort A selections (2026-10-01) were forced entirely by governance, labor and security at 90 days while the August-dived themes aged in the queue, and the 2026-10-01 and 2026-10-02 runs sat one day apart, so the two cohorts' clocks bunched. Instrument-review should check whether forced-by-staleness should trigger earlier (for example at 75 days with a lower selection bonus) so a cohort does not carry six near-limit themes into one run. Cohort B has the same exposure in miniature: memory and truth (dived 2026-08-13) pass 90 days on 2026-11-11, so they are forced at any cohort B run on or after that date.
