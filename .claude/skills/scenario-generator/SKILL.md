---
name: scenario-generator
description: Generate a Pathfinder Scenario narrative from exploration, PESTLE, and forces-feelings, including a Futures Cone pullback layer and present-day connections. Deep-dive step for selected themes.
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
- `sweep_output` (text from evidence-sweep)
- `calibration` (active heuristics from ledger/CALIBRATION.md)

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
- Center the protagonist's struggle around the Irreplaceable Thing.
- Declare the vantage on one line before the prose, in the form
 `Vantage: <role class> / <setting class>`. Role classes are: person
 subject to the system, frontline operator, mid-senior professional
 inside the institution, outsider or volunteer with no contract,
 collective with no single protagonist.
- The mid-senior professional vantage is permitted only where the
 Irreplaceable Thing is unreachable from any other vantage, and the
 scenario must carry one clause saying why.
- Do not open on a named professional plus job title plus organisation
 headcount. No staff count in the first sentence.
- Do not fix the scene to a named weekday. Keep the in-world year implicit
 unless a dated instrument in sweep_output makes it load-bearing.
- A structural form (a day, a case file, a sequence of readings, letters) may
 be assigned by the orchestrator; if so, follow it and name it on the
 Vantage line.

## 4. Behavioral Shifts (Human Lens) – How People Adapt
(150–250 words)

## 5. Structural Forces (System Lens) – What Holds This World Together
(150–250 words)

## 6. Reflection & Implications – Questions This World Asks Us
2–3 short reflections or open questions.

## 7. Pullback Layer: From Possibility to Probability
### 7.1 Signals Emerging (Plausible Zone) – Early Signals We Already See
- 4–6 bullets

### 7.2 Probable Direction (Near-Term Future) – Where We're Likely Headed
(120–200 words)

### 7.3 Preferred Path (Intentional Future) – The Path We Could Choose Instead
(4–6 bullets, mix of individual/org/society actions)

## 8. Connect to Today
### Skills We May Need
- 4–6 "skill seeds" (short provocations)

### Signals & Refractions
- 2–3 examples

## 9. Final Insight
(Short closing paragraph; no instructions)
Do not close on the run's default move (reasonable actors, structural outcome,
the Irreplaceable Thing named in the last clause). The Irreplaceable Thing has
already carried Section 3; if it appears here it must appear as a cost already
paid or a choice already refused, not as a reveal.

## Constraints
- Keep the time horizon 0–5 years.
- No far-future AGI omniscience.
- Narrative should be reflective, grounded, and non-technical.
- Must reflect PESTLE forces and Forces & Feelings tensions.
- Section 7.1 Signals Emerging must reuse at least 3 signals from sweep_output (confirmed/emerging/regulatory/capital/technical), rephrased for readability.
- Section 5 Structural Forces must reflect at least 2 sweep_output items (for example regulatory shift + technical change).
- No new major institutions or technical primitives unless implied by sweep_output.
- A regulatory commencement date shared across the corpus (for example an EU
 applicability date) may appear in Section 5 only where the theme's own
 sweep_output carries it as a Confirmed Development or Regulatory Shift, and
 it may not be the first structural force listed.
- Apply active calibration heuristics as restraint: if the pipeline is known to overestimate a class of change (e.g. regulatory speed), slow that clock in the world-building rather than repeating the bias.
- No meta-commentary: reader-facing sections never name a calibration
 heuristic (CAL-NNN) or the pipeline itself.

## Quality checks before finalizing
- Section 3 includes 2+ Normal Absurdities and the Irreplaceable Thing as the emotional center.
- Signals Emerging bullets are plausible present-day indicators (not inventions detached from reality).
- Output matches headings exactly.
