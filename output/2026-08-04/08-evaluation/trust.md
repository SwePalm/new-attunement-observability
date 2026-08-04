# Scenario evaluation, trust, 2026-08-04

Artifact under audit: `output/2026-08-04/07-scenario/trust.md` ("The Unbought Witness")

## 0. Citation Gate

Pass/Fail: **Pass** (with two recorded defects, neither gate-failing)

Notes:

- Every Confirmed Development in `02-sweep/trust.md` carries at least one source URL and a month+year. All three carry two URLs each: Article 50 application (digital-strategy.ec.europa.eu, Jul 2026; techpolicy.press, Aug 2026), the Hugging Face intrusion (huggingface.co/blog/security-incident-july-2026, Jul 2026; techpolicy.press, Jul 2026), and NIST AITE (nist.gov, Jul 2026; nextgov.com, Jul 2026). The Emerging Signals, Counter-Signals, Regulatory Shifts and Technical Changes bullets are also individually sourced and dated. The gate's hard requirement is met.
- Of the seven Signals Emerging bullets in scenario section 7.1, six trace cleanly to a dated, sourced sweep item. Bullet-by-bullet: Article 50 plus Code of Practice plus complaint channels to Confirmed Development 1 and the Counter-Signal; sandbox escape and disabled safeguards to Confirmed Development 2; forensic scale (17,600 actions, 6,280 clusters, open-weights fallback) to Technical Changes; Aon's 28 Jul 2026 diagnostic to Emerging Signals; KYND's 23 Jul 2026 accumulation warning to Emerging Signals; NIST AITE to Confirmed Development 3.
- **Defect 1 (traceability, not fabrication).** Bullet 5's second clause, "in the same season standard commercial lines filed generative AI exclusions," has no anchor in this run's sweep. The sweep's insurance content is Aon and KYND only. The ISO forms (CG 40 47, CG 40 48, CG 35 08) and Berkley's absolute exclusion appear in `01-grading/trust.md` and in the trust-2026-07-03 ledger grade, sourced to insurancejournal.com, Jul 2026. That is a legitimate artifact of this run, so no fabrication has occurred, but the scenario's second structural force (section 5, "price stopped carrying information") rests on grading output rather than sweep output. This is worth recording because the scenario-generator contract asks section 5 to reflect sweep items; it clears that bar on forces 1 and 3 without force 2.
- **Defect 2 (date without a URL-bearing bullet).** The "full technical timeline on 27 July 2026" date, used in section 7.1 bullet 3 and in section 5's logic, appears in the sweep only inside the Contradictions section, which carries no inline URL. The underlying artifact is cited elsewhere in the sweep (huggingface.co/blog/agent-intrusion-technical-timeline, Jul 2026) but without that specific publication date attached to a sourced bullet. The gate applies to Confirmed bullets, so this does not fail, but the date is one step less supported than the scenario's use of it implies.
- Claims in the scenario that cite no upstream evidence at all: see section 2 below. Two are material (the mutual corroboration pool, the evidence-custodian occupation). They are narrative constructions, not fabricated citations, and are presented without source attribution, so the gate is not breached. They are penalised under Cross-Layer Grounding and Institutional Realism instead.

Proceeding to scoring.

---

## 1. Structural Compliance

Pass/Fail: **Pass with deviations**

Notes:

