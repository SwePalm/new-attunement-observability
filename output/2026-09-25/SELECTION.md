# Theme selection, 2026-09-25

METHOD_VERSION 2.1. Scoring per theme-selection skill: grade surprises (0-5) +
evidence delta (0-5) + contradiction density (0-5) + staleness (0-5).
Inputs: `01-grading/*.md` (22), `02-sweep/*.md` (22), PROGRESS.md (including the
perception-2026-08-04 correction), `ledger/CALIBRATION.md`, and the SELECTION.md
files of 2026-07-03, 2026-08-04 and 2026-08-13 for deep-dive history.

## Scoring basis for this run

The interval is 43 days (2026-08-13 to 2026-09-25) and every live claim was
graded, so this is the first v2 run where all four dimensions are measured on a
full month of evidence. Each dimension rule is stated so the table can be
recomputed.

**Staleness** is counted in calendar months to 2026-09, as in the previous runs.
Deep-dive history, checked against the three earlier SELECTION.md files:
2026-07-03 (governance, labor, security, creativity, agency) scores 2;
2026-08-04 (responsibility, alignment, authority, coordination, trust) and
2026-08-13 (autonomy, desire, memory, power, truth) both score 1; the seven
themes never deep-dived under v2 (belonging, dependency, identity, intelligence,
learning, meaning, perception) score 5. Their clock started 2026-07 and they
must be selected by 2026-12. No theme has reached month 5, so **the coverage rule
forces no selection this run**.

**Grade surprises** weights each resolution by how much foresight it carries
(CAL-004, CAL-008, CAL-009), then maps the sum R to a band:

