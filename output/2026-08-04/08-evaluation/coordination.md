# Scenario evaluation, coordination, 2026-08-04

Artifact under audit: `output/2026-08-04/07-scenario/coordination.md` ("The Name in the Field")
Upstream chain audited: `02-sweep/coordination.md`, `01-grading/coordination.md`,
`03-structural-question`, `04-exploration`, `05-pestle`, `06-forces-feelings`,
`ledger/coordination.md`, `ledger/CALIBRATION.md`.

---

## 0. Citation Gate

Pass/Fail: PASS

Notes:

- All three Confirmed Developments in the sweep carry at least one source URL and a month+year, and two of the three carry two independent URLs. IETF agentproto BoF (datatracker.ietf.org minutes, Jul 2026; nerdleveltech.com, Jul 2026). MCP specification 2026-07-28 (blog.modelcontextprotocol.io, Jul 2026; aaif.io, Jul 2026). Article 50 final guidelines (faegredrinker.com, Jul 2026; digital-strategy.ec.europa.eu, Jul 2026). Every Emerging Signal, Counter-Signal, Regulatory Shift, Capital Movement and Technical Change bullet also carries URL plus month+year. The gate passes on its stated terms.
- Five of the six Signals Emerging bullets in scenario section 7.1 trace to dated, sourced sweep items: Article 50 (Confirmed Development 3), MCP 2026-07-28 (Confirmed Development 2), agentproto BoF (Confirmed Development 1), UCP 11,414-store conformance snapshot (Counter-Signals), and the Neo / Act Security / Hush Security / Natural / AIsa funding cluster (Capital Movements).
- The sixth bullet (human review falling 40% to 25%, full autonomy rising 11% to 26%, 44% keeping AI-specific incident procedures) does not appear in the sweep at all. It comes from this run's grading file and the ledger grade on coordination-2026-02-04, where it is sourced to prnewswire.com, Jul 2026. It is dated and sourced within this run, so it does not fail the gate, but it is a cross-artifact borrow and the scenario presents it as if it were sweep material.
- Recorded upstream defect, not gate-failing: the sweep's own Contradictions section states the IETF room "agreed that interoperability needs standardizing (155 yes, 30 no)". No 155 figure appears in the sweep's Confirmed Developments, which record three distinct votes (154-51-5 on forming a WG, 158-30 on the IETF as venue, 38-124 rejecting scope). The scenario inherited the ambiguity and made it worse: 7.1 bullet 3 attaches the "agreement that interoperability needs standardising" gloss to the 158-30 venue vote. Both a sourced number and a sourced gloss exist upstream; they have been fused into a pairing that the minutes do not support as written.
- Claims in the scenario with no upstream evidence at all: the occupational role "principal of record" (section 3), the practice of "selective pre-signature" (sections 3, 4, 7.3, 8), and the assertion that a vendor control-plane log is a record affected parties "cannot subpoena" (section 4). The first two are narrative constructions derived from the Forces and Feelings Irreplaceable Thing rather than from evidence; the third is an upstream inference stripped of its marker. These are grounding problems, scored in sections 2 and 3 below, not gate failures, because none of them is offered as a dated factual claim about the present.

Proceeding to scoring.

---

## 1. Structural Compliance

Pass/Fail: PASS

Notes:

- All nine required sections are present, in the prescribed order, with the exact headings from the scenario-generator contract, including both 7.x and 8.x subheadings.
- Length constraints are respected throughout. Section 2 is 152 words (target approximately 150). Section 3 is 374 words (target 300-400). Section 4 is 223 words (target 150-250). Section 5 is 219 words (target 150-250). Section 7.2 is 149 words (target 120-200).
- Bullet counts are in range: 7.1 has six bullets (4-6), 7.3 has six (4-6), Skills We May Need has six (4-6), Signals and Refractions has three (2-3), section 6 has three reflections (2-3).
- Pullback layer is complete: all three subsections present and populated, with 7.3 mixing individual, organisational and societal actions as required.
- Required scenario elements are used. All three Normal Absurdities from Forces and Feelings appear in section 3 (the disclosure nobody reads and where careful reading is a novice tell; the agent that assembles a basket and hands back a manual checkout; the post-mortem about actors who no longer exist, reconstructed by an open-weight model). The requirement is two; three are delivered. The Irreplaceable Thing (an answerable name, one person who accepts an action in advance and stays reachable) is the emotional centre of the closing beat and recurs in sections 4, 7.3, 8 and 9.
- Docked for meta-commentary, which the generator contract prohibits outright. Section 7.2 names an internal pipeline artifact inside a reader-facing narrative: "this pipeline's own calibration (CAL-002) records that it overestimates the firmness of announced regulatory dates". Section 4 carries "Inference, not established by this run's evidence: this practice spreads socially". The calibration constraint asks the generator to slow the clock in the world-building, not to cite the memo to the reader. Section 4's marker is defensible under the run's honesty requirement and I treat it as the lesser fault; the CAL-002 citation is not.
- No em-dash characters. The en-dashes present are in the prescribed section headings.