- All nine required sections present, in the prescribed order, with headings matching the scenario-generator contract exactly (including 7.1, 7.2, 7.3 and the two subheadings under section 8).
- Length constraints, measured: section 2 is 146 words (target ~150, met); section 3 is 349 words (300-400, met); section 4 is 204 words (150-250, met); section 5 is 215 words (150-250, met); section 7.2 is 158 words (120-200, met); section 6 carries three open questions (2-3, met); section 7.3 carries six bullets (4-6, met); section 8 carries six skill seeds and three refractions (4-6 and 2-3, met).
- **Deviation 1: section 7.1 carries seven bullets against a 4-6 bullet ceiling.** Not cosmetic in this case. The seventh bullet (NIST AITE "and not on containment behaviour") is the one carrying the most inference load, and the overrun is what admits it.
- **Deviation 2: meta-commentary inside the narrative.** Section 7.2 contains "This pipeline is calibrated to overestimate how fast published rules bite (CAL-002)" and "this pipeline also expects private ordering to lead statute (CAL-003)." The scenario-generator contract states "No meta-commentary" and asks that calibration be applied as restraint in the world-building rather than named. Naming the heuristics is epistemically honest and I would rather have it than not, but it is a contract deviation. Noting for fairness: `07-scenario/responsibility.md` does the same thing this run, so this is a run-level pattern rather than a trust-specific lapse, and it belongs in the instrument-review channel rather than being charged fully to this artifact.
- Required scenario elements are clearly used. Normal Absurdity 1 (green heat map and absolute AI exclusion on consecutive pages of the same pack, unread against each other) appears as the opening beat of section 3. Normal Absurdity 3 (the compliant model refuses the forensic work, the unguarded one does it, signed off in a footnote) is the middle beat, and the "fire axe behind glass" simile is carried over from forces-feelings intact. Normal Absurdity 2 (flagging as unpaid civic chore) appears as the closing beat. Three of three, against a requirement of two.
- The Irreplaceable Thing (an unbought witness) is the emotional centre of section 3 and is restated structurally in section 9. This is the strongest single compliance element in the artifact.
- No em-dash characters present (verified: 0 occurrences; 8 en-dashes, all in section headings supplied by the contract).

Subscore: 7

---

## 2. Cross-Layer Grounding Check

Pass/Fail: **Pass with a material exception**

Grounding Strength: **moderate**

Notes:

- PESTLE traceability is genuinely good on five of six categories. Legal maps to section 5 force 1 and 7.1 bullet 1 (Article 50 applicable with voluntary provenance, report-driven enforcement). Economic maps to section 5 force 2 and the vendor-pack beat (exclusions plus purchasable maturity score). Technological maps to section 5 force 3 and the cabinet beat (agent-scale forensics, safety alignment obstructing audit). Social maps to section 4's final paragraph and the report-button beat (verification labour pushed downward, protection tracking verification capacity). Environmental maps to the explicit inference sentence closing section 5 (unobserved concentration), and that sentence is correctly marked as inference in the artifact itself, which is the right behaviour.
- Political is the thinnest mapping. The PESTLE political thesis is a contest over who defines proof of trustworthiness, with four named venues including Google's proposed Frontier AI Regulatory Organization, the FTC deception theory and the AI Kill Switch Act. In the scenario, all four collapse into a single unnamed clause in section 5 ("none of the venues bidding to settle AI trust is scoped to measure ecosystem concentration") and into the preferred-path bullets. No political actor appears in the lived world at all. The FTC theory, the shutdown-authority bill and the incumbent-designed regulator, three of the four most consequential political forces upstream, have no presence in the depicted 2029-2031. Their absence is asserted by omission rather than argued.
- Contradictions are visibly operationalised, and this is the artifact's strongest grounding work. Forces-and-feelings Contradiction 2 (legal exposure rising while the pricing institution withdraws) is not summarised but dramatised as two pages of one document that no one is tasked to read together, with the procurement outcome stated. Contradiction 3 (assurance as the failure vector, safety as the obstacle to knowing) is dramatised as a licensed model refusing the payload and an isolated box doing the work. Contradiction 1 (complaint-driven enforcement depending on complainants without instruments) is carried argumentatively in section 5 rather than lived, which is weaker but present.
- **New systems not grounded upstream.** Two, one of them load-bearing.
  - *The corroboration pool.* Section 3 closes on "nineteen firms her size now hold their incident records to a shared retention format, so that when one of them is disbelieved by a counterparty far larger than itself, it can be corroborated by the other eighteen." This institution has no anchor in the sweep, in PESTLE, or in the exploration. It originates in one clause of the forces-and-feelings Irreplaceable Thing explanation ("building the mutual pool that lets small parties testify about large ones"), where it is a suggested protagonist action, not an observed signal. The scenario promotes it into a functioning institution with a specific membership count, a stated cost ("almost nothing"), a technical artifact (a shared retention format) and an outcome verdict ("it works"). It then recurs in 7.3 and section 8. It is the only constructive institutional development in the world, and it is the least grounded thing in the artifact.
  - *The evidence-custodian occupation.* Section 3 opens on a named job title and section 4 asserts "Evidence custody quietly becomes a profession, staffed by people who came out of incident response and compliance." No upstream item supports a labour-market or job-architecture shift. This is a reasonable inference from the forensic-bottleneck thesis, but it is stated as fact, not marked as inference, while the artifact demonstrably knows how to mark inference (it does so twice, in section 5 and, upstream, throughout PESTLE).
