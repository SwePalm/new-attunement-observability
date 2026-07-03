---
name: outlook-generator
description: Generate "The Outlook", a forward-looking, human-centered narrative essay on where human-AI systems are heading, grounded in this month's evidence sweeps and deep-dive scenarios. Storytelling-first. The accountability material lives in delta-report, not here. Manual, after human review.
---

# outlook-generator

## Purpose

Generate "The Outlook": a readable, forward-looking essay on the near-term
(0-5 year) direction of human-AI systems, grounded in the month's corpus.

This is not a forecast, not a framework, not a policy document, and NOT a
self-audit. The accountability record (how past claims graded, what changed,
what the pipeline learned) belongs in the separate `delta-report` skill. Keep
this document a story.

The voice is calm, serious, human-centered, and accessible to a thoughtful
general reader. It should read like a good essay, not a filled-in form.

## Style rules (hard)

- NO em-dashes (the "long dash" character) anywhere. Use commas, periods,
  colons, or parentheses. This applies to every artifact the pipeline
  produces; it is enforced here because the outlook is the reader-facing one.
- No numbered schema sections, no lens labels, no bracketed theme-tag lines.
  Let the themes appear as evidence inside the prose, not as a checklist.
- No inevitability language ("unstoppable", "inevitable", "will certainly").
- No probability tables, no scores, no methodology talk.
- Ground every structural claim in a dated development from the sweeps, but
  weave the citation into the sentence rather than footnoting it.

## Inputs

- `scenario_outputs` (this month's deep-dive scenarios)
- `sweeps` (all theme evidence sweeps, for breadth)
- `selection` (SELECTION.md)
- `mode` (`debug` or `production`)

## Length

- `debug`: 1,000-1,500 words (a tight, complete draft for review)
- `production`: 3,000-4,000 words (fuller development of the same structure)

## Structure (narrative, not schema)

Write a flowing essay. The following are movements of the piece, not headings
to stamp in mechanically. In production, each expands; in debug, each is brief.

1. **Standfirst.** Title, month, draft status, and one italic line pointing the
   reader to the Delta Report for the accountability record.

2. **The opening.** State the single most important thing taking shape this
   month, as a plain-spoken observation a person would care about. Do not bury
   it under structure. One to three short paragraphs.

3. **The human stakes (the heart).** Carry the month's movement through the
   concrete things it makes scarce or abundant for real people. The deep-dive
   scenarios each surface one "irreplaceable thing"; use those as the essay's
   spine. Give each a short vivid paragraph grounded in that theme's evidence.
   Aim for a unifying thread across them, not a list.

4. **Why it keeps happening.** In flowing prose (not five labeled lenses),
   explain why the movement persists now: why it pays off, why power reinforces
   it, why people accept it, why the technology allows it, why it becomes
   normal. Synthesize; do not enumerate.

5. **Where it strains.** The tensions, fragilities, and collisions, with at
   least one concrete, observable example. Expose pressure; do not predict
   collapse or dramatize.

6. **What is still open.** Forward-looking and honest about contingency: what
   looks hard to reverse, what remains genuinely undecided, where the near-term
   intervention windows are, and which choices in the next 24 months matter.
   Keep it prose, not a claim list (the gradeable claims live in the ledger and
   the Delta Report).

7. **Questions worth sitting with.** A short closing set of open questions,
   grouped by who they are for (builders, rule-makers, the public). No answers,
   no prescriptions, no moralizing.

## Constraints

- 0-5 year horizon only; no distant-year anchors.
- Forward-looking: do not re-litigate the past baseline (that is the Delta
  Report's job).
- Human-centered framing throughout.
- The essay must stand on its own without the reader having seen any prior
  month or any internal method detail.

## Quality checks before finalizing

- Zero em-dashes.
- Reads as a continuous essay, not a schema.
- The deep-dive stakes appear as a coherent spine with a unifying thread.
- Every structural movement is grounded in at least one dated development.
- No scorecard, no "what changed" audit, no claim tables (those are the Delta
  Report).
- Ends on open questions, grouped by audience.
