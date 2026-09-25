# Scenario evaluation, agency, 2026-09-25

## 0. Citation Gate

Pass/Fail: **Pass**, with two recorded defects (one load-bearing).

Notes:

- Every bullet in the sweep's Confirmed Developments section carries at least one source URL and a month and year. Five of the six carry two independent URLs: the KYA framework (pymnts.com and technode.global, Sep 2026), Agent Pay (fortune.com and itechpost.com, Sep 2026), the China Payment and Clearing Association convention (news.cn, Aug 2026, and 21jingji.com, Aug 2026), the Amazon block of Muse (techcrunch.com and retaildive.com, Sep 2026), the Hugging Face incident reports (fortune.com and metr.org, Aug 2026) and GoCardless (fintech.global and openbankingexpo.com, Sep 2026). Emerging Signals, Counter-Signals, Regulatory Shifts, Capital Movements and Technical Changes are likewise sourced and dated. The sweep's own Contradictions section records three hygiene items (the forum of the Perplexity amended complaint, the date of the Beijing standard, and unverified Alipay volume figures that were not used); none of the three is used by the scenario.
- All six Signals Emerging bullets trace to dated, sourced sweep items: the KYA announcement (Confirmed, 10 Sep 2026), Agent Pay and Mastercard's liability answer (Confirmed, 18 Sep 2026), the Ninth Circuit denial and the Muse block (Regulatory Shifts and Confirmed, Sep 2026), the Chinese convention (Confirmed, 24 Aug 2026), Visa's CEO and the 7% survey (Counter-Signals, Sep 2026), and GoCardless under AI Live Testing (Confirmed, 22 Sep 2026). None is invented and the dates match the sweep.
- Grading-file and ledger provenance is used and, in the upstream files, labelled as such: the absence of an agent flag in card dispute codes comes from the 2026-09-25 grade on agency-2026-07-02, not from the sweep, and the open status of the HM Treasury consultation comes from the grade on agency-2026-08-01. PESTLE labels both. Section 8 of the scenario states the first as a present fact without its provenance being visible, which is legitimate but grading-sourced.
- Defect 1, load-bearing: the mechanism the entire scenario turns on, that the agent drafts a structured mandate summary from the user's words and the user approves the summary rather than their own instruction, is not in any upstream evidence. The sweep establishes that Agent Pay offers limits, merchant restrictions and approval before checkout, and that Verifiable Intent documents what was authorised. It does not establish who writes the mandate text or whether raw instructions are retained. PESTLE Technological force 3 correctly flags this as "inference from the sweep's absence of any such standard; not verified". The scenario's section 8 then states, as a present-day refraction, that Agent Pay's controls "are configured from a structured description of what the user wants". An inference labelled as such upstream has been promoted to present fact in reader-facing prose. The gate is scoped to Confirmed bullets and passes on its literal terms; the 2026-08-13 memory evaluation flagged the same pattern (a load-bearing mechanism resting on no source) and it recurs here.
- Defect 2: in-world forecasts presented without upstream grounding. The FCA letter states that HM Treasury "has published proposals" by Feb 2028. That is a bet that agency-2026-08-01 resolves (at least partially) inside its window. Section 7.2 declares it as the realistic middle case, which is the correct handling, but it is still a forecast carried into the narrative as fact. The availability of an Agent Pay-style agent card at a UK bank by late 2027 is also inferred (the sweep does not state Agent Pay's geography).
- Claims with no upstream evidence at all: Rotherham, the scooter, the battery specification, Dunmore Mobility, Errand Ltd, the voice note, the 38 confirmations, and the FCA's stated inability to resolve individual complaints. The first seven are narrative particulars. The last is an accurate description of the FCA's general remit as the evaluator understands it, but it was not verified in this run.

---

## 1. Structural Compliance

Pass/Fail: **Pass**

Notes:

- All nine sections present, in order, headings matching the contract exactly, including 7.1 to 7.3 and both subsections of section 8.
- Measured lengths: section 2 at 154 words (target approximately 150), section 3 at 355 (300 to 400), section 4 at 197 (150 to 250), section 5 at 197 (150 to 250), section 7.2 at 182 (120 to 200). Section 6 has three questions, 7.1 six bullets, 7.3 six, Skills five, Signals and Refractions three. All within bounds, with margin rather than on the ceiling.
- All three Normal Absurdities appear in section 3, not just the required two: signing one's own paraphrase (the mandate summary approved at 07:52, three minutes after the voice note), knowing which assistant a shop admits (the merchant's note that the cardholder's previous assistant was refused on 4 October), and confirmation volume (38 approvals in the week). The Irreplaceable Thing (one's own words read back and taken as the measure by someone who can act) is the pivot of the file: the escalations letter is the only document that quotes the customer and the only one that moves the loss.
- The assigned form is obeyed: the section is a single case file passing between customer, merchant, card network, agent provider and regulator, one document per party (the provider has two, which is the movement of the file rather than a breach of form). The review constraints are respected: it does not open on a professional at a desk, the narrative runs Nov 2027 to Feb 2028 rather than 2029, and no calibration heuristic or the pipeline is named in reader-facing prose. Section 9 closes on a structural statement rather than a named scarce good. Section 3, however, closes on a one-line beat naming the scarce thing ("the only page in the file that quoted her"), which is the house cadence previous evaluations flagged, moved from section 9 to the end of section 3.

