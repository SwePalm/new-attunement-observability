## 0. Citation Gate

Pass/Fail: Pass, with two recorded defects

Notes:
- Both Confirmed Developments in `02-sweep/power.md` carry at least one source URL and a month+year. The Texas item carries gov.texas.gov (Aug 2026) and datacenterdynamics (Aug 2026); the PJM item carries insidelines.pjm.com (Aug 2026) and datacenterdynamics (Aug 2026). The Emerging Signals, Regulatory Shifts, Capital Movements and Technical Changes entries are likewise URL-and-date bearing. The gate's primary condition is satisfied.
- Defect 1, traceability of one Signals Emerging bullet. Bullet 3 of Section 7.1 cites the six FERC Section 206 dockets EL26-67 to EL26-72, an 18 Jun 2026 opening date and a 17 Aug 2026 response deadline. None of that detail appears in this run's sweep. It traces instead to `01-grading/power.md` (the power-2026-08-01 grade line) and to the ledger entry power-2026-08-01, which carries a dated CAISO primary document (Jun 2026). So the claim is sourced and dated upstream, but not by the artifact the gate names. This is not a fail (the claim does not cite zero upstream evidence) and it is arguably the correct behaviour given the instruction to carry graded evidence forward, but it is recorded because a reader checking the scenario against the sweep alone will not find it.
- Defect 2, an unsourced item propagated into the scenario. The Pacific, Missouri withdrawal of 12 Aug 2026 appears in the sweep's Delta section without its own URL; the adjacent Counter-Signals entry sources only Allentown and Hillsboro. The scenario reuses Pacific, Missouri in Section 7.1 and again in Section 8. The sweep should not have carried an undated, unsourced third instance in a list whose other two members are sourced, and the scenario inherited it.
- No claim in the scenario cites no upstream evidence at all. Section 3 is explicitly fictional and is not held to the gate; its invented quantities (2,400 MW, the forty-minute tank, the nineteen-month rate case) are narrative instantiations rather than asserted facts.

## 1. Structural Compliance

Pass/Fail: Pass

Notes:
- All nine required sections present, correctly numbered, in the contract order, with 7.1, 7.2 and 7.3 subsections and the two Section 8 subheadings intact.
- Length discipline is good but not exact. Section 2 runs roughly 165 words against a stated target of about 150, because the horizon justification was folded into it (the contract provides no dedicated slot for that, so the overrun is a deliberate trade). Section 3 lands near the top of its 300-400 range. Sections 4, 5, 7.2 all sit inside their bands. Section 9 runs roughly 200 words against "short closing paragraph", which is the clearest overrun in the file.
- Section 7.1 has 6 bullets (contract allows 4-6). Section 7.3 has 6 (allows 4-6). Section 8 has 6 skill seeds (allows 4-6) and 3 refractions (allows 2-3). All at the ceiling, none over.
- Required scenario elements are present and load-bearing rather than decorative. Two Normal Absurdities are integrated into Section 3 itself: the reliability credit paid to the campus appearing as a line item on the protagonist's own bill (Normal Absurdity 1), and the reliability working group seating the campus three times and the water district not at all (Normal Absurdity 3). Normal Absurdity 2, substations known by name and feeders checked before signing a lease, appears in Section 4 rather than Section 3, which satisfies the "at least two" requirement in Section 3 without wasting the third.
- The Irreplaceable Thing (ride-through for everything that is not a data center) is the explicit emotional center of Section 3 and closes it: "What she wants is not a generator."

## 2. Cross-Layer Grounding Check

Pass/Fail: Pass

Grounding Strength: strong

