---
name: scenario-eval
description: Conduct a structured epistemic audit of a generated Pathfinder Scenario. Validates structural compliance, cross-layer grounding, plausibility discipline, and narrative inflation risk. Produces a logged evaluation without modifying the scenario.
---

# scenario-eval

## Purpose

Conduct a disciplined evaluation of a completed scenario artifact to determine:

- Structural compliance
- Cross-layer coherence
- Institutional realism
- Evidence anchoring strength
- Horizon discipline (0–5 years)
- Narrative inflation risk
- Cross-theme convergence risk

This skill does NOT rewrite, optimize, or improve the scenario.
It evaluates and logs findings only.

This is an epistemic audit, not a literary critique.

---

## Inputs

You will be given:

- `theme` (string)
- `scenario_output` (from Step 04)
- `exploration_output` (from Step 01)
- `pestle_output` (from Step 02)
- `forces_feelings_output` (from Step 03)

---

## Output Contract (strict)

Return exactly the following sections:

---

## 1. Structural Compliance

Pass/Fail:
Notes:

- All required sections present?
- Correct section order?
- Section length constraints respected?
- Pullback Layer complete?
- Required scenario elements (Normal Absurdities + Irreplaceable Thing) clearly used?

---

## 2. Cross-Layer Grounding Check

Pass/Fail:
Grounding Strength: (strong / moderate / weak)

Notes:

- Are all major institutional systems traceable to PESTLE?
- Are contradictions visibly operationalized in the narrative?
- Does the scenario introduce new systems not grounded upstream?
- Are abstractions converted into lived mechanisms?

---

## 3. Institutional Realism Audit

Assessment: (high / moderate / low realism)

Notes:

- Are governance, enforcement, or economic mechanisms described with sufficient friction?
- Are transitions implied, or is the system presented as fully stabilized?
- Are power asymmetries visible?
- Does the world feel too elegant or overly coherent?

---

## 4. Horizon Discipline Check

Pass/Fail:
Notes:

- 0–5 year horizon maintained?
- No sci-fi drift?
- Probable Direction plausible given current trajectories?
- Are institutional shifts proportional to timeline?

---

## 5. Signal Integrity Check

Pass/Fail:
Signal Anchoring Strength: (strong / moderate / weak)

Notes:

- Are Signals Emerging plausibly present today?
- Are extensions incremental or speculative leaps?
- Does scenario rely on unobserved breakthroughs?

---

## 6. Narrative Inflation Risk

Assessment:
(low / moderate / high)

Notes:

- Does the scenario exaggerate coherence?
- Does it collapse complexity into a single dominant logic?
- Does it lean excessively dystopian or utopian?
- Is there emotional over-concentration around scarcity?

---

## 7. Cross-Theme Convergence Risk

Assessment:
(low / moderate / high)

Notes:

- Does this theme replicate structural patterns seen in other themes?
- Is the emotional scarcity similar to other scenarios?
- Is there tonal homogeneity emerging?

(If no comparison data available, state: "Not evaluated – no cross-theme context provided.")

---

## 8. Overall Evaluation

Score (1–10):

Forecast Integrity Level:
(high / moderate / fragile)

Stability Risk:
(low / medium / high)

Summary:
(200–300 word analytical synthesis focused on epistemic strength, not literary quality.)

Subscores:
- Structural Compliance (1-10):
- Cross-Layer Grounding (1-10):
- Institutional Realism (1-10):
- Horizon Discipline (1-10):
- Signal Integrity (1-10):
- Narrative Inflation Control (1-10):
- Distinctiveness vs. Other Themes (1-10):

Scoring Method:
- Weighted total must be used for `Score (1–10)`:
  - Structural Compliance: 10%
  - Cross-Layer Grounding: 20%
  - Institutional Realism: 20%
  - Horizon Discipline: 15%
  - Signal Integrity: 20%
  - Narrative Inflation Control: 10%
  - Distinctiveness vs. Other Themes: 5%
- Report final weighted score to one decimal place.

---

## Constraints

- Do NOT rewrite.
- Do NOT propose edits.
- Do NOT suggest improvements.
- Do NOT generate alternative futures.
- Evaluate only.
- Be analytical, skeptical, and disciplined.
- Penalize unsupported institutional leaps.
- Penalize excessive elegance.
- Avoid score collapse to a single repeated value across themes unless evidence strongly supports it.
- Use the full score range when justified by artifact quality differences.