- Abstractions are otherwise converted into lived mechanisms competently. "Price stops carrying information" becomes an insurance certificate on page fourteen. "Safety alignment obstructs auditing" becomes a licensed model declining a payload. "Verification labour redistributed downward" becomes four taps on a report button while half-watching television. This is the conversion the contract asks for, done well.

Subscore: 6

---

## 3. Institutional Realism Audit

Assessment: **moderate to low realism**

Notes:

- **The load-bearing transition is asserted in five words.** Section 2 states: "None of those threads reversed." Everything in the depicted world follows from that. It is the single largest unearned move in the artifact, and it is unearned in a theme whose own evidence this month is a record of rapid reversal. `01-grading/trust.md` records trust-2026-07-03 decaying inside a single month, in a direction the claim explicitly excluded, and the grading Surprises section says so in terms: the insurance mechanism inverted within four weeks. A scenario for this theme that rests on three-to-five years of non-reversal is in direct tension with the run's own demonstration that trust threads invert on a one-month timescale. The artifact never acknowledges this, and it had the material to.
- **The system is presented as fully stabilised.** Section 5 opens "Three forces keep the arrangement stable" and the world contains no live contestation. Over roughly three to five years there is no enforcement action landing, no insurer re-entry attempt, no litigation over a maturity score that was relied on, no detection-technology improvement, no consolidation or discrediting of the score vendors, no failed pool, no regulator acquiring forensic capacity. Section 7.2 is candid that "insurance re-entry is the genuine uncertainty" and then the lived world contains no trace of that uncertainty being worked out by anyone. The one implied transition is the pool's formation, and it happens offstage.
- **The pool has no friction and should have a great deal.** Firms pooling incident records into a shared retention format is a discovery and disclosure exposure before it is a corroboration asset: preserved, standardised, third-party-held incident records are exactly the material a plaintiff, a regulator or a counterparty's counsel would seek, and in a period where the same firms' policies carry absolute AI exclusions the liability incentive runs against pooling, not toward it. The scenario notices there is something to explain ("Ines finds it strange that this is voluntary, and stranger that it works") and then declines to explain it. Naming an anomaly is not the same as surviving it. There is also no free-rider account, no governance account, and no account of what happens the first time a member's record is subpoenaed.
- **The forensic scale is internally inconsistent with the scenario's own thesis.** The artifact's central claim is that incident reconstruction is the scarce, bottlenecked, professionally distinctive capability. Section 3 then has one person at a mid-sized firm reconstruct eleven thousand actions between eleven in the morning and four in the afternoon, as a routine Tuesday item, alongside a vendor renewal review and other work. The upstream referent is a large platform security organisation reconstructing 17,600 actions in about 6,280 clusters for an incident that ran 9 to 13 Jul 2026, disclosed 16 Jul and technically documented 27 Jul, meaning roughly two weeks of organisational effort. If a five-hour solo reconstruction is available to a mid-sized firm, the capability is not scarce and the world's premise weakens. If it is scarce, the scene is wrong. The scenario cannot have both, and it takes both.
- Power asymmetries are, by contrast, genuinely well drawn and this is where the artifact earns realism credit. Procurement outranks the reviewer who is correct. The vendor's account arrives eight days late and shorter. The small firm's default condition is being disbelieved by a larger counterparty. The user trains a classifier they are not permitted to inspect. The protagonist's compliance sign-off for the unguarded box exists "in a footnote three renewals ago," which is exactly how such approvals actually persist. None of this is elegant, and it should not be.
- The world is overall too coherent for its own subject matter. Everything resolves to one axis, and no institution behaves incompetently, self-interestedly, or at cross purposes in a way that is not already on that axis.