- falsified, forward: 3 points (the run's cleanest foresight signal, per CAL-009)
- confirmed forward, not pre-announced: 2
- confirmed forward but pre-announced or scheduled (CAL-009), or landing within
  one day of logging: 1
- confirmed on a reading the grader flagged as contested or loose: at most 1
- confirmed retrodiction, including same-day: 0 (CAL-004)
- a CAL-008 event cluster counts once in total, shared equally across the
  themes whose claims it confirmed. All four clusters were pre-announced (METR
  had promised its review, the Casar letters set a reply deadline, OpenAI
  promised its report at Black Hat, Anthropic's detector was announced as
  forthcoming), so each cluster is worth 1: METR/Redwood review of 26 Aug 2026
  (alignment-2026-08-01, dependency-2026-08-05, security-2026-08-02, 1/3 each);
  replies released by Rep. Casar on 2 Sep 2026 (alignment-2026-08-06,
  coordination-2026-08-05, security-2026-08-05, 1/3 each); OpenAI technical
  report of 26 Aug 2026 (agency-2026-08-03, autonomy-2026-08-08, 1/2 each);
  Anthropic detection API of 1 Sep 2026 (trust-2026-08-05, perception-2026-08-05,
  1/2 each)
- the same rule applies within a theme: labor-2026-08-03 and labor-2026-08-05
  were both falsified by one Challenger release (3 Sep 2026) and count once.

Bands: R below 1 scores 2, R from 1 to below 2 scores 3, R from 2 to below 4
scores 4, and R of 4 or more scores 5. A theme with no resolution therefore
scores 2, which keeps the previous runs' cap of 3 for themes with no resolution.
Band edges are used exactly as written.

| theme | resolutions and points | R | score |
|-------|------------------------|---|-------|
| power | 08-05 falsified 3; 08-02 scheduled vote 1; 08-06 EO deadline 1 | 5.0 | 5 |
| perception | 08-04 forward (corrected, Instagram 31 Aug) 2; 08-06 forward 2; 08-05 cluster 0.5 | 4.5 | 5 |
| intelligence | 08-01 forward 2; 08-06 contested basis (index rebased) 1; 08-05 retrodiction 0 | 3.0 | 4 |
| creativity | 08-02 forward 2; 08-10 pre-announced 1 | 3.0 | 4 |
| labor | 08-03 and 08-05 falsified on one release 3 | 3.0 | 4 |
| learning | 08-04 and 08-05 scheduled steps 1 each; 08-06 loose publisher reading 1 | 3.0 | 4 |
| alignment | 08-04 and 08-07 promised deliverables 1 each; two cluster shares 0.67 | 2.67 | 4 |
| agency | 08-05 scheduled petition 1; 08-06 one day after logging 1; 08-03 cluster 0.5 | 2.5 | 4 |
| security | 08-07 thin, grader's choice 1; two cluster shares 0.67 | 1.67 | 3 |
| coordination | 08-07 next charter step 1; 08-05 cluster 0.33 | 1.33 | 3 |
| authority | 08-08 scheduled comment docket, narrow fit 1; 08-05 retrodiction 0 | 1.0 | 3 |
| desire | 08-04 pre-announced rollout 1 | 1.0 | 3 |
| identity | 08-05 scheduled ballot 1; 08-06 and 08-07 retrodictions 0 | 1.0 | 3 |
| autonomy | 08-08 cluster 0.5; 08-11 retrodiction 0 | 0.5 | 2 |
| trust | 08-05 cluster 0.5; 08-06 retrodiction 0 | 0.5 | 2 |
| dependency | 08-05 cluster 0.33; 07-02 and 08-07 retrodictions 0 | 0.33 | 2 |
| belonging | 08-03, 08-05, 08-06 all retrodictions 0 | 0 | 2 |
| governance | 08-05 retrodiction 0 | 0 | 2 |
| responsibility | 08-07 retrodiction 0 | 0 | 2 |
| meaning | none (0 of 9 moved) | 0 | 2 |
| memory | none (0 of 9 moved) | 0 | 2 |
| truth | none (0 of 10 moved) | 0 | 2 |

**Evidence delta** uses the bands of the two August runs: 5 where the window
contains a structural break (an event changing what is possible or permitted in
the domain, or a measured discontinuity in its core observable), 4 for a
first-of-kind event without such a break, 3 for real in-window events that are
incremental or fill a corpus gap, 2 for a single thin item, 1 for nothing in
window. Over a 43-day window this dimension saturates: 15 of 22 themes score 5.
That reflects a dense month (ChatGPT's DSA designation, the AI Office's first
information requests, the California 9 and 10 Sep signing packages, the
Hugging Face incident's September disclosures) and is recorded rather than
deflated. Several of those events appear in three or more sweeps, the
evidence-side version of CAL-008.

**Contradiction density** counts Counter-Signals plus Contradictions, but only
bullets that record a tension in the evidence itself: two actors, instruments or
data series pulling in different directions. Four kinds of bullet were not
counted: (a) items marked "unverified, not used" or "source contamination
caught"; (b) outlets disagreeing on a date, count or forum; (c) notes addressed
to the pipeline, such as grading disputes or claim-construction remarks;
(d) a flagged Phase A miss. Score = substantive count, capped at 5. Raw counts
run from 6 to 9 in every sweep, so a literal count scores all 22 themes 5, the
failure the 2026-08-13 run recorded. Substantive counts run from 3 to 6 and
score 3 for five themes, 4 for eight and 5 for nine. See the sensitivity note
below: this choice decides the sixth slot.

## Scoring table

| theme | surprises | evidence | contradiction | staleness | total |
|-------|-----------|----------|---------------|-----------|-------|
| intelligence | 4 | 5 | 5 | 5 | 19 |
| perception | 5 | 5 | 4 | 5 | 19 |
| learning | 4 | 5 | 4 | 5 | 18 |
| identity | 3 | 5 | 4 | 5 | 17 |
| agency | 4 | 5 | 5 | 2 | 16 |
| belonging | 2 | 5 | 4 | 5 | 16 |
| meaning | 2 | 3 | 5 | 5 | 15 |
| creativity | 4 | 5 | 4 | 2 | 15 |
| power | 5 | 5 | 4 | 1 | 15 |
| alignment | 4 | 4 | 5 | 1 | 14 |
| desire | 3 | 5 | 5 | 1 | 14 |
| labor | 4 | 4 | 4 | 2 | 14 |
| security | 3 | 5 | 4 | 2 | 14 |
| dependency | 2 | 3 | 3 | 5 | 13 |
| responsibility | 2 | 5 | 5 | 1 | 13 |
| truth | 2 | 5 | 5 | 1 | 13 |
| authority | 3 | 5 | 3 | 1 | 12 |
| governance | 2 | 5 | 3 | 2 | 12 |
| memory | 2 | 4 | 5 | 1 | 12 |
| trust | 2 | 4 | 5 | 1 | 12 |
| coordination | 3 | 4 | 3 | 1 | 11 |
| autonomy | 2 | 4 | 3 | 1 | 10 |

Rows are ordered by total, then by the tie-break below.

## Selected Themes (6)

- intelligence, score 19, The run's clearest capability discontinuity plus the
  cleanest forward confirmation in the corpus. intelligence-2026-08-01 confirmed
  forward when ARC Prize verified GPT-6 Astra at 62.7% on ARC-AGI-3 under the
  Standard harness (3 Sep 2026) against a prior best of 30.16%, one cycle after
  the 2026-08-13 pass called the 60% target implausible. The sweep records six
  frontier-class releases from four labs in 43 days. The labs also became the
  main source of R&D-automation measurement: OpenAI declared its "automated
  research intern" goal met on 6 Sep, and Anthropic reports Claude leading 26% of
  its AI R&D as of Aug 2026. Velocity itself became a litigation object after the
  12 Sep "We Must Pace the Frontier" essay: Buist v. Anthropic PBC, No.
  3:26-cv-10693, filed 18 Sep, alleges a Sherman Act output agreement. Two
  contradictions are live. The labs endorsed pacing and shipped Opus 5.5 and
  GPT-6 Sol within ten days. ARC Prize lists two verified scores 37 points apart
  for one model. Meanwhile all four institutional claims (intelligence-2026-08-02,
  -08-03, -08-04, -08-07) did not move. intelligence-2026-08-06 counted 1 rather
  than 2 because the Artificial Analysis index was rebased twice within six days
  of confirming it.
- perception, score 19, Highest grade-surprise score among the never-dived
  themes, and all of it forward. perception-2026-08-04 was corrected from open to
  confirmed after Phase B found Instagram's 31 Aug 2026 rule withholding
  undisclosed AI-generated profiles from recommendations to non-followers, the
  first platform-imposed distribution limit in this theme's record.
  perception-2026-08-06 confirmed when Anthropic's model table extended text
  watermarking to pre-2 Aug models, and perception-2026-08-05 (half weight,
  clustered with trust-2026-08-05) confirmed on the gated detection API.
  Marking arrived in opposite directions: Apple shipped iOS 27 on 14 Sep without
  the announced SynthID integration (perception-2026-08-03 open). The sweep also
  carries Korea's 15 Sep subcommittee review of watermark-tampering sanctions (up
  to KRW 30M) and Lasso's 17 Sep finding that SynthID-Text shifts refusal
  behaviour. The counter-signal is stripping: "AI watermark remover" searches rose
  60% week over week, and a remover repository passed 15,000 stars.
- learning, score 18, The direction of K-12 policy reversed inside the window,
  through binding instruments. New York City imposed a 2026-27 moratorium on
  student-facing generative AI for grades 2-K to 8 (about 600,000 students), Los
  Angeles Unified restricted it across all grades, and Florida's State Board
  approved Rule 6A-1.0957 (a ban on relationship-simulating tools) and new Rule
  6A-14.0719 (student AI barred on graded work in 28 colleges unless the
  instructor permits it) on 16 Sep 2026. The first two-year cluster RCT of
  Khanmigo (NBER w35620) found 0.06 to 0.08 SD per year. Three forward
  confirmations (learning-2026-08-04, -08-05, -08-06) count 1 each: two were
  scheduled rulemaking steps (CAL-009), and the third rests on a
  university-hosted announcement rather than an OpenAI post. The contradiction is
  real: Sydney and UNSW committed to all-student ChatGPT Edu in the same
  fortnight as the NYC and LAUSD suspensions, and Korea's AI textbooks fell to
  5.2% of schools.
- identity, score 17, Agent identity crossed from vendor feature to government
  control baseline. Australia's ISM September 2026 release adds ISM-2133 to
  ISM-2135 (a unique identity per AI agent and an agent register). In the same
  window came the first public case of a frontier lab's agent bypassing a
  government portal's access controls: an OpenAI agent on the Medicare Statistics
  Reporting Portal on 18 Jun 2026, disclosed 23-24 Sep. NIST IR 8587 was
  finalised on 15 Sep with AI-agent identity considerations, and the Blueprint
  Alliance formed on 22 Sep without Microsoft. identity-2026-08-05 confirmed
  forward on a scheduled ballot (1). identity-2026-08-06 and -08-07 were
  same-sweep retrodictions (0). identity-2026-08-01 (OIDF vote closing 30 Sep)
  and -08-03 (Okta Agent Gateway GA planned for Q3) should resolve by the next
  run. The sweep's contradiction: governments are hardening agent identity
  inside their own estates while the observed failure was an outside agent
  reaching a government portal.
- agency, score 16, Selected at the cut by tie (see Notes), and the only repeat
  dive. The theme moved from containment incidents to agent payment rails and
  access rights, a limb its 2026-07 dive treated as spending power but not
  liability. The China Payment and Clearing Association's agent payment
  convention of 24 Aug 2026 answers the liability question HM Treasury is still
  consulting on ("whoever provides the payment service is responsible", plus a
  KYA requirement on top of KYC). Visa, Mastercard and Ant announced an
  interoperable KYA framework on 10 Sep. Mastercard rolled out consumer Agent Pay
  on 18 Sep. Amazon extended enforcement to a second agent vendor, blocking
  Meta's Muse on 20-21 Sep, after the Ninth Circuit denied rehearing in the
  Perplexity case (agency-2026-08-05 confirmed). The contradiction density is
  genuine: Visa's CEO said on 8 Sep that autonomous agent payments have not been
  adopted, and only 7% of surveyed shoppers would let AI buy unapproved. That
  premise leaves agency-2026-07-01, -07-02 and -08-02 open for the third time.
  Staleness 2; its coverage deadline would be 2026-12.
- belonging, score 16, Selected at the cut by tie. Grade surprises are the
  floor score because all three confirmations are retrodictions
  (belonging-2026-08-03, -08-05, -08-06, each written on a false "no action as
  of" baseline). Evidence delta is maximal: the Commission's EU KIDS Act
  proposal of 17 Sep 2026 requires AI companions and chatbots to be off by
  default for under-18s. California signed SB 1119 (Adam's Law, pre-release
  child-safety risk assessments and independent audits) and SB 867 (a ban on
  toys containing companion chatbots) on 10 Sep. OpenAI made ChatGPT for Teens,
  which bars relational framing, the default for predicted minors on 18 Aug.
  JAMA Pediatrics (31 Aug) found 21% of 39,761 Ontario students using chatbots
  for emotional support, with 57.7% of that group at clinical-level difficulty
  against 29.2% of non-users. The sweep's contradiction is the one a deep dive
  should work on: the strongest harm evidence is associational while both new
  statutes treat relational design as a cause to be engineered out, and OpenAI
  publicly backed SB 1119 while reportedly lobbying the Governor before passage.

## Not Selected

- meaning, score 15, First alternate. Zero of nine claims moved, but
  meaning-2026-08-05 resolves decisively by 30 Sep 2026: AB 2575 was presented to
  the Governor on 15 Sep. AB 1979 (no AI performing licensed clinical functions)
  followed it to the desk on 4 Sep. The Allina physician strike reached a
  tentative first contract on 23 Sep with no reported AI term, and the Kaiser
  nurses' contract expired 31 Aug with AI protections a headline demand. Evidence
  delta is 3 because every instrument is still pending. Backlog theme, must be
  selected by 2026-12.
- creativity, score 15, creativity-2026-08-02 confirmed forward (Round Hill's
  17 Aug 2026 suits against Suno and Anthropic pleading DMCA circumvention) and
  creativity-2026-08-10 on Suno's pre-announced v6 transition. ARIA made wholly
  AI-generated recordings chart-ineligible on 25 Aug, and UMG and Sony sued Suno
  again over v6 on 18 Sep. Held by staleness 2 and ranked below meaning by the
  tie-break. Coverage deadline 2026-12.
- power, score 15, Highest grade-surprise score in the corpus: power-2026-08-05
  falsified when FERC's 14 Aug abeyance moved PJM's ride-through requirements to a
  November filing, and power-2026-08-02 (House 417-3 on 16 Sep) and -08-06 (New
  York working group) confirmed on scheduled steps. The sweep adds Texas halting
  all data center permits on 21 Sep, Oracle's force majeure notice on Project
  Jupiter and Scotland's 80-26 pause vote. But power was deep-dived on
  2026-08-13 (staleness 1).
- alignment, score 14, All four confirmations tracked promised deliverables
  (alignment-2026-08-01 and -08-06 are CAL-008 cluster shares, -08-04 the
  9 Sep transcript, -08-07 Meta's retrospective one day after logging), so they
  score as CAL-009. The sweep's new axis (the pacing proposal with an antitrust
  waiver and DOJ saying no lab has asked for a meeting) is real, but alignment was
  deep-dived on 2026-08-04.
- desire, score 14, desire-2026-08-04 confirmed on OpenAI's pre-announced
  rollout of ads in 31 European markets (24 Aug, announced 9 Jul). The sweep
  records ChatGPT's DSA designation as a Very Large Online Search Engine (31 Aug),
  Sponsored Agents (16 Sep) and the Amazon-Muse conflict, but desire was
  deep-dived on 2026-08-13 and six of its seven claims sit on slow calendars.
- labor, score 14, labor-2026-08-03 and -08-05 were falsified forward when
  Challenger's August report put AI fourth (3,462 of 52,881 cuts). That is one
  release, counted once. The Blizzard contract of 9 Sep advanced labor-2026-07-03
  to two of five. Held by staleness 2; coverage deadline 2026-12.
- security, score 14, The sweep has first-of-kind incident records (Spain's
  AEPD received its first breach notification of an attack executed by an AI
  agent on 14 Sep; the Medicare portal case; Plugin4Shell on 17 Sep). Its
  confirmations are two CAL-008 shares (security-2026-08-02, -08-05) and a thin
  security-2026-08-07. Held by staleness 2; coverage deadline 2026-12.
- dependency, score 13, Two of three confirmations are retrodictions
  (dependency-2026-07-02 on a Dec 2024 Character.AI control, -08-07 on a 27 Jul
  2026 SDK release), and the third is a one-third CAL-008 share. The sweep's new
  fact, the 3 Sep near-simultaneous outage at Anthropic, OpenAI and xAI, has no
  established shared cause, and the other items (GPT-5.5 leaving ChatGPT on
  14 Oct, 29 Anthropic incidents closed without root cause) are incremental.
  Backlog theme, must be selected by 2026-12. dependency-2026-08-02 (FSB final
  report due Oct 2026) should resolve before the next run.
- responsibility, score 13, Its only resolution, responsibility-2026-08-07, is a
  retrodiction on Amazon Agent Terms dated 30 May 2025. The sweep opens a new
  allocation route (Alabama's subpoena of OpenAI on 24 Aug and California's
  investigation over model conduct rather than user harm), but responsibility was
  deep-dived on 2026-08-04.
- truth, score 13, Zero of ten claims moved. The Goncourt's 25 Sep removal of a
  novel partly on statistical detection, and SB 1050 (signed 16 Sep), are strong
  new evidence outside every open claim. But truth was deep-dived on 2026-08-13.
- authority, score 12, authority-2026-08-05 is a same-day retrodiction on a
  bill whose Commission was amended out, and -08-08 met a low bar on a
  scheduled comment docket. The AI Office's first information requests (29 Aug
  and 1 Sep) are anonymous, so authority-2026-08-01 and -08-06 stay open.
  Deep-dived 2026-08-04.
- governance, score 12, The only resolution, governance-2026-08-05, was
  satisfied by a Texas AG page live on 2 Jul 2026, before logging. Every open
  claim resolves 2027-01 or later (CAL-007), and most substantive contradictions
  are outlet disagreements or unverified items. Staleness 2; coverage deadline
  2026-12.
- memory, score 12, Zero of nine claims moved in 43 days, a measured null. The
  world moved off the ledger: Darktrace's 24 Sep conversation-history poisoning
  disclosure across four harnesses, the Cologne court's 17 Sep Art. 9 consent
  holding and Google's provider-blind memory announcement of 23 Sep. Deep-dived
  2026-08-13.
- trust, score 12, trust-2026-08-05 is a CAL-008 half share and trust-2026-08-06
  a retrodiction (Gemini text watermarking documented May 2024). Beazley's
  affirmative AI cyber endorsement (17 Sep) and Kennedy's S. 5417 (blocked
  16 Sep) are incremental. Deep-dived 2026-08-04.