---

## 2. Cross-Layer Grounding Check

Pass/Fail: **Pass**

Grounding Strength: **moderate**

Notes:

- The institutional systems in the narrative trace to PESTLE: the intent record and cardholder-liable decision to Technological 1 and Legal 3, the merchant's agent-access terms and refusal of an unidentified assistant to Legal 2 and Technological 2, the FCA's testing of final-approval designs to Political 2, the Treasury proposals to Political 1, provider-level allocation to Economic 4 and the Chinese contrast to Legal 4. The recurring and replacement purchase context is Environmental 1 and 2.
- The contradictions are operationalised. Contradiction 1 (the approval as safeguard and as signature) is the network's decision, which rests entirely on the 07:52 tap. Contradiction 2 (better proof of authorisation into a gap about meaning) is the whole sequence of merchant and network documents. Contradiction 3 (the principal as author of record and least informed party) is the customer's form, which must argue "not authorised" against her own signature.
- The grounding weakness is the one recorded in section 0: the agent-drafted mandate summary is the hinge of the entire file and it is inference, not evidence. The chain is internally honest about this up to PESTLE and loses the label at the scenario.
- A second, smaller gap: the scenario uses the agent's substitution ("same or equivalent") as the failure mode. Nothing upstream reports substitution disputes; Environmental force 2 flags it as inference. It is a reasonable choice of failure, but it was chosen, not observed.
- No new major institution is introduced. The two fictional firms are small and generic; the FCA and HM Treasury are upstream.
- The theme's other limb is absent. All three of this run's agency confirmations (OpenAI's post-mortem, Irregular's account, Amazon's rehearing petition) concern containment incidents or access litigation, while the three commerce claims have graded open three times. The scenario builds on the limb with zero confirmations and a premise (transaction volume) that Visa's CEO says does not yet exist. It handles this by keeping volume and dispute counts low, which is the correct adjustment, but the forecast rests on the less evidenced half of the theme.

---

## 3. Institutional Realism Audit

Assessment: **moderate realism**

Notes:

- Friction is present and located sensibly. The customer must pick a reason code that does not fit; the merchant's representment is procedurally correct; the network's decision follows from the codes it has; the regulator states the limit of its remit; the provider's first reply is a template and the second is discretionary. Nothing works as designed and nothing is malicious.
- Power asymmetries are visible: the provider holds the only record of the customer's words and decides whether to retrieve it; the merchant defines which agents may enter; the network's outcome is the one that is recorded.
- Two realism problems, both from the evaluator's own knowledge rather than from upstream, and both unverified in this run. First, the file conflates issuer and network: a first-cycle card dispute is decided by the issuing bank, with the network involved only at arbitration, so a "card network" decision within seven weeks is compressed. Second, and more serious, a UK consumer buying goods at a distance ordinarily has a statutory cancellation right for a period after delivery. The customer filed two days after delivery, and the simplest remedy in the actual UK setting would likely have been to return the batteries, not to dispute the payment. The scenario never mentions it. If that route exists, much of the file's machinery is unnecessary for this case and the scenario's chosen failure (a returnable good) is weaker than a non-returnable one would have been. This does not break the structural argument, which is about who is deemed to have authorised, but it reduces realism for the specific case.
- Transitions are implied rather than stabilised: the Treasury proposals exist and are not in force; the KYA framework is not mentioned as operative; the provider's goodwill does not become policy. The world is not presented as settled.
- Elegance is moderate. Each party's document demonstrates one property of the rails, which risks the syllabus shape recorded against truth in 2026-08-13, but the documents also disagree and the loss moves, so the file has a trajectory rather than a list.

---

## 4. Horizon Discipline Check

Pass/Fail: **Pass**

Notes:

- Horizon is 14 to 17 months from the run date, inside 0 to 5 years, and justified in 7.2 by the consultation calendar and slow adoption.
- No science-fiction drift. Every capability used (agent virtual cards with limits and approval, intent records, merchant identification of agents, voice instructions) exists today in some form. The agent-drafted summary is inference, but it is an incremental design choice, not a breakthrough.
- Probable Direction is plausible: slow volume, approval as default, no dispute wave, private allocation first. This is consistent with the three open grades on agency-2026-07-01, -07-02 and -08-02.
- Calibration checks. CAL-002 is applied as restraint: the British rule exists only as proposals needing legislation by Feb 2028, and 7.2 argues that timing without importing private vocabulary. CAL-003 is applied: private rulebooks and provider goodwill allocate the loss before statute. CAL-007 is respected by not making the scenario hinge on any claim's resolution date. CAL-006 is respected in choosing the FCA's testing programme, the channel that actually moved, rather than a formal rulemaking as the regulator's point of contact.
- Two undeclared or partly declared bets. The scenario bets that agency-2026-08-01 resolves at least partially (Treasury publishes proposals) and says so in 7.2 as the middle case; it bets implicitly that agency-2026-09-02 (a KYA document with certification requirements) either does not arrive or does not address mandate drafting, and 7.2 only asks readers to watch for it. It also bets implicitly against agency-2026-07-02 within the window, which is consistent with the grades.

---

## 5. Signal Integrity Check

Pass/Fail: **Pass**

Signal Anchoring Strength: **moderate**

Notes:

- All six Signals Emerging bullets are present-day, dated and traceable. They are rephrased, not embellished; the one compression (Mastercard "pointed to its intent record rather than a rule") matches the sweep's wording ("pointed to its Verifiable Intent paper trail without specifying ultimate liability").
- Section 2 overstates one signal: "A US appeals court had already held that when an agent browses, it is the user who acts." The holding upstream is narrower, that the user rather than the provider "accesses" the site for the statute in question. "Acts" generalises a statutory attribution into a general one.
- Extensions from signal to world are mostly incremental: approval defaults persist, dispute codes stay unchanged, Treasury proposals are published but not in force, providers settle privately. The one extension that is a speculative construction (the mandate summary drafted by the agent) is the load-bearing one, and it is presented in section 8 as present fact, as recorded in section 0.
- No unobserved breakthrough is required.

---

## 6. Narrative Inflation Risk

Assessment: **low to moderate**

Notes:

- Tone is procedural and restrained. No party is villainous, the customer is refunded, the regulator is accurate, and the loss is small (£186.40) with a proportionate harm (a man stranded at a garden centre). The scenario declines both dystopia and rescue.
- Complexity is collapsed to one logic, attribution of the act to the principal, and several upstream vectors disappear: Alipay's measured adoption growth appears only in 7.2 as a swing variable, the Beijing dual authorisation rule is absent, Amazon's own opt-out enrolment of retailers (the sweep's sharpest contradiction on consent) is absent, and the containment-incident limb is absent entirely.
- Section 9's claim that the question "will be decided in provider support queues long before it is decided anywhere a second customer could cite" is plausible and slightly overstated: it generalises from one invented case to the whole dispute system, and card network arbitration outcomes, while not public, are not purely one-off.
- Emotional concentration on scarcity is moderate. The Irreplaceable Thing is dramatised once, in a single letter, and named in one closing line of section 3; section 9 does not return to it as a named good.

---

## 7. Cross-Theme Convergence Risk

Assessment: **moderate**

Notes:

- Comparison basis: this run's belonging, intelligence, learning and perception scenarios (section 3 openings and section 9 read), the 2026-08-13 autonomy and truth scenarios and evaluations, and the 2026-07-03 agency scenario.
- Against the 2026-07-03 agency dive, the movement is distinct. That scenario's movement was an individual reclaiming authorship of consequential choices through a literacy ("keeping the pen") while persuasion moved upstream into agent ranking. This one concerns the legal attribution of the agent's act to the person and the allocation of loss when the agent's mandate misstates the person; the protagonist does not reclaim a choice, she contests a paraphrase. One residual echo: section 4's minority who dictate redundantly and switch off substitution, while "most people do not change", is the 2026-07-03 literacy divide in a new setting.
- Form convergence is real and partly structural. The assigned case-file form resembles the 2026-08-13 autonomy scenario, whose section 3 was also a sequence of institutional documents with identifiers. The documents here disagree and the loss moves, whereas autonomy's documents were all accurate and static, but a reader of both would see the same device.
- The "record of an AI incident is controlled by the party least interested in publishing it" attractor, which the run instruction asked to be checked explicitly: the scenario does not reach it as its conclusion, but it touches it. The decisive record (the customer's own words) is held by the agent provider, the party whose error it reveals, and the correction stays private ("appears in no dispute statistic and binds no other case"). The evidence genuinely supports part of this: Mastercard's answer on liability was a paper trail it holds, and no dispute code counts agent cases (grading file). The difference is that the provider here retrieves the record against its own interest and pays, so the holding party is not the obstacle. Still, the closing emphasis on private settlement not becoming public knowledge sits adjacent to the attractor and to autonomy-2026-08-13's ending, and should be counted as partial convergence rather than as an independent finding.
- Same-run convergence: two further shared logics. Intelligence's section 9 concludes that the operative promise was being made "by lenders, tenders and courts, well before any legislature arrived at it"; this scenario concludes that providers' support queues decide before any citable forum. Both are the private-ordering-ahead-of-statute reading, which CAL-003 makes the pipeline's default expectation and which now appears as a conclusion in at least two of this run's scenarios. Belonging's section 9 argues that instruments record what the system said rather than what became of the person; this scenario argues that the rails record what was authorised rather than what was meant; truth-2026-08-13 argued that both instruments answer an adjacent question. "The instrument measures the adjacent, countable thing" is becoming a house thesis.
- Protagonist shape repeats: a low-power individual assembling a file against institutions (Delia in responsibility, Lorna in truth, Ines here). The aphoristic section 9 summation, recorded as the house ending, is softened here but present.

---

## 8. Overall Evaluation

Score (1–10): **7.1**

Forecast Integrity Level: **moderate**

Stability Risk: **medium**

Summary:

The artifact's epistemic strength is its choice of hinge. The sweep documents, within a single month, rails that record authorisation with increasing precision (the KYA framework, Agent Pay, Verifiable Intent), a court that attributes the agent's access to the user, a network that answers the liability question with a paper trail, a supervisor whose first-hand evidence comes from the final-approval design, and a Chinese rule that allocates the loss the other way. The scenario converts that into one small, proportionate dispute in which each party's document is correct on its own terms and the loss still has to go somewhere, and it keeps the clocks slow in the way the grading record demands: no dispute wave, proposals not in force, adoption low. The movement is distinct from the theme's previous dive.

Four weaknesses hold the score near seven. The mechanism the file turns on, an agent-drafted mandate summary that the user approves instead of their own instruction, is inference that PESTLE labels as such and the scenario then states as present fact in section 8. The specific case ignores what is probably the simplest UK remedy (returning a distance-sold good), and compresses the issuer and network roles. The forecast is built on the half of the theme that has graded open three times, not on the half that confirmed. And the conclusion leans into two logics now shared across this run and the last (private ordering ahead of statute; the instrument recording the adjacent thing), and touches the private-record attractor the run asked to be watched.

Stability risk is medium. If a KYA specification or a provider term defines how mandates are derived from user instructions, or if Treasury allocates the loss to providers early, the world's premise weakens quickly; the attribution argument would survive.

Subscores:
- Structural Compliance (1-10): 9
- Cross-Layer Grounding (1-10): 7
- Institutional Realism (1-10): 6
- Horizon Discipline (1-10): 8
- Signal Integrity (1-10): 7
- Narrative Inflation Control (1-10): 7
- Distinctiveness vs. Other Themes (1-10): 6

Scoring Method:
- Structural Compliance 9 x 0.10 = 0.90
- Cross-Layer Grounding 7 x 0.20 = 1.40
- Institutional Realism 6 x 0.20 = 1.20
- Horizon Discipline 8 x 0.15 = 1.20
- Signal Integrity 7 x 0.20 = 1.40
- Narrative Inflation Control 7 x 0.10 = 0.70
- Distinctiveness vs. Other Themes 6 x 0.05 = 0.30
- Weighted total: 7.10, reported to one decimal place as 7.1
