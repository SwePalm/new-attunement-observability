---
name: scenario-generator
description: Generate a Pathfinder Scenario narrative from exploration, PESTLE, and forces-feelings, including a Futures Cone pullback layer and present-day connections. Use when generating Step 04 scenario artifacts.
---

# scenario

## Purpose
Transform the upstream artifacts into a **reader-friendly**, emotionally resonant near-future scenario (0–5 years), grounded in everyday life and structured for publishing.

## Inputs
You will be given:
- `theme` (string)
- `exploration_output` (text)
- `pestle_output` (text)
- `forces_feelings_output` (text)
- `evidence_layer` (text)

## Output contract (strict)
Return exactly these numbered sections, in order:

## 1. Title & Core Question
- Title:
- Core Question:

## 2. Context Summary (Translation Layer) – Why This Future Exists
(≈ 150 words)

## 3. Future World Snapshot (The Lived Experience) – A Day in This Future
(300–400 words)
Requirements:
- Integrate at least **two** Normal Absurdities from Forces & Feelings.
- Center the protagonist’s struggle around the Irreplaceable Thing.

## 4. Behavioral Shifts (Human Lens) – How People Adapt
(150–250 words)

## 5. Structural Forces (System Lens) – What Holds This World Together
(150–250 words)

## 6. Reflection & Implications – Questions This World Asks Us
2–3 short reflections or open questions.

## 7. Pullback Layer: From Possibility to Probability
### 7.1 Signals Emerging (Plausible Zone) – Early Signals We Already See
- 4–6 bullets

### 7.2 Probable Direction (Near-Term Future) – Where We’re Likely Headed
(120–200 words)

### 7.3 Preferred Path (Intentional Future) – The Path We Could Choose Instead
(4–6 bullets, mix of individual/org/society actions)

## 8. Connect to Today
### Skills We May Need
- 4–6 “skill seeds” (short provocations)

### Signals & Refractions
- 2–3 examples

## 9. Final Insight
(Short closing paragraph; no instructions)

## Constraints
- Keep the time horizon 0–5 years.
- No far-future AGI omniscience.
- Narrative should be reflective, grounded, and non-technical.
- Must reflect PESTLE forces and Forces & Feelings tensions.
- Section 7.1 Signals Emerging must reuse at least 3 signals from evidence_layer (confirmed/emerging/regulatory/capital/technical), rephrased for readability.
- Section 5 Structural Forces must reflect at least 2 evidence_layer items (for example regulatory shift + technical change).
- No new major institutions or technical primitives unless implied by evidence_layer.
- No meta-commentary.

## Quality checks before finalizing
- Section 3 includes 2+ Normal Absurdities and the Irreplaceable Thing as the emotional center.
- Signals Emerging bullets are plausible present-day indicators (not inventions detached from reality).
- Output matches headings exactly.
