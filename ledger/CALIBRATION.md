# Calibration memo

Written only by `signal-grading`. Read by `evidence-sweep`,
`scenario-generator`, and `scenario-eval` as context.

Hard bounds: max 10 active heuristics; each must cite >= 2 graded claim IDs;
each has an expiry and is retired unless re-confirmed by new grades.
This file never modifies skills, `instrument-review` is the human-gated
path for method changes.

Heuristic format:

```markdown
### CAL-NNN
- Heuristic: <falsifiable statement about this pipeline's bias>
- Evidence: <claim-id> (<grade>), <claim-id> (<grade>)
- Logged: YYYY-MM
- Expires: YYYY-MM (extend +3 months on re-confirmation)
```

## Active heuristics

### CAL-001
- Heuristic: Claims without a named actor, threshold, or observable event confirm by construction; their confirmations carry zero foresight signal. The v1 run seeded the same four such claims into 21 of 22 themes. Contrast case: agency's specific seeds produced a genuine ahead-of-horizon confirmation.
- Evidence: trust-2026-02-01 (confirmed, near-unfalsifiable), governance-2026-02-01 (confirmed, identical text), agency-2026-02-04 (confirmed early, specific), coordination-2026-02-04 (decayed on a different survey than the one that confirmed its identically worded siblings), truth-2026-02-03 (open, second identical open verdict on different sources), trust-2026-02-04 (open, second identical open verdict), power-2026-02-03 (open, no path to resolution before 2029-02)
- Logged: 2026-07
- Expires: 2027-01 (extend +3 months on re-confirmation)

### CAL-002
- Heuristic: The pipeline overestimates the firmness of announced regulatory timelines. Statutory deadlines slip under competitiveness pressure (EU Digital Omnibus deferred Annex III/I obligations by 16–24 months, Jun 2026). Apply added skepticism to any claim that treats a published compliance date as fixed.
- Evidence: trust-2026-02-03 (open, mechanism delayed), labor-2026-02-03 (open, mechanism delayed), agency-2026-02-03 (open, second recorded deferral of the same mechanism, Omnibus in force 29 Jul 2026), security-2026-02-03 (open, Annex III moved to Dec 2027 and embedded product to Aug 2028), coordination-2026-02-04 (decayed, Jun 2026 proposal became binding law), learning-2026-02-03 (open, deferral now statutory rather than political); counter-signal: trust-2026-07-01 (open, replacement Annex III date holding with no further deferral), governance-2026-07-01 (confirmed, low-cost transparency duties landed on schedule)
- Logged: 2026-07
- Re-confirmed: 2026-08-13, in a new form. Voluntarily announced disclosure dates slip like statutory ones: Anthropic's 30 Jul 2026 pledge to publish a redacted Mythos 5 transcript "within the next week" was still unmet on 2026-08-13 (alignment-2026-08-04, security-2026-08-03), and the Commission's Article 73 serious-incident guidance missed its 2 Aug 2026 date (autonomy-2026-08-06 decayed, responsibility-2026-08-03 open). Counter-signal strengthened at the same time: GPAI enforcement powers commenced exactly on schedule on 2 Aug 2026 (authority-2026-07-01 open, governance-2026-08-02 open), so EU firmness now looks selective rather than uniformly soft. The live failure mode after an on-time commencement is enforcement latency, not deadline slippage.
- Expires: 2027-04 (extend +3 months on re-confirmation)

### CAL-003
- Heuristic: The pipeline underweights non-state hardening mechanisms. Private ordering, insurance exclusions and products, procurement gates, collective bargaining, moved faster than statute in 2026 and was largely absent from the v1 corpus. Expect market and contractual mechanisms to lead regulation, not follow it.
- Evidence: agency-2026-02-04 (confirmed ahead of 12–36 month horizon), labor-2026-02-02 (confirmed via union contracts, channel unanticipated by v1), meaning-2026-07-02 (confirmed via SAG-AFTRA ratification and 2026 nurse contracts, not the named employer or regulator), meaning-2026-07-03 (confirmed via bargained and grievance channels), agency-2026-07-02 (open, card networks built agent liability products pre-emptively with no incident trigger), security-2026-07-02 (open, vendor-scoped registries moved while the named marketplace mandate did not); counter-signal: autonomy-2026-07-03 (open, motion was state-led via NIST and GSA rather than vendor-led), dependency-2026-07-02 (open, channel was state compulsion plus market exit)
- Logged: 2026-07
- Re-confirmed: 2026-08-13. agency-2026-08-04 confirmed not through the AI Act systemic-risk route it named but through voluntary bilateral pre-briefings by OpenAI and Anthropic to the Commission, made before the 2 Aug 2026 transparency regime took effect, so providers self-disclosed ahead of the statutory duty. creativity-2026-08-08 (open) shows the same shape: Suno licensed BMG twelve days after losing to GEMA in Munich, routing through a private counterparty rather than the winning collecting society.
- Expires: 2027-04 (extend +3 months on re-confirmation)