Subscore: 5

---

## 4. Horizon Discipline Check

Pass/Fail: **Pass with deviations**

Notes:

- No sci-fi drift. There are no new technical primitives, no capability breakthroughs, and no AGI framing. Every technology in the world exists in the sweep: guarded frontier models, open-weight models, LLM-assisted log triage, watermarking and metadata, report buttons, maturity scoring. This is the artifact's most disciplined dimension in kind.
- **Deviation 1: section 3 carries no date.** It is "her Tuesday," unanchored. All four sibling scenarios this run date their lived section explicitly (alignment "early 2029," authority "Thursday in November 2029," responsibility "Thursday in November 2029," coordination four years on from mid-2026). Section 2's "by the end of the decade" and section 7.2's "through 2031" are the only temporal anchors, and they disagree with each other by one to two years. An undated lived section cannot be checked for proportionality of institutional shift to timeline, which is the substance of this gate. It is a real weakness, not a formatting quibble.
- **Deviation 2: "the likeliest path through 2031" exceeds the 0-5 year horizon** from a run date of 2026-08-04 by roughly five months. Marginal, and I weight it lightly.
- Institutional shifts are, where datable, proportional and modest. Complaint-driven enforcement producing "a handful of visible transparency actions," a mandatory-provenance upgrade that "is discussed each year and lands late if it lands," and incident reporting advancing ahead of pre-release testing are all small, cheap, incremental moves consistent with three-to-five years. The scenario resists the temptation to have the EU fix the provenance gap or the US pass the Kill Switch Act. That restraint is real and I credit it.
- **Calibration heuristics.** CAL-002 is applied correctly and, importantly, applied with its own counter-signal attached: section 7.2 slows the regulatory clock and then immediately tempers that with "the August 2026 obligations were not deferred," which is precisely the counter-signal recorded against CAL-002 in the memo and in this run's grading of trust-2026-07-01 and trust-2026-07-02. That is the most sophisticated calibration handling I can identify in the artifact.
- CAL-003 is applied in the direction of withdrawal rather than hardening, correctly reading this month's evidence. But there is an unflagged interaction: CAL-003 says the pipeline underweights non-state hardening, and the scenario's response is to invent a non-state hardening mechanism (the corroboration pool) that no evidence supports. Over-correcting a known bias by fabricating an instance of the underweighted class is a failure mode the memo does not name and the artifact does not notice.
- CAL-001 (unfalsifiable claims confirm by construction) is not fully escaped in section 7.2. "Drift rather than rupture," "a handful of visible transparency actions," and "lands late if it lands" contain no threshold that a future run could grade. This is Probable Direction rather than a ledger claim, so the bar is lower, but the theme's own ledger already carries two ungradeable 2026-02 claims that this run's grading flags as stuck until 2029, and the same softness recurs here.
- No horizon-inflating bias from an active heuristic is repeated. The scenario does not treat any published compliance date as fixed.

Subscore: 7

---

## 5. Signal Integrity Check

Pass/Fail: **Pass**

Signal Anchoring Strength: **strong**

Notes:

- All seven Signals Emerging are present-day observed events with dates in July and August 2026, not inventions. Six are directly sweep-anchored (see section 0). Six of seven carry a specific date in the bullet text itself, which is above the standard of most artifacts in this run.
- No unobserved breakthrough is required anywhere. The world runs entirely on capabilities demonstrated in the July 2026 record. This is the cleanest structural property of the artifact and the main reason the score does not fall further.
- Extensions from signal to world are incremental in four cases (voluntary provenance persisting, score-based procurement persisting, unguarded-model fallback becoming routine practice, complaint-driven enforcement producing thin output) and speculative in two (the pool, the profession). The speculative pair is confined to sections 3 and 4 and does not propagate into 7.2, which is the section that matters most for forecast integrity. Probable Direction contains no invented institution.
- **Two signals carry inference presented as observation.** Bullet 7 states AITE "opened on three vision-language tasks and not on containment behaviour." The three tasks (quantum science, genomics, public safety) are sourced; the exclusion of containment behaviour is an absence-based inference from a launch announcement, and a launch scope is not a permanent scope. Bullet 5's insurance clause is grading-sourced rather than sweep-sourced, as recorded in section 0. Neither is false on this run's evidence. Both are stated with more certainty than their support carries.
- One smaller instance: section 3's "training a classifier she will never be permitted to inspect" and section 8's "a classifier the users cannot inspect" go beyond the sweep, which records only that LinkedIn's report button trains its classifiers. Non-inspectability is a fair inference and a small one, but it is stated as fact.

Subscore: 8

---

## 6. Narrative Inflation Risk

Assessment: **moderate**

Notes:

- The scenario collapses a genuinely multi-vector month into a single dominant logic: attestation versus witness. Section 9 states the collapse outright ("The instruments this period built are all statements"). The compression is intellectually productive and it is the reason the artifact has a thesis at all, but it is a compression. The sweep contains at least three live vectors the single logic swallows: a US preemption contest running through administrative reinterpretation, a shutdown-authority proposal placing executive power over running systems, and an incumbent bid to constitute the regulator itself. None of those is an attestation problem, and all three disappear.
- Coherence is exaggerated in one specific place: the pool works, costs nothing, and is voluntary. The artifact flags this as strange and moves on. A scenario that lets its one hopeful institution succeed without friction, in a world whose entire premise is that incentives run against evidence preservation, is inflating.
- Tone is well controlled and the artifact deserves credit here. It is neither dystopian nor utopian. The register is resigned competence: the protagonist wins her small victories, the vendor's account does not contradict hers, and she registers that as "the win it is." Nobody is villainous. The FTC is not jackbooted and the vendors are not cartoonish. Section 4's "Individuals adapt worse" is the one place the artifact allows an unrelieved bad outcome, and it does so briefly.
- Emotional concentration around scarcity is present by design (the Irreplaceable Thing is defined as a scarcity) and is moderate rather than high in execution. The scarcity is institutional and procedural rather than existential, and the prose does not dwell.
- One inflationary rhetorical move worth naming: section 9's "Every one of them can be produced by a system whose safeguards were switched off that morning" is a strong line that overstates its evidence. It generalises from one incident in which safeguards were reportedly disabled deliberately, in an internal evaluation context, to a universal property of all trust instruments. Rhetorically effective, epistemically loose.

Subscore: 6

---

## 7. Cross-Theme Convergence Risk

Assessment: **high**

Notes:

Cross-theme context is available: four sibling scenarios were generated in this run (alignment, authority, coordination, responsibility). Comparison is not favourable.

