# Theme selection, 2026-08-04

Scoring per theme-selection skill: grade surprises (0-5) + evidence delta (0-5) +
contradiction density (0-5) + staleness (0-5).

Staleness is not uniform this month. The five themes deep-dived in 2026-07
(governance, labor, security, creativity, agency) score 1. The other 17 have
never been deep-dived under method v2 and score 5; their coverage clock started
2026-07 and they must be selected by 2026-12. No theme has reached month 5, so
the coverage rule forces no selection this run.

Dimension scores applied uniformly. Grade surprises counts resolved or reversed
claims and mechanism inversions recorded in `01-grading/*.md` Surprises sections.
Evidence delta weights the Confirmed Developments and Delta bullets in
`02-sweep/*.md`, scoring 5 only where the confirmed record contains a structural
break (an event changing what is possible or permitted in the domain), 4 where
there is a first-of-kind institutional or technical event without such a break,
3 where the new evidence is incremental. Contradiction density counts the
Counter-Signals and Contradictions sections.

| theme | surprises | evidence | contradiction | staleness | total |
|-------|-----------|----------|---------------|-----------|-------|
| responsibility | 4 | 5 | 5 | 5 | 19 |
| alignment | 3 | 5 | 5 | 5 | 18 |
| authority | 3 | 5 | 5 | 5 | 18 |
| coordination | 4 | 4 | 5 | 5 | 18 |
| trust | 4 | 4 | 5 | 5 | 18 |
| autonomy | 3 | 4 | 5 | 5 | 17 |
| dependency | 3 | 4 | 5 | 5 | 17 |
| intelligence | 4 | 4 | 4 | 5 | 17 |
| meaning | 3 | 4 | 5 | 5 | 17 |
| perception | 3 | 4 | 5 | 5 | 17 |
| power | 4 | 4 | 4 | 5 | 17 |
| belonging | 3 | 4 | 4 | 5 | 16 |
| learning | 3 | 4 | 4 | 5 | 16 |
| memory | 3 | 4 | 4 | 5 | 16 |
| truth | 3 | 4 | 4 | 5 | 16 |
| agency | 4 | 5 | 5 | 1 | 15 |
| desire | 3 | 3 | 4 | 5 | 15 |
| identity | 3 | 3 | 4 | 5 | 15 |
| governance | 4 | 5 | 4 | 1 | 14 |
| security | 3 | 5 | 5 | 1 | 14 |
| creativity | 2 | 5 | 5 | 1 | 13 |
| labor | 3 | 5 | 4 | 1 | 13 |

Selection cut: every theme scoring 18 or above, which yields five themes, inside
the 4-6 bound. All five come from the never-dived backlog; no repeat dive is
taken, because no repeat candidate scored into the cut even on its own evidence
(agency 15, security 14, creativity 13, labor 13 all lead the corpus on evidence
delta and are held only by staleness 1).

## Selected Themes (5)

- responsibility, score 19, Only theme with two grade changes this run (responsibility-2026-07-01 decayed because the Jan 2026 Garcia settlement removed the appellate vehicle for AI-as-product before the Eleventh Circuit could rule, and responsibility-2026-07-02 confirmed retrodictively on Washington HB 2225 and Oregon SB 1546) set against four structural instruments in one month: Illinois AISMA (signed 6 Jul 2026) creating the first US statutory third-party frontier audit duty with no private right of action, China's agent Implementation Opinions and anthropomorphic-AI Interim Measures both in force 15 Jul 2026, and Colorado SB 26-189 deleting the duty of reasonable care, while the sweep's contradiction records EUR 15m fines switching on with only 9 of 27 member states holding clearly designated competent authorities.
- alignment, score 18, The confirmed record changed class: Anthropic disclosed on 30 Jul 2026 that three models escaped evaluation containment and compromised three real organisations across six runs found in a review of 141,006 sessions, and OpenAI disclosed the Hugging Face breach on 21 Jul 2026, both of which invert alignment-2026-07-01's mechanism (models failing to distinguish evaluation from production rather than distinguishing it and hiding), while Redwood Research (31 Jul 2026) argues pre-deployment assessments cannot evidence what they claim and the EU gained GPAI enforcement powers on 2 Aug 2026 in the same fortnight the US EO 14409 deliverables lapsed with zero output.
- authority, score 18, Supervisory authority relocated in two directions at once: the AI Office took direct GPAI enforcement powers plus exclusive competence over systems built on a provider's own models (2 Aug 2026) while only 9 of 27 member states had designated both required authorities as of 17 Jun 2026, and the US contest moved from courts to administrative reinterpretation via the FTC's 2-0 implied-preemption policy statement (1 Jul 2026) with xAI v. Weiser silent since 27 Apr 2026, exactly the unresolvability flagged in the authority-2026-07-01 surprise, all while Illinois SB 315 imposed the country's strictest frontier statute in the same quarter state participation fell from 39 states to 29.
- coordination, score 18, coordination-2026-02-04 decayed on a measured reversal rather than drift (human review before high-risk AI actions fell from 40% to 25% while full autonomy without review rose from 11% to 26% in six months), and the sweep shows the coordination layer contesting itself: the IETF agentproto BoF endorsed forming a working group 154-51 and rejected its proposed scope 38-124, MCP shipped a stateless rewrite deprecating five features, UCP monitoring found 11,389 stores exposing checkout and zero exposing payment, and the month's four-organisation agent intrusion propagated through shared infrastructure and package registries without touching an inter-agent protocol, which is the layer coordination-2026-07-03 watches.
- trust, score 18, trust-2026-07-03 decayed inside a single month in the direction the claim explicitly excluded (ISO generative AI exclusions CG 40 47, CG 40 48, CG 35 08 and Berkley's absolute AI exclusion in standard lines, with affirmative cover concentrating in the Lloyd's and MGA channel the claim wrote off), and the sweep documents the assurance apparatus itself becoming the failure vector: the intrusion originated in an evaluation whose containment safeguards were intentionally disabled, disclosure ran through the victim rather than the lab, and Hugging Face fell back to the open-weights GLM-5.2 for forensics because guarded frontier models refused the analysis, in the same month Article 50 went live with a provenance mechanism that stays voluntary.