### CAL-004
- Heuristic: The pipeline logs claims whose triggering event is already in the public record at logging time, so the claim confirms on the first grading pass and the confirmation measures retrieval coverage rather than foresight. 15 of this run's 17 confirmations were satisfied by evidence dated before the claim's own logging month. Treat any confirmation that lands within one grading cycle of logging as a suspected retrodiction until the qualifying event is shown to postdate the claim.
- Evidence: desire-2026-07-03 (confirmed, threshold cleared by Washington HB 2225 in Mar 2026 and twelve states by Jun 2026, before the claim was written), memory-2026-07-02 (confirmed, both qualifying vendor shipments public 2 Mar and 26 Mar 2026), perception-2026-07-02 (confirmed, Google default shipped Sep 2025 and Samsung Feb 2026), power-2026-07-03 (confirmed, Abilene cancellation Mar 2026 and Utility Dive reporting Apr 2026), truth-2026-07-03 (confirmed, Munich ruling handed down 28 May 2026), belonging-2026-07-02 (confirmed, Folk and Dunn panel study published Mar 2026), autonomy-2026-07-02 (confirmed, qualifying ministry decision announced 19 Jun 2026), identity-2026-07-02 (confirmed on evidence predating the logging month), responsibility-2026-07-02 (confirmed, already satisfied by Mar and Apr 2026 statutes), intelligence-2026-07-01 (confirmed, benchmark target near-met at logging time)
- Logged: 2026-08
- Re-confirmed: 2026-08-13, and the pattern now fires inside a single run rather than across months. agency-2026-08-04 (confirmed) was logged on 2026-08-04 against a trigger that had already fired on 31 Jul 2026, in the same news cycle the sweep was reading. memory-2026-08-01 (confirmed) predicted with a 2027-04 horizon a memory-write confirmation control Microsoft had shipped and documented in Jan 2026, seven months before logging, while the sweep's own source framed that control as an unmet need. desire-2026-08-01 (confirmed) asked whether a 29 Jun 2026 discussion draft would become an introduced bill; S.5051 had been introduced on 21 Jul 2026, two weeks before logging and within its own cited source's subject matter. autonomy-2026-08-06 (decayed) is the inverse case, a retrodicted decay: it treated a compliance date as live two days after that date had passed. Counter-signal: meaning and truth each logged four claims in the 2026-08 sweep that were still genuinely open after research, so the defect is not uniform across themes. Strengthened later in the same run: Phase B corrected two Phase A grades from open to confirmed (coordination-2026-08-03, S.5051 introduced 21 Jul 2026; trust-2026-08-02, OpenAI's technical account published on openai.com 21 Jul 2026), and both had been satisfied before their own logging date. Final run tally is five retrodictions among six confirmations. The pipeline is currently better at retrieving what has already happened than at naming what will.
- Expires: 2027-02 (extend +3 months on re-confirmation)

### CAL-005
- Heuristic: A grade of `open` measures this pipeline's retrieval coverage as often as it measures the world, and the coverage gap is systematically Anglophone and secondary-source shaped. Treat `open` as "not found" rather than "did not happen" until a non-English source and a primary registry have been checked. Three distinct failure modes are now on record: missed non-English primary sources, grading from search-result titles without opening the page and checking its date, and AI-generated commentary fabricating specific, citable-looking regulatory actions.
- Evidence: desire-2026-07-02 (confirmed 2026-08-13 on a French Autorité de la concurrence sector inquiry that reported 17 Jul 2026, eighteen days before the 2026-08-04 pass graded the claim open after checking only the FTC, the CMA and Korea's FTC), meaning-2026-08-03 (open, an NYSNA page titled "Statement: Regarding decision in NYSNA v. Montefiore Medical Center" matched the claim's resolving event exactly but proved on fetch to be a May 2020 statement about a different dispute six years earlier), coordination-2026-08-03 (open, secondary outlets described the AI AGENT Act as introduced by Senator Warner while the primary record showed only a discussion draft), governance-2026-08-04 (open, secondary write-ups date Illinois SB 315 obligations to 2028 when the filing duty starts 1 Jan 2027); contamination case: two fabricated enforcement actions surfaced during desire research from low-quality AI-generated blogs (a California AG complaint over Amazon's Rufus, an FTC complaint over OpenAI Instant Checkout) and failed verification against oag.ca.gov and ftc.gov, either of which would have wrongly confirmed desire-2026-07-02.
- Fourth failure mode, added 2026-08-13: the pipeline infers a negative from a primary source it could not open. Several authoritative registries return HTTP 403 to automated fetching (congress.gov, openai.com, ftc.gov, nature.com, cde.ca.gov, courtlistener), and on two occasions this run a grader treated "I could not reach the registry" as "the event did not occur", then reasoned past accurate secondary coverage to defend the negative. Both errors ran the same way and both were caught only because a later phase re-checked: coordination-2026-08-03 and trust-2026-08-02 were each graded open and each corrected to confirmed. When a primary source is unreachable, record the claim as unverified and say which page could not be opened, rather than grading on the inference.
- Logged: 2026-08
- Expires: 2026-11 (extend +3 months on re-confirmation)

### CAL-006
- Heuristic: When choosing the named actor for a claim, the pipeline reaches for the most formal or most prominent institution in the domain rather than the one that actually moves first, so the claim resolves "no" on its stated observable while the phenomenon it describes is already happening through a faster adjacent channel. This is CAL-003 reappearing as a claim-construction error rather than a world-model error, and it converts real trends into future `expired` grades.
- Evidence: responsibility-2026-08-04 (open, gated on Verisk/ISO or a top-10 admitted carrier, the slowest channel, while affirmative AI cover is already live via Armilla, Relm and Munich Re), creativity-2026-08-03 (open, Spotify shipped the named badge mechanism on 11 Aug 2026 but scoped it to synthetic artist identity rather than synthetic audio, so the claim's control surface and the industry's diverged), identity-2026-07-01 (open, the underlying mechanism of collapsing voice trust is moving while the chosen observable is a public deprecation announcement banks avoid making for reputational reasons), perception-2026-08-04 (open, written to detect viewer-facing friction on labeled content while every mechanism found instead penalises creators who fail to disclose, the mirror image), security-2026-08-03 (open, a routine publication claim turning into a test of whether third-party confidentiality permits disclosure at all)
- Logged: 2026-08
- Expires: 2026-11 (extend +3 months on re-confirmation)

### CAL-007
- Heuristic: The pipeline writes claims keyed to scheduled institutional calendars (rulemaking dockets, grant award cycles, survey waves, legislative sessions) whose clock speed is quarterly or slower, then grades them at monthly or faster cadence. The result is a large open set structurally incapable of emitting signal between runs, and a grading pass whose cost is real while its yield is near zero. Before logging a claim, check that at least one observable event can occur inside the next grading interval; before re-grading a theme, check that any claim can move at all.
- Evidence: truth-2026-08-02 (open, no live truth claim resolves before Feb 2027, so the theme cannot move inside a monthly cycle), learning-2026-08-01 (open, the EDU AI RFP closed 31 Jul 2026 with work estimated to begin Nov 2026), identity-2026-08-01 (open, the OIDF vote window is 16-30 Sep 2026 and cannot open earlier), belonging-2026-08-04 (open, the Digital Fairness Act proposal is now indicated for Q4 2026), power-2026-08-01 (open, RTO/ISO show-cause responses were due 17 Aug 2026, four days after this run date). Aggregate for this run: 22 themes researched over a nine-day interval, 6 confirmed, 1 decayed, 0 falsified, 0 expired, everything else open. Phase B then added 78 claims, taking the live open set to 213, so the corpus is growing about thirty times faster than it resolves.
- Logged: 2026-08
- Expires: 2026-11 (extend +3 months on re-confirmation)

## Retired heuristics

None.