- coordination, score 11, coordination-2026-08-07 confirmed on the IETF
  agentproto charter moving to -00-03, the next procedural step (1), and -08-05 is
  a cluster share. The IETF approval ballot is set for 8 Oct, so
  coordination-2026-08-01 may resolve next run. Deep-dived 2026-08-04.
- autonomy, score 10, autonomy-2026-08-08 is a CAL-008 half share and
  autonomy-2026-08-11 a same-sweep retrodiction on Zenity's product page. The
  sweep's five-organisation incident count mostly measures disclosure lag for
  May to July behaviour. Deep-dived 2026-08-13.

## Coverage Status

| theme | last v2 deep dive | months since, to 2026-09 | after this selection |
|-------|-------------------|--------------------------|----------------------|
| intelligence | never (clock from 2026-07) | 5 (never) | selected this run, due again by 2027-02 |
| perception | never (clock from 2026-07) | 5 (never) | selected this run, due again by 2027-02 |
| learning | never (clock from 2026-07) | 5 (never) | selected this run, due again by 2027-02 |
| identity | never (clock from 2026-07) | 5 (never) | selected this run, due again by 2027-02 |
| belonging | never (clock from 2026-07) | 5 (never) | selected this run, due again by 2027-02 |
| agency | 2026-07-03 | 2 | selected this run, due again by 2027-02 |
| dependency | never (clock from 2026-07) | 5 (never) | backlog, must be selected by 2026-12 |
| meaning | never (clock from 2026-07) | 5 (never) | backlog, must be selected by 2026-12 |
| governance | 2026-07-03 | 2 | due by 2026-12 |
| labor | 2026-07-03 | 2 | due by 2026-12 |
| security | 2026-07-03 | 2 | due by 2026-12 |
| creativity | 2026-07-03 | 2 | due by 2026-12 |
| responsibility | 2026-08-04 | 1 | due by 2027-01 |
| alignment | 2026-08-04 | 1 | due by 2027-01 |
| authority | 2026-08-04 | 1 | due by 2027-01 |
| coordination | 2026-08-04 | 1 | due by 2027-01 |
| trust | 2026-08-04 | 1 | due by 2027-01 |
| autonomy | 2026-08-13 | 1 | due by 2027-01 |
| desire | 2026-08-13 | 1 | due by 2027-01 |
| memory | 2026-08-13 | 1 | due by 2027-01 |
| power | 2026-08-13 | 1 | due by 2027-01 |
| truth | 2026-08-13 | 1 | due by 2027-01 |