Notes:
- Institutional systems in the narrative trace to PESTLE. The tariffed transfer and the reliability credit trace to Economic force 3 (Section 206 compensation for large-load flexibility). The approval-gate regime in Section 5 traces to Political forces 1 and 2. The queue-vintage effect ("a fleet governed by the year of its queue position", and Ruth's 2031 energisation date) traces to Legal force 4. The standing telemetry proposal in 7.3 traces to Technological force 4. The small-institutions-behaving-like-small-utilities shift in Section 4 traces to Social force 4 and to the Irreplaceable Thing.
- The contradictions are operationalised rather than restated. Contradiction 2 (the same disconnection as violation and as service) is not explained in the narrative; it is enacted, in the sentence where the transfer "is not a violation, it is a product. It settles at a tariffed rate." Contradiction 1 (leverage concentrated in the hands that can make it irrelevant) is enacted through the working-group seat count and the SpaceX exit posture in Section 5. Contradiction 3 (commons versus designed optionality) carries Section 9.
- One genuine weakness. The Environmental PESTLE category barely reaches the narrative. Water appears in Section 3 only as a load (a treatment plant with pumps), not as the resource constraint the PESTLE Environmental thesis makes central, and the Generic Environmental Impact Statement as the effective venue for an electricity decision, which is the sharpest item in that category, appears only as a clause in Section 5 and a bullet in 7.3. The narrative is a five-category story with a sixth category attached.
- No new institutions or technical primitives are introduced. Every body named (FERC, NERC, PJM, PUCT, ERCOT, a state DEC, a rate case, an interconnection queue) exists upstream. The reliability credit is an extrapolation of an existing compensation track, not a new instrument.

## 3. Institutional Realism Audit

Assessment: high realism, with one clean-edge

Notes:
- Friction is rendered at the right granularity and in the right units. The generator fails on its second attempt. The transfer switch is twenty-two years old. The rate case has run nineteen months. The queue position energises five years after it was taken. The substation rebuild reached the protagonist's feeder as a side effect of somebody else's project. These are the actual textures of utility work rather than gestures at difficulty.
- Power asymmetries are visible and are stated as structure rather than as villainy: three seats versus no seat, a filing versus no filing, a tariffed product versus a column of water.
- Transitions are implied rather than asserted. Section 5 says the standards track "arrived, late and narrow" and specifies what it does not cover, which is the correct shape.
- The clean edge, and it is the file's main realism cost: by March 2028 the scenario has a working NERC-derived ride-through standard, a functioning compensation tariff, and an orderly instrumented transfer filed within the hour. That is three institutional products all landing roughly on schedule and interoperating. The real-world version is likelier to be one of them working, one contested on rehearing, and one applying to a subset of interconnections nobody agrees on. Section 7.2 concedes exactly this, but Sections 3 and 5 do not live inside the concession.
- Counterweight: the world is not presented as stabilised. Local refusal is still running, the moratorium still has no expiry, and the largest participants are still exiting, so the elegance is confined to the federal layer.

## 4. Horizon Discipline Check

Pass/Fail: Pass

Notes:
- Horizon is March 2028, roughly 19 months from the run date, comfortably inside 0-5 years, and it is justified arithmetically in Section 2 rather than chosen for atmosphere: a standard filed end-2026 is approved through 2027 and phases in across 2028; rate cases against 2026-2027 spend reach bills in the same period; 2026 queue positions energise in the 2030s. This is a materially better-reasoned horizon than the 2029 default the 2026-08-04 cohort used.
- No sci-fi drift. Nothing in the scenario requires a capability that does not exist in 2026. The technology is relays, transfer switches, elevated tanks and diesel.
- Calibration bias check, and this is where the file loses points. The scenario partially repeats CAL-002 (the pipeline overestimates the firmness of announced regulatory timelines). Section 3 opens on a world where "the standard took effect", and Section 5 states the standards track arrived. That treats the 31 Dec 2026 NERC filing date and the expected 2027 standards as having held well enough to produce compliance behaviour by early 2028. Section 7.2 explicitly hedges this ("later and covering less than the 31 Dec 2026 filing date suggests"), which is the right restraint, but the hedge lives in the pullback layer while the narrative layer proceeds as if the dates held. CAL-002's own 2026-08-13 re-confirmation notes that after an on-time commencement the live failure mode is enforcement latency rather than deadline slippage, which the scenario does not model at all: its 2028 standard is not merely in force, it is being complied with by default.
- The scenario does correctly engage CAL-006 and CAL-007 rather than repeating them. Section 7.2's closing sentence names, without labelling it, the finding that this theme's claims are weighted toward federal and transnational dockets while the observable motion came from a grid operator's incident report and two governors' offices. That is the graded evidence carried forward into the forecast rather than dropped.

## 5. Signal Integrity Check

Pass/Fail: Pass

Signal Anchoring Strength: strong

Notes:
- Five of the six Signals Emerging bullets trace directly to dated, sourced sweep items: the PJM event and disclosure, the FERC-to-NERC direction and expected 2027 ride-through requirements, the Texas named-company commitments and New York Executive Order 62, the SpaceX TeraFab grid-exit statement, and the BloombergNEF pipeline assessment paired with the three local refusals. The sixth (the Section 206 dockets) is sourced upstream but from the grading file and ledger rather than the sweep, as recorded at the gate.
- Extensions are incremental rather than speculative. The two named leaps are (a) that large-load transfer becomes an instrumented, filed, compensated event rather than an unannounced one, which is a straight-line extension of two tracks already running, and (b) that the compensation surfaces on residential bills as a labelled credit, which is an inference about rate design and is presented inside the absurdity frame rather than as prediction. Neither requires an unobserved breakthrough.
- The scenario does not rely on any capability that is not already deployed. This is the file's strongest dimension: an all-hardware world is hard to inflate.
- Minor: the "2,400 MW in one wave rather than two" figure is invented and unmarked. It is fine as fiction, but a reader could mistake it for a projected quantity.

## 6. Narrative Inflation Risk

Assessment: moderate

Notes:
- The scenario collapses toward one dominant logic, exit asymmetry, and reads nearly every institution through it. That logic is well evidenced (SpaceX TeraFab, the 3,800 MW self-disconnection, Abbott's approval gate) but it is one reading, and the file does not seriously entertain the alternative in which ride-through standards plus compensation actually make large loads better grid participants than the industrial customers they replaced. Section 6's first reflection gestures at this and does not develop it.
- There is a mild dystopian lean. Every institutional outcome in the narrative lands against the protagonist, and the one thing that helped her (the substation rebuild reaching her feeder) is immediately converted into a source of anger. That is emotionally true but it is also a thumb on the scale.
- Emotional over-concentration around scarcity is present and is structurally required by the skill (the Irreplaceable Thing must be scarce and pursued). The mitigation here is that ride-through is a real engineering property with a public specification path rather than a metaphor, so the scarcity is falsifiable: if a state writes a critical-small-load ride-through program, the scenario's emotional core dissolves. That is the right kind of scarcity.
- The "everyone acted correctly and the outcome is still a distribution nobody chose" move is doing a great deal of work, appearing in Section 4, Section 6 and Section 9. It is a strong move and it is being leaned on three times.

## 7. Cross-Theme Convergence Risk

Assessment: moderate, materially reduced from the 2026-08-04 cohort

Notes:
- Comparison set: `output/2026-08-04/07-scenario/authority.md` and `coordination.md`, plus the recorded finding that all five scenarios in that cohort shared a house form and scored 3 or 4 on this dimension.
- The named form markers are absent. There is no mid-senior professional at a headcount-specified organisation, no named weekday in 2029, no European entity in a corporate structure, no EU commencement date as the load-bearing force (the 2 Aug 2026 commencement is not mentioned at all, correctly, since it is close to irrelevant to a US grid story), and the close is not on a named scarce good. Section 3 is organised by nested physical durations (92 milliseconds, five cycles, nine seconds, forty minutes, four minutes, nineteen months, six years) rather than by a human working day, and the durations are the section's actual skeleton rather than decoration. The horizon is 2028 and is justified. This is a genuine break in form.
- Residual convergence, and it is real. Two patterns from the previous cohort survive the form change. First, the emotional architecture is unchanged: a single named individual with an operational role, embedded in a system, wanting one thing the system structurally cannot give (Nadia wanted a refusal with standing, Tomas wanted a named reachable action, Ruth wants a written ride-through obligation). The object is physical here rather than procedural, which is an improvement, but the shape is the same. Second, the "reasonable actors, structural outcome" close persists almost verbatim in logic: authority's "Nothing here requires bad faith" is answered by this file's "Nobody is proposing this. There is no bill to oppose." The 2026-08-04 diagnosis identified that move as one of the five shared markers, and it survived.
- Tonal homogeneity across the corpus remains a live risk. The register (measured, structural, quietly angry, ending on a systemic observation) is the same register as the other two files read.

## 8. Overall Evaluation

Score (1–10): 7.7

Forecast Integrity Level: moderate

Stability Risk: medium

Summary:
This is the strongest artifact in the power chain and its strength is unusual in kind: it is grounded in hardware. Every mechanism in the scenario is a relay, a tariff, a permit, a queue position or a tank, all of which existed before the run and none of which requires a capability leap. That makes the file hard to inflate and easy to falsify, which is what forecast integrity is supposed to mean. Signal anchoring is strong, with five of six emerging signals tracing to dated, sourced sweep items, and cross-layer grounding is strong enough that the contradictions are enacted in the narrative rather than narrated at it.

Two things hold the score below 8. First, a horizon-discipline defect that the pipeline is on record for: the narrative layer assumes the announced NERC and FERC chain held closely enough to produce routine compliance by March 2028, while the pullback layer correctly says it probably will not. The hedge and the story disagree, and the story is what a reader remembers. CAL-002's current form, that enforcement latency rather than deadline slippage is the live failure mode after an on-time commencement, is not modelled at all. Second, the file collapses toward a single dominant logic (exit asymmetry) and does not seriously test the reading in which regulated, compensated large loads become better grid citizens than the industrial customers they replaced.

The citation gate passes but records two defects worth carrying: one Signals Emerging bullet is sourced from the grading file and ledger rather than the sweep, and an unsourced local-refusal instance propagated from the sweep's Delta section into the scenario twice.

Stability risk is medium because the world described depends on the NERC and FERC chain roughly holding. If phase one slips materially, the compensated-transfer half of the scenario does not exist as written, though the approval-gate and grid-exit half survives unchanged, which is itself a useful robustness property.

Subscores:
- Structural Compliance (1-10): 8
- Cross-Layer Grounding (1-10): 8
- Institutional Realism (1-10): 8
- Horizon Discipline (1-10): 7
- Signal Integrity (1-10): 8
- Narrative Inflation Control (1-10): 7
- Distinctiveness vs. Other Themes (1-10): 7

Scoring Method:
Weighted total, one decimal place.
- Structural Compliance 8 x 0.10 = 0.80
- Cross-Layer Grounding 8 x 0.20 = 1.60
- Institutional Realism 8 x 0.20 = 1.60
- Horizon Discipline 7 x 0.15 = 1.05
- Signal Integrity 8 x 0.20 = 1.60
- Narrative Inflation Control 7 x 0.10 = 0.70
- Distinctiveness vs. Other Themes 7 x 0.05 = 0.35
- Total: 7.70, reported as 7.7
