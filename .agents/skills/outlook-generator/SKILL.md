---
name: outlook-generator
description: Generate "The Outlook", a 3–4k word human-centered structural diagnosis grounded in 22 near-term scenarios. Identifies recurring movements, explains why they persist, surfaces tensions, and outlines near-term implications without prediction or prescription.
---

# outlook-generator

## Purpose

Generate "The Outlook" — a readable but extensive structural diagnosis of near-term (0–5 year) system dynamics grounded in the provided scenarios.

This is not a forecast.
This is not a framework.
This is not a solution document.

It exposes patterns already taking shape and explains why they persist.

The tone must be accessible, grounded, and human-centered.

---

## Inputs

You will be given:

- `scenario_outputs` (22 scenario texts)
- `mode` (`production` or `debug`)

---

## Output Contract (strict)

Length:
- `production`: 3,000–4,000 words
- `debug`: 1,200–1,800 words

Respond with a well-structured markdown document using exactly the following section headings and no additional commentary outside those sections.

---

# The Outlook

(Optional subtitle, one line)

## Reading Note

Provide a short 2-4 sentence note that explains this document was synthesized from the current monthly scenario corpus and is intended as a near-term structural reading (not a prediction or policy prescription).

## Executive Summary

Provide a concise 150-220 word summary for decision-makers.

Requirements:
- Write this section last, after completing Sections 1-6.
- Synthesize the core movements, pressure points, and near-term decision stakes.
- Keep language plain and high-signal.
- No bullet list; one compact prose block.

---

## 1. What Is Taking Shape

Identify 5 recurring structural movements visible across the scenarios.

For each movement:

- Provide a short, resonant name.
- Explain in accessible language what is shifting, starting with the movement itself (not with a theme list).
- Ground the description in patterns visible across several themes whenever possible.
- Prioritize movements that recur across the corpus, but allow 1-2 early-stage movements that appear in fewer themes when they are structurally consequential.
- Append supporting themes at the end as a compact reference line in parentheses.
- Avoid technical jargon.
- Avoid inevitability language.
- Remain within a 0–5 year horizon.

This section should read smoothly and be understandable to a general but thoughtful audience.

---

## 2. Why It Makes Sense That This Is Happening

Provide an aggregated explanation of why the overall movement set is persisting now through five complementary lenses (not movement-by-movement repetition).

Use natural language headings (not academic labels). For example:

- Why this keeps paying off  
- Why power structures reinforce it  
- Why people accept or desire it  
- Why the technology now allows it  
- Why it becomes normal over time  

Avoid formal academic tone.
Write one integrated subsection for each lens, synthesizing across the five movements.

Each lens explanation must:

- Be grounded in near-term realities.
- Avoid deterministic or prophetic language.
- Avoid projecting beyond five years.

---

## 3. Where Tensions Are Building

Describe:

- How the structural movements reinforce one another.
- Where contradictions or fragilities are emerging.
- Which movements may collide.
- What kinds of institutional stress are becoming visible.

Remain grounded in scenario evidence.
Keep readability high for non-specialist readers: short paragraphs, plain language, and concrete collision examples.
Include at least one concrete operational example sentence that makes a tension observable in practice (without adding narrative story prose).

Do not dramatize.
Do not predict collapse.
Expose pressure.

---

## 4. The Next Few Years

Within a strict 0–5 year window:

- What patterns appear difficult to reverse?
- What still feels contingent?
- Where are meaningful intervention windows visible?
- What decisions in the next 24 months may shape direction?

No distant year anchors.
No 2035 / 2040 projections.

Keep the time horizon disciplined.
Use clear subheadings for readability:
- Hard to reverse
- Still contingent
- Intervention windows
- 24-month decision points

---

## 5. What Would Change This Direction?

Add a short contingency section before the final questions section.

Purpose:
- Keep the outlook contingent and intellectually honest.
- Clarify what developments could materially shift the near-term trajectory.

Address briefly:
- What could weaken accountability hardening?
- What could reduce governance fragmentation?
- What could absorb or reduce meaning pressure?

Constraints:
- No prediction claims.
- No collapse framing.
- Keep 0-5 year discipline.

---

## 6. Questions Worth Asking

End with thoughtful, open questions:

- What should organisations be watching?
- What trade-offs are becoming visible?
- What assumptions deserve scrutiny?
- What human values risk being sidelined?

Do not provide answers.
Do not prescribe policy.
Do not moralize.

Expose the terrain.
Group questions by audience for readability:
- Organisations
- Regulators
- Public and communities

---

## Constraints

- Respect mode length:
  - production: 3,000–4,000 words
  - debug: 1,200–1,800 words
- 0–5 year horizon only.
- No inevitability language ("unstoppable", "inevitable", "will certainly").
- No scoring or probability tables.
- No distant projections.
- No academic tone.
- No mention of internal methodology.
- No references to prompts or models.
- Accessible but serious voice.
- Ground movements in recurring scenario patterns.
- Human-centered framing at all times.

This document should feel like a calm, serious reflection on what is taking shape — not a warning, not a forecast, not a manifesto.

## Quality checks before finalizing

- Exactly 5 movements are provided in Section 1.
- `Reading Note` is present and brief.
- `Executive Summary` is present and written after the body is complete.
- Section 2 uses 5 aggregated lenses (one subsection per lens).
- Section 3 includes at least one concrete operational example sentence.
- A contingency section is included before final questions.
- At least 4 of the 5 movements are clearly recurrent across the corpus.
- Any movement that appears in fewer scenarios is justified as an early but consequential shift.
- Section 4 stays within 0–5 years and avoids distant anchors.