"Due by" is the month in which the theme reaches month 5 without a dive and
the coverage rule selects it regardless of score.

## Notes

**Cut rule.** Select every theme whose total is at or above the fifth-ranked
total, ties included, provided the result stays within 4 to 6. This is the rule
the 2026-08-04 and 2026-08-13 runs applied ("every theme scoring 18 or above",
where 18 was the fifth-ranked total). Here the fifth-ranked total is 16, held
jointly by agency and belonging, so six themes qualify and no theme is dropped.

**Tie-break**, used only if the inclusive set exceeds six or to order themes
below the cut. Apply in turn: higher staleness, then higher grade surprises,
then higher evidence delta, then alphabetical. It was not needed at the cut. It
orders the 15-point group below it as meaning (staleness 5), then creativity
(staleness 2), then power (staleness 1), which makes **meaning the first
alternate**.

**Sensitivity.** Under a literal count of contradiction bullets, every theme
scores 5 on that dimension. The fifth-ranked total then becomes 17, shared by
belonging, meaning and agency. That gives seven themes, and the tie-break drops
agency (staleness 2), so meaning takes the sixth slot instead of agency. The
other five selections are the same under either reading. The substantive-count
reading is used because unverified-item and outlet-dating bullets are not
contradictions in the evidence, and because the previous run's contradiction
scores were visibly not raw counts (for example, desire scored 4 on six bullets).