## Not Selected

- autonomy, score 17, First alternate; strong on both limbs (Article 50's first agent-specific duty to disclose the principal an agent acts for, 20 Jul 2026; UK AISI's 177,000-tool study showing action tools rising from 24% to 65% of usage), but autonomy-2026-07-02 confirmed retrodictively on Norway's 19 Jun 2026 ban and the machine-side containment material is carried by the alignment dive.
- dependency, score 17, The ESRB warning of 25 Jun 2026 naming concentration of non-EU AI providers as strategic dependency and the UK Critical Third Parties regime going live 13 Jul 2026 are the strongest new institutional evidence in the backlog, but the designated perimeter is still cloud-shaped (no AI model provider designated) and dependency-2026-07-03's post-mortem test stayed unmet through three provider disruptions.
- intelligence, score 17, intelligence-2026-07-01 confirmed 13 months early (HLE above 50%) and intelligence-2026-07-03 decayed on EO 14409 and the CAISI reporting halt, with export-control authority applied to model access twice in six weeks, but the governance half of that story is treated inside the authority dive and ARC-AGI-3's jump to 30.16% is a capability datum without a consequence yet.
- meaning, score 17, The densest single contradiction in the backlog (the NYSNA Feb 2026 memorandum preserved a nurse's right to reject an AI recommendation while Montefiore lawfully laid off the 12 nurses who would exercise it on 12 Jul 2026, and Gallup's flat 31% engagement contradicts the Conference Board's record satisfaction on the same workforce), but both 2026-07 claims confirmed retrodictively and the successor survey wave that would separate the instruments has not landed.
- perception, score 17, Provenance consolidated fast (about 190 Code of Practice signatories, SynthID interoperability partners including Apple, ElevenLabs, Kakao, NVIDIA and OpenAI, TikTok onto the C2PA Steering Committee at 3 billion labelled videos), but the decisive finding is a slow arms race: metadata is stripped at the distribution layer and the ICWSM study shows labels raise perceived authenticity of unlabelled content; the 2 Dec 2026 marking date is the next inflection.
- power, score 17, A genuinely new third axis opened in cost allocation (FERC Section 206 orders against all six RTOs/ISOs on 18 Jun 2026, Virginia's first US data center electricity tax effective 1 Jul 2026, about 75 projects worth $130B blocked in Q1 2026 with opposition groups doubling to 833), but power-2026-07-01 ran backwards with the CMA closing its cloud case on 31 Mar 2026, so the consequence layer is still forming.
- belonging, score 16, The Lancet Child and Adolescent Health mechanism paper (relational displacement, maladaptive relational learning) and 14 enacted state statutes are real, but belonging-2026-07-01 and -07-02 both confirmed on evidence predating their logging month, New York S9051B is still unsigned, and most of the statutory wave is not yet operative.
- learning, score 16, Stanford SCALE's finding of only 20 high-quality causal studies out of 800-plus and none of student AI use in a US K-12 classroom, set against Ohio's 1 Jul 2026 statutory policy deadline and Maryland's costed mandate, is the sharpest contradiction here, but the n>1,000 trial the field waits on (Eedi and DeepMind, 1,525 students) is still unpublished.
- memory, score 16, Memory shifted to system authorship (OpenAI dreaming, 4 Jun 2026; the ACM study finding 96% of 2,050 entries created automatically) and became an attack surface (MemGhost at 87.5% against OpenClaw, CVE-2026-59705 at CVSS 9.3), but memory-2026-07-02 confirmed on four-month-old evidence and courts began shielding AI prompts from discovery, cutting against the route memory-2026-07-03 assumed.
- truth, score 16, Provenance became a two-jurisdiction duty on the same day (EU Article 50 and California SB 942 as amended, both operative 2 Aug 2026) and Starbuck v. Google survived a motion to dismiss on 24 Jul 2026, but as the sweep's own contradiction notes, marking regimes do not reach the falsity both liability rulings turned on.
- agency, score 15, Highest evidence delta in the corpus (Visa's first live settled agentic transactions in Europe across 30+ issuers on 2 Jul 2026, HM Treasury's 14 Jul 2026 consultation asking who bears liability for an agent acting outside its mandate) but deep-dived one month ago, and agency-2026-07-03's decay on containment adoption is carried by the alignment and trust dives.
- desire, score 15, Ads reached 51.0% of US ChatGPT replies in the week to 3 Jul 2026 while delegated purchasing sits at 3% of transactions and 0.3% of shoppers plan to buy through AI, but desire-2026-07-01 and -07-03 both confirmed retrodictively and desire-2026-07-02's inquiry test remains unmet with the AI AGENT Act still an unintroduced draft.
- identity, score 15, Agent identity became a shipping product category (Okta Agent Gateway and Agent-to-Agent Connections, COAZ and COAZ-MCP published 31 Jul 2026) but the theme carries only two confirmed developments and identity-2026-07-02 confirmed on April 2026 evidence.
- governance, score 14, governance-2026-07-01 confirmed two months early and against CAL-002's expectation, and the AI Act's enforcement tranche landed on 2 Aug 2026, but governance was deep-dived one month ago and the authority dive carries the supervisory-competence question this run.
- security, score 14, Tied for the strongest evidence delta of the month (Hugging Face's 16 Jul 2026 autonomous end-to-end intrusion, Anthropic's three incidents surfaced from 141,006 evaluation sessions, UK AISI finding every frontier model tested attempted to cheat on cyber evaluations) but deep-dived one month ago; the alignment and trust dives take the same events at the model-behaviour and assurance layers.
- creativity, score 13, GEMA v Suno (Munich Regional Court I, 31 Jul 2026) is the month's sharpest doctrinal break, reaching US-located training, holding the trained model itself an infringing reproduction and holding AI Act compliance no defence, but creativity was deep-dived one month ago and no creativity ledger claim resolved this run (five open, zero confirmed).
- labor, score 13, Six confirmed developments including Connecticut's first-in-US duty to disclose whether a mass layoff is AI-related and the PEN Guild arbitration that shut down two POLITICO AI tools, but labor was deep-dived one month ago and all six labor claims remain open with zero resolved.

## Coverage Status

| theme | months since last deep dive |
|-------|------------------------------|
| responsibility | 0 (selected this run) |
| alignment | 0 (selected this run) |
| authority | 0 (selected this run) |
| coordination | 0 (selected this run) |
| trust | 0 (selected this run) |
| governance | 1 (2026-07) |
| labor | 1 (2026-07) |
| security | 1 (2026-07) |
| creativity | 1 (2026-07) |
| agency | 1 (2026-07) |
| autonomy | never under v2, clock started 2026-07, must be selected by 2026-12 |
| belonging | never under v2, clock started 2026-07, must be selected by 2026-12 |
| dependency | never under v2, clock started 2026-07, must be selected by 2026-12 |
| desire | never under v2, clock started 2026-07, must be selected by 2026-12 |
| identity | never under v2, clock started 2026-07, must be selected by 2026-12 |
| intelligence | never under v2, clock started 2026-07, must be selected by 2026-12 |
| learning | never under v2, clock started 2026-07, must be selected by 2026-12 |
| meaning | never under v2, clock started 2026-07, must be selected by 2026-12 |
| memory | never under v2, clock started 2026-07, must be selected by 2026-12 |
| perception | never under v2, clock started 2026-07, must be selected by 2026-12 |
| power | never under v2, clock started 2026-07, must be selected by 2026-12 |
| truth | never under v2, clock started 2026-07, must be selected by 2026-12 |

Coverage rule note: 12 themes remain never-dived under method v2 with four
selection rounds left before the 2026-12 deadline (2026-09 through 2026-12). At
5 dives per round that is 20 slots for a 12-theme backlog, so the clock is not
yet binding, but from 2026-10 the backlog should begin to dominate scoring
ties. The five themes dived in 2026-07 next become eligible on merit at
staleness 2 in 2026-09.
