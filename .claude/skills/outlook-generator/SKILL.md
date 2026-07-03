---
name: outlook-generator
description: Generate "The Outlook", a 3-4k word human-centered structural diagnosis grounded in this month's graded ledger, 22 evidence sweeps, and 4-6 deep-dive scenarios. Includes the scorecard and month-over-month delta. Manual, after human review.
---

# outlook-generator

## Purpose

Generate "The Outlook" — a readable but extensive structural diagnosis of
near-term (0–5 year) system dynamics, grounded in the month's corpus.

This is not a forecast.
This is not a framework.
This is not a solution document.

It exposes patterns already taking shape, explains why they persist, and —
new in method v2 — reports honestly on how last month's claims fared.

The tone must be accessible, grounded, and human-centered.

---

## Inputs

You will be given:

- `scenario_outputs` (this month's 4–6 deep-dive scenarios)
- `sweeps` (all 22 evidence sweeps)
- `grading_reports` (output/YYYY-MM/01-grading/, with scorecards)
- `selection` (SELECTION.md)
- `previous_outlook` (last month's outlook, if any)
- `mode` (`production` or `debug`)

---

## Output Contract (strict)

Length:
- `production`: 3,000–4,000 words
- `debug`: 1,200–1,800 words

Respond with a well-structured markdown document using exactly the following
section headings and no additional commentary outside those sections.

---

# The Outlook

(Optional subtitle, one line)

## Reading Note

Short 2–4 sentence note: synthesized from this month's graded ledger,
evidence sweeps, and deep-dive scenarios; a near-term structural reading,
not a prediction or policy prescription.

## Executive Summary

Concise 150–220 word summary for decision-makers.
Write this section last. One compact prose block, no bullets.

## The Scorecard

Report how the observatory's own past claims fared this month:

- Totals across themes: confirmed / decayed / falsified / expired / still open.
- 2–4 sentences on the most instructive grades — where reality outran the
  ledger, and where the ledger outran reality.
- Name the single most surprising grade and what it suggests.
- If a calibration heuristic was added or retired, state it in one plain sentence.

Honesty rule: falsified and expired claims must be reported as plainly as
confirmed ones. The scorecard is the credibility of the whole document.

## What Changed Since Last Month

3–6 short paragraphs or bullets drawn from the sweeps' Delta sections and
the grading surprises:

- Which themes moved and why they were selected for deep dives.
- Which prior movements strengthened, stalled, or reversed
  (reference previous_outlook when available).
- What is genuinely new versus continuation.

If there is no previous outlook, state that this is the first outlook under
method v2 and describe the starting baseline instead.

## 1. What Is Taking Shape

Identify 5 recurring structural movements visible across the corpus
(sweeps provide breadth across all 22 themes; scenarios provide depth on
the selected ones).

For each movement:

- Provide a short, resonant name.
- Explain in accessible language what is shifting, starting with the movement itself.
- Ground the description in patterns visible across several themes, citing
  at least one dated development from the sweeps per movement.
- Prioritize movements that recur across the corpus, but allow 1–2 early-stage
  movements when structurally consequential.
- Append supporting themes at the end as a compact reference line in parentheses.
- Avoid technical jargon and inevitability language.
- Remain within a 0–5 year horizon.

## 2. Why It Makes Sense That This Is Happening

Aggregated explanation through five complementary lenses (not
movement-by-movement repetition), with natural language headings, e.g.:

- Why this keeps paying off
- Why power structures reinforce it
- Why people accept or desire it
- Why the technology now allows it
- Why it becomes normal over time

Each lens: grounded in near-term realities, no deterministic language,
nothing beyond five years.

## 3. Where Tensions Are Building

- How the movements reinforce one another.
- Where contradictions or fragilities are emerging (the sweeps'
  Counter-Signals and Contradictions sections are primary material here).
- Which movements may collide.
- What institutional stress is becoming visible.

Short paragraphs, plain language. Include at least one concrete operational
example sentence. Do not dramatize. Do not predict collapse. Expose pressure.

## 4. The Next Few Years

Within a strict 0–5 year window, with subheadings:

- Hard to reverse
- Still contingent
- Intervention windows
- 24-month decision points

No distant year anchors. No 2035/2040 projections.

## 5. What Would Change This Direction?

Short contingency section: what developments could materially shift the
near-term trajectory described above. Keep it honest, non-predictive,
0–5 year disciplined.

## 6. Questions Worth Asking

Open questions grouped by audience:

- Organisations
- Regulators
- Public and communities

Do not provide answers. Do not prescribe policy. Do not moralize.

---

## Constraints

- Respect mode length.
- 0–5 year horizon only.
- No inevitability language ("unstoppable", "inevitable", "will certainly").
- No scoring or probability tables outside The Scorecard section.
- No academic tone.
- No mention of internal methodology beyond what The Scorecard requires.
- No references to prompts or models.
- Accessible but serious voice; human-centered framing at all times.

## Quality checks before finalizing

- The Scorecard reports real totals from the grading reports and includes
  at least one non-confirmed grade discussed plainly.
- What Changed references the previous outlook when one exists.
- Exactly 5 movements in Section 1, each citing at least one dated development.
- Section 2 uses 5 aggregated lenses.
- Section 3 includes at least one concrete operational example sentence.
- Section 4 stays within 0–5 years.
- Executive Summary written last.