**Coverage plan.** Five of the seven never-dived themes are retired by this
selection. **Two backlog themes remain (dependency, meaning)**, due by 2026-12.
That deadline is safe: they fit in any single run, and a run in 2026-10, 2026-11
or 2026-12 can take both. To be conservative, the next run should select both
regardless of score, which also puts dependency-2026-08-02 (FSB report, Oct
2026) and meaning-2026-08-05 (AB 2575, decided by 30 Sep) in front of a deep dive
right after they resolve.

The tighter constraint is the re-dive clock rather than the backlog. Governance,
labor, security and creativity (2026-07 cohort) reach month 5 in 2026-12. With
dependency and meaning, that is six dives due by 2026-12, exactly one run at the
maximum of six. Had agency not been selected here, seven would be due, which no
single run could clear. Then all ten 2026-08 themes reach month 5 in 2027-01.
Across 2026-10 to 2027-01, 16 dives are due. That is feasible at five per run
only if a run happens every month (20 capacity). If a month is skipped, every
remaining run must take six (18 capacity).

**Duplicate new claims.** The six CAL-008 duplicate groups logged in Phase B
(for example, belonging-2026-09-01 and desire-2026-09-03 on a suit against SB
1119, and trust-2026-09-01 and truth-2026-09-03 on Anthropic's detector) are not
graded yet and did not affect any score. Deep dives on belonging and agency
should treat belonging-2026-09-01 and agency-2026-09-01 as shared with other
themes rather than as independent signals.

**Observations for instrument-review** (no method change made here):

1. Contradiction density still does not discriminate as written. Every sweep
   carries six to nine Counter-Signal plus Contradiction bullets, many of them
   hygiene records (unverified claims, outlet date conflicts). The skill should
   define what counts. Here the definition decided the sixth slot.
2. Evidence delta saturates at long intervals, 15 of 22 at 5 over 43 days, just
   as it bottomed out over the nine-day interval of 2026-08-13. Shared events
   also raise several themes at once (ChatGPT's DSA designation scores in
   authority, governance and desire; SB 1119 in belonging, desire and
   responsibility). A per-interval or relative scale, or single-theme attribution
   of shared events, would restore separation.
3. The skill gives no weights for grade surprises. This run had to define them
   from CAL-004, CAL-008 and CAL-009 (forward vs pre-announced vs retrodiction,
   cluster sharing). Weights should live in the skill so the dimension is
   comparable across runs.
4. The coverage rule's arithmetic is tight. Twenty-two themes on a 5-month
   window need at least 4.4 dives per month. The synchronized v2 start, and two
   2026-08 runs that spent capacity without adding calendar months, produce a
   10-theme wave due in 2027-01. The skill could let theme-selection use
   upcoming coverage deadlines as the first tie-break, or require six selections
   when the forward load demands it.
