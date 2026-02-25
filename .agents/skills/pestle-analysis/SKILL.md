---
name: pestle-analysis
description: Convert a theme exploration into a structured PESTLE analysis with concrete near-future forces and a thesis per category. Use when generating Step 02 PESTLE artifacts.
---

# pestle

## Purpose
Translate exploration insights into **concrete**, organized external forces for a near-future (0–5 years) world.

## Inputs
You will be given:
- `theme` (string)
- `exploration_output` (text from the exploration skill)
- `evidence_layer` (text)

## Output contract (strict)
Return exactly the six categories below, each with:
- `Core Shift Thesis:` (1–2 sentences)
- `Forces:` (3–4 numbered forces; 4th is optional)

### Political
Core Shift Thesis:
Forces:
1.
2.
3.
4.

### Economic
Core Shift Thesis:
Forces:
1.
2.
3.
4.

### Social
Core Shift Thesis:
Forces:
1.
2.
3.
4.

### Technological
Core Shift Thesis:
Forces:
1.
2.
3.
4.

### Legal
Core Shift Thesis:
Forces:
1.
2.
3.
4.

### Environmental
Core Shift Thesis:
Forces:
1.
2.
3.
4.

## Constraints
- Forces must be concrete and “actionable” (institutions, policies, market mechanisms, standards, enforcement patterns, org practices).
- Avoid vague items like “more AI” or “more data.” Be specific.
- Keep within plausible adoption curves for 0–5 years.
- No narrative paragraphs outside the thesis line.
- At least one force in each PESTLE category must be grounded in the evidence_layer (confirmed developments, regulatory shifts, capital movements, technical changes, contradictions, or horizon items).

## Quality checks before finalizing
- Every force clearly links back to exploration content.
- At least one force per category is institutional (policy, procurement, treaty, standard, enforcement, governance mechanism).