---

## 2. Cross-Layer Grounding Check

Pass/Fail: PASS (with a material omission)

Grounding Strength: moderate

Notes:

- Four of the six PESTLE categories are visibly load-bearing. Technological (MCP's stateless rewrite, routing headers, removal of the session identifier) drives section 5's first force and the scenario's core conceit. Legal (Article 50 enforceable 2 Aug 2026, per-agent first-contact duty) drives the disclosure absurdity and section 5's second force. Economic capital flows (Neo at $100M for real-time attribution, Act Security, Hush Security, Mastercard Agent Pay for Machines with 30-plus participants) drive section 5's third force. Environmental (shared infrastructure as the real substrate, the 8-13 Jul 2026 four-organisation intrusion through a JFrog Artifactory cache-proxy zero-day, Modal and Hugging Face) drives section 5's fourth force and the section 3 post-mortem. Political (the agentproto BoF deadlock) carries section 2 and 7.1.
- Contradiction 1 from Forces and Feelings is the best-operationalised element in the artifact. "Law is constructing an addressee for accountability at the same rate that organisations are vacating the position" becomes, concretely, a man whose name resolves 412 agents' disclosures and who reviewed almost none of what they did. That is an abstraction converted cleanly into a lived mechanism.
- Contradiction 3 is also well operationalised: the verb travels in headers, the subject does not, and the post-mortem has no host to image.
- Contradiction 2 is only half-operationalised, and this is the artifact's most consequential grounding failure. The economic half of that contradiction is not just "attribution is sold" but that it is selling into pilot budgets against a demand side that does not work: IDC data cited late Jul 2026 puts 88% of agent proofs-of-concept as never reaching broad production, Fiddler AI telemetry shows enterprise agent success falling from roughly 60% on a single run to 25% across eight consecutive runs at production load, and Gartner projects more than 40% of agentic projects cancelled by end-2027. None of that reaches the narrative. The lived world contains 412 agents at a regional pharmaceutical wholesaler and an eleven-supplier reorder run that completes availability checks, substitution pricing and cold-chain windows without incident. The sweep's single strongest counter-signal, that coordination capability is not converting into production systems, has been deleted from the world it should most constrain. The scenario grounds the accountability gap meticulously and grounds the reliability gap not at all.
- Systems introduced without upstream grounding: "principal of record" as a salaried occupational role, and "selective pre-signature" as a spreading professional practice. Neither is a new institution or technical primitive in the sense the generator contract prohibits, and both descend from the Forces and Feelings Irreplaceable Thing, so I do not treat them as violations. But note what the first one does to the argument. Article 50 as recorded in the sweep requires naming "the person or entity" on whose behalf the agent acts, which in an employment setting is satisfied by the employer. The scenario adds a second clause naming a specific employee. That addition is the mechanism the entire scenario turns on, and it is invented, unmarked, and not required by the instrument it is attributed to.
- One upstream inference is presented as fact. PESTLE Legal force 4 explicitly labels as "Inference, not established by this run's evidence" the proposition that attribution becomes a contractual rather than statutory entitlement. Section 4 restates it harder and unmarked: the authoritative record "lives in a vendor's control plane they cannot subpoena". Third-party discovery against vendors is ordinary practice; the sweep contains nothing establishing that such records are unobtainable. The scenario upgraded a hedged inference into a legal impossibility.

---

## 3. Institutional Realism Audit

Assessment: low to moderate realism

Notes:

- Some friction is well drawn. The nine minutes of manual invoice payment, the director calling pre-signature a hobby, the post-mortem that resolves to an infrastructure path rather than an actor, and the pharmacists skipping the notice are all textured and none of them resolves neatly. The scenario is not naive about how organisations behave day to day.
- Power asymmetries are visible: vendors hold the authoritative record, the wholesaler holds the liability, the individual holds the name. That is a real asymmetry and the scenario states it.
- Against that, the world is presented as fully stabilised, and the stabilisation is doing unearned work. Four years after Article 50 becomes enforceable, disclosures go out "correctly, in six languages", universally, at first contact. Section 7.3 simultaneously asks that someone "enforce one Article 50 case visibly against a named deployer, because a disclosure duty nobody has seen applied trains the whole market to treat it as decorative". The scenario therefore depicts near-universal, technically correct, multilingual compliance with a duty it says in the same document has never been enforced against anyone. Those two states are not compatible without an explanation the artifact does not give.
- Enforcement is absent as a system. The AI Office took general-purpose enforcement powers on 2 Aug 2026 per the sweep. Four narrative years later there is no fine, no inquiry, no supervisory correspondence, no compliance vendor selling Article 50 conformance, nothing. A regulatory regime is depicted purely as a behavioural norm.
- The most implausible silence is around the protagonist himself. A named individual is the disclosed principal for 412 agents whose actions he does not review, in a regulated pharmaceutical supply chain, in a world where a cross-company cascade already happened. In that situation the mechanisms that would move first are exactly the ones CAL-003 says this pipeline underweights: professional indemnity carriers pricing or excluding the exposure, employment contracts allocating it, works councils or professional bodies objecting to individual employees carrying it, sector procurement clauses requiring it. The sweep already shows insurers and card networks building agent liability products. None of that machinery exists in this world. The role is invented and then left uncontested by every institution that would in practice contest it, which is what makes it feel like a device rather than a job.
- Transitions are implied only in the pullback layer. Sections 3 to 5 present arrival without passage: no migration pain from the mid-2027 MCP deprecation cliff, no failed control-plane procurements, no vendor consolidation or failure among the five funded startups the scenario relies on, despite Gartner's cancellation projection sitting in the sweep.
- The world is too elegant. Every institution in it behaves exactly as the thesis requires and no institution behaves inconveniently.

---

## 4. Horizon Discipline Check

Pass/Fail: PASS (with a recorded calibration relapse)

Notes:

- Horizon is held nominally. Section 2 dates the world at "four years on" from mid-2026, so roughly 2030, inside the 0-5 year bound. No sci-fi drift: nothing in the world requires a capability that does not exist in Aug 2026. The technologies named are MCP headers, gateways, control planes, payment credentialing and short-lived sandboxes, all present today.
- Probable Direction (7.2) is the strongest section in the artifact epistemically. It forecasts divergence rather than resolution, explicitly declines to treat the Article 50 date as a switch, notes the 2 Dec 2026 extension for pre-existing deployments, predicts a framework document before a deployed principal field, and states that the binding constraint is coverage rather than capability. That is a disciplined, falsifiable, appropriately slow forecast and it maps cleanly onto the four ledger tests logged this run (coordination-2026-08-01 through -08-04).
- Institutional shifts are mostly proportional. Nothing statutory is invented; the changes are behavioural and market-side.
- The calibration relapse is CAL-002, and it is a real one despite the verbal disclaimer. 7.2 tells the reader that this pipeline overestimates the firmness of announced regulatory dates. Section 3 then builds a world in which the announced regulatory date produced universal, correct, routine compliance within four years. The heuristic was cited rather than applied. The narrative layer, which is the layer readers absorb, does exactly what the heuristic warns against; the analytic layer disclaims it. This is the specific failure mode CAL-002 was written to catch, appearing in the artifact that names CAL-002.
- A second horizon problem runs the other way, and it is a static extrapolation rather than an accelerated one. The scenario freezes the 7 Jul 2026 UCP conformance snapshot (11,414 verified stores, 11,389 exposing checkout, zero exposing payment) as a stable structural feature of 2030, with Tomas still paying four invoices by hand. The same sweep bullet records verified store count growing 38% month over month, and the same sweep records Mastercard's Agent Pay for Machines live since 10 Jun 2026 with more than 30 participants including Adyen, Stripe, Cloudflare, Coinbase and Ant International, plus Natural funded at $30M in Jul 2026 for an agent orchestration and payments layer. The scenario's own section 4 says buyers steer transactions onto payment rails because that is where a principal gets named. Holding "the payment rail is the working identity layer" and "shops cannot take agent payment after four years" together is possible in a lagging sector, but the scenario does not argue the lag; it inherits a one-month snapshot and treats it as a permanent condition. This is the loosest inference in the artifact and it carries one of the three Normal Absurdities.

---

## 5. Signal Integrity Check

Pass/Fail: PASS

Signal Anchoring Strength: strong

Notes:

- Every one of the six Signals Emerging bullets is a genuine present-day observable with an upstream date and source in this run's artifacts. None is invented, none is a projection dressed as a signal, and none is a rounded or inflated restatement of the underlying figure. The UCP numbers, the funding amounts, the vote tallies, the oversight percentages and the dates all match their upstream records.
- Extensions from signal to world are incremental in kind. Nothing in the scenario requires an unobserved breakthrough. The world is a straight-line consequence of shipped protocol behaviour, an in-force regulation, an observed intrusion path and a documented funding pattern.
- One anchoring defect, carried in from the sweep: 7.1 bullet 3 pairs the 158-30 venue endorsement with the claim that it expressed "agreement that interoperability needs standardising". The sweep supports the number and separately supports a similar gloss on a different number (155-30). The scenario should not be the place where two upstream figures are merged.
- One bullet (the oversight reversal) is sourced from the grading file rather than the sweep. Sourced and dated, but it means the generator reached outside its declared input for its sixth signal.
- Deducted nothing for the reliability material being missing here, because 7.1 is a signals list rather than a counter-signals list. That omission is scored in section 2, where it belongs.

---

## 6. Narrative Inflation Risk

Assessment: moderate to high

Notes:

- The scenario collapses into a single dominant logic and then never tests it. The thesis is stated in section 9: naming was skipped because naming is the expensive part. Every element in the world is an instance of that thesis. The protocol drops the subject because subjects are expensive. The stores skip payment because identity is expensive. The organisations abandon review because supervision is expensive. The vendors sell attribution because it is expensive. There is no element in this world that the thesis does not explain, which is a warning sign rather than a strength. A world with one working explanation is a thesis with scenery, not a scenario.
- Coherence is exaggerated. No actor in the world is confused, self-interested in an inconvenient direction, or simply bad at their job. The pharmacists respond uniformly, the disclosures are uniformly correct, the incident review reaches its finding calmly, the market moved in one direction. Real coordination failures are noisier than this.
- The register is uniformly elegiac and the prose is aphoristic to a degree that does epistemic work it has not earned. "Reading the notice is a beginner's tell." "It is simply where the machine part ends." "It does not scale. That may be the point." These are good sentences and that is the problem: they confer an air of settledness on extrapolations that are contingent, particularly the four-year commerce freeze and the invented principal-of-record role.
- Not lurid, and that is a genuine mitigation. The scenario avoids catastrophe, avoids villains, explicitly denies that oversight "lost an argument", and keeps the stakes at the scale of a working day. It is not dystopian inflation; it is coherence inflation.
- Emotional over-concentration around scarcity is present and tight. Every thread terminates on the same scarce object, an answerable name, and the closing image, the reflections, the skill seeds and the preferred path all restate it. Six of the six Skills We May Need are variations on one skill.

---

## 7. Cross-Theme Convergence Risk

Assessment: high

Notes:

- Comparison data is available: all five 2026-08-04 scenarios (coordination, responsibility, alignment, authority, trust) were read for this section.
- The scarce object is nearly the same in all five, and in three cases it is literally the same object. Coordination: "an answerable name... one action, one name, reachable when it lands." Responsibility: "a sum offered in place of a sentence, and a blank space where a name should be." Authority: "a binding no... the practical test of a rule is whether its enforcer has a phone number." Trust: an account of an incident that does not depend on the party that caused it. Alignment: "a witness with nothing to lose." Five themes, one scarcity: someone specific who can be reached and held.
- The reachability image is duplicated almost verbatim across two artifacts of the same run. Coordination gives its protagonist "a phone number that reaches him"; authority tests rules by "whether its enforcer has a phone number". That is tonal homogeneity at the level of the sentence, not just the theme.
- The Final Insight sections share a structural formula: a concessive opening that nobody acted in bad faith or carelessly, a pivot to what is structurally scarce, and a closing human-scale image. Coordination, alignment, authority and responsibility all run this pattern. Trust runs a close variant.
- Source overlap compounds it. The 8-13 Jul 2026 intrusion and the GLM-5.2 open-weight reconstruction appear as load-bearing material in coordination, trust and alignment. Coordination's third Normal Absurdity (an incident reconstructed by an unguarded model because the guarded ones refuse) is the trust scenario's central subject, used here as a secondary beat.
- The 2 Aug 2026 AI Office enforcement date anchors coordination, authority, responsibility and trust. Concurrent themes drawing on one month's evidence will overlap legitimately, but four of five scenarios organising themselves around the same fortnight of EU instruments is a corpus-level risk to the Outlook, not just a per-artifact one.
- Coordination's distinctive contribution, which is real, is the layer argument: that the attributable surface and the propagating surface are different surfaces, and that events travel through package registries and cache proxies rather than through the protocols governance watches. That argument is this theme's own and appears nowhere else in the run.

---

## 8. Overall Evaluation

Score (1-10): 6.2

Forecast Integrity Level: moderate

Stability Risk: medium

Summary:

This artifact is strong exactly where the pipeline is usually weak and weak exactly where its prose is most persuasive. Signal anchoring is the best in the run's coordination chain: six present-day signals, all dated, all sourced, all faithfully stated, with no invented capability and no unobserved breakthrough required to reach the world described. The Probable Direction section is disciplined, forecasts divergence rather than resolution, slows its own regulatory clock, and maps onto four falsifiable ledger tests resolving 2027-02 and 2027-03. The structural question it dramatises, that routing metadata standardised in the same fortnight accountability metadata became a legal duty, is genuinely this theme's own and is not duplicated elsewhere in the run.

Three defects hold the score down. First, the artifact deletes the sweep's strongest counter-signal: the world runs 412 agents reliably at a regional wholesaler while the evidence says 88% of proofs-of-concept never reach production, multi-run success falls to 25% at load, and Gartner expects over 40% of projects cancelled. A coordination scenario that assumes coordination works is not grounded in this month's coordination evidence. Second, the mechanism the whole narrative turns on, a salaried individual "principal of record" whose personal name appears in every disclosure, is invented, unmarked, not required by Article 50 as the sweep records it, and left uncontested by every insurer, contract and professional body that would in practice contest it. Third, CAL-002 is cited rather than applied: the analytic layer disclaims regulatory firmness while the narrative layer depicts universal correct compliance with a duty the same document says has never been enforced.

Subscores:
- Structural Compliance (1-10): 8
- Cross-Layer Grounding (1-10): 6
- Institutional Realism (1-10): 5
- Horizon Discipline (1-10): 6
- Signal Integrity (1-10): 8
- Narrative Inflation Control (1-10): 5
- Distinctiveness vs. Other Themes (1-10): 3

Weighted calculation:
- Structural Compliance 8 x 0.10 = 0.80
- Cross-Layer Grounding 6 x 0.20 = 1.20
- Institutional Realism 5 x 0.20 = 1.00
- Horizon Discipline 6 x 0.15 = 0.90
- Signal Integrity 8 x 0.20 = 1.60
- Narrative Inflation Control 5 x 0.10 = 0.50
- Distinctiveness vs. Other Themes 3 x 0.05 = 0.15
- Total = 6.15, reported as 6.2

Weakest dimension: Distinctiveness vs. Other Themes (3). Among the dimensions carrying material weight, Institutional Realism and Narrative Inflation Control (both 5) are the binding constraints on the score.