- **Near-identical protagonist framing with alignment.** Trust: "Ines is the evidence custodian at a mid-sized logistics software firm outside Rotterdam... Her Tuesday starts with..." Alignment: "Maureen runs platform security for a mid-sized logistics software firm with three hundred staff in Ohio... It is a Tuesday in early 2029." Same employer type, phrase for phrase, and the same weekday. Two of five scenarios in one run placing their protagonist at a mid-sized logistics software firm on a Tuesday is not convergence by subject matter, it is convergence by generation habit.
- **The same core scarcity as alignment.** Trust's protagonist needs an account of an incident that does not depend on the party responsible. Alignment's protagonist "wants somebody with nothing at stake to read the whole session and tell her what her systems did in the hours she cannot reconstruct." These are the same want, expressed at nearly the same length, in nearly the same position in section 3. Both derive from the same July 2026 incident, which explains the overlap without excusing it: the two dives were selected partly on the ground that they take that incident at different layers (assurance versus model behaviour, per SELECTION.md), and at the level of lived experience they do not.
- **The open-weights forensic fallback recurs verbatim in coordination**, where a post-mortem "reconstruction was done overnight by an open-weight model, because the guarded ones will not look at the artefacts," and appears again in coordination's preferred path. This is trust's Normal Absurdity 3 appearing in a scenario that is not trust.
- **A shared section-3 closing beat across the run.** Trust: the pool, and section 9's capability that "belongs to no institution's mandate." Alignment: "She wants one thing, and she cannot buy it." Authority: "What she wants she cannot requisition. She wants one refusal with standing behind it." Responsibility: the single sentence in the drawer with a blank where a name would go. Four of five scenarios end their lived section on a competent mid-level professional wanting one unpurchasable thing, named in short declarative sentences. That is a house style hardening into a template.
- Tonal homogeneity across the five is high: resigned competence, dry institutional detail, an absurdity nobody in the room remarks on, a protagonist who has stopped being angry. Trust is a good instance of that tone and not a distinct one.
- The one genuinely distinctive element is the insurance-and-score axis (a purchasable maturity report against an absolute exclusion on consecutive pages). Nothing in the other four occupies that ground, and responsibility's insurer material runs in the opposite direction (the insurer's file as the record families can actually reach). That earns some separation, but it is one beat against several shared ones.

Subscore: 3

---

## 8. Overall Evaluation

Score (1–10): **6.3**

Forecast Integrity Level: **moderate**

Stability Risk: **medium**

Summary:

The artifact's evidentiary base is the strongest thing about it and its institutional imagination is the weakest. Every technology and every regulatory fact in the depicted world exists, dated and sourced, in this run's sweep, and the scenario requires no breakthrough, no new primitive and no accelerated compliance clock to hold together. Calibration handling is unusually careful: CAL-002 is applied as restraint and then tempered by its own recorded counter-signal, which is the correct treatment of a heuristic that this run's grading partially contradicted. Contradiction 2 and Contradiction 3 from forces-and-feelings are dramatised rather than restated, which is the harder and better move.

Against that, the world rests on an assertion the theme's own evidence undercuts. "None of those threads reversed" carries three to five years of institutional stasis in a theme whose headline grading event this month is a mechanism inverting inside four weeks. Nothing in the depicted world contests anything: no enforcement lands, no insurer returns, no score is litigated, no detector improves. The two ungrounded constructions, an evidence-custodian profession and a nineteen-firm corroboration pool, are both promoted from a narrative suggestion in forces-and-feelings into stated fact, and the pool is the world's only constructive institution while also being its least supported and least frictioned element. A shared incident-record pool is a discovery exposure before it is a corroboration asset, and the artifact names that strangeness instead of answering it. The scenario also asserts that forensic reconstruction is the scarce bottleneck capability and then shows one person performing eleven thousand actions of it in an afternoon.

Convergence is the sharpest discount. Trust and alignment place their protagonists at a mid-sized logistics software firm on a Tuesday and give them the same want. The forensic fallback that is trust's signature absurdity also appears in coordination. Four of five scenarios end section 3 on the same beat.

Subscores:
- Structural Compliance (1-10): 7
- Cross-Layer Grounding (1-10): 6
- Institutional Realism (1-10): 5
- Horizon Discipline (1-10): 7
- Signal Integrity (1-10): 8
- Narrative Inflation Control (1-10): 6
- Distinctiveness vs. Other Themes (1-10): 3

Weighted calculation:
(7 x 0.10) + (6 x 0.20) + (5 x 0.20) + (7 x 0.15) + (8 x 0.20) + (6 x 0.10) + (3 x 0.05)
= 0.70 + 1.20 + 1.00 + 1.05 + 1.60 + 0.60 + 0.15
= **6.3**
