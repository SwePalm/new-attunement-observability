---
name: forces-feelings
description: Synthesize exploration + PESTLE into the structural and emotional DNA of one future world - contradictions, normal absurdities, and the single irreplaceable thing. Deep-dive step for selected themes.
---

# forces-feelings

## Purpose
Create the "engine" for scenario-writing by defining:
- Systemic contradictions
- Normalization of the absurd
- The single, irreplaceable thing

## Inputs
You will be given:
- `theme` (string)
- `exploration_output` (text)
- `pestle_output` (text)
- `sweep_output` (text from evidence-sweep)
- `recent_irreplaceable_things` (the Irreplaceable Thing from every 06-forces-feelings file in the previous two runs, plus any sibling theme already written this run)

## Output contract (strict)
Return exactly these sections:

## A. Systemic Contradictions (The Engine of the Story)
Contradiction 1 (Political vs. Social):
Contradiction 2 (Economic vs. Legal):
Contradiction 3 (Philosophical vs. Lived Reality):

## B. The Normalization of the Absurd (The Tone)
Normal Absurdity 1:
Normal Absurdity 2:
Normal Absurdity 3:

## C. The Single, Irreplaceable Thing
The Irreplaceable Thing:
Explanation:
(100–150 words)

## Constraints
- Contradictions must be genuine tensions (not two synonyms).
- At least two contradictions must explicitly reference PESTLE category interactions.
- At least 1 systemic contradiction must be directly grounded in sweep_output contradictions or regulatory/capital/technical tensions.
- Normal Absurdities must be plausible daily-life norms (not tech specs).
- At least 1 Normal Absurdity must be a plausible lived-expression of a sweep_output item.
- Irreplaceable Thing must be emotional, social, physical, material or
 institutional, and scarce in-world.
- The Irreplaceable Thing must be made scarce by a specific mechanism named in
 sweep_output or pestle_output; the Explanation cites that item.
- It must differ in kind from every item in `recent_irreplaceable_things`.
 In particular, do not default to a variant of "a real person being present"
 (company, being known, being checked or noticed by someone who is there):
 six of six scenarios in the 2026-09-25 run resolved to it. If this theme's
 evidence genuinely compels a repeat, say so in the Explanation and name the
 evidence.
- No scenario prose here. This is scaffolding, not story.

## Quality checks before finalizing
- Contradictions are "generative": you can imagine conflict arising from them.
- Normal Absurdities feel mundane *inside* the world, shocking *outside* it.
- Irreplaceable Thing is something a protagonist could actively pursue.
