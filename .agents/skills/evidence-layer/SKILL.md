---
name: evidence-layer
description: Produce a structured evidence layer for a theme. Supports mock mode and deep research mode.
---

# evidence-layer

## Purpose

Produce a structured evidence layer grounded in verifiable, recent sources.
This artifact is the factual substrate for all downstream steps.

## Input

theme: string
structural_question: string
use_deep_research: boolean

## Operating Modes

### Mode A: `use_deep_research = true` (production)

You must perform actual deep research, not shallow keyword search.

Research protocol (required):
1. Decompose the structural question into 4-6 research sub-questions.
2. Build and execute a deep-research pass for each sub-question:
   - prioritize primary sources first (official reports, regulator docs, company filings/blogs, standards bodies, peer-reviewed research)
   - use secondary analysis only to fill gaps
3. Collect 8-15 sources total, with at least 5 primary sources.
4. Triangulate "Confirmed Developments" with at least 2 independent sources per bullet.
5. Keep claims time-bounded:
   - Confirmed: event happened or formally announced.
   - Emerging: weak-signal but observable behavior, pilots, early deployments.
6. Track sources privately during research to verify each claim before writing.
7. If evidence quality is weak, output `None` for that subsection instead of inventing.

### Mode B: `use_deep_research = false` (development fallback)

Allow mock placeholders, but keep output schema identical.

## Output Format (strict)

Confirmed Developments:
- bullet

Emerging Signals:
- bullet

Counter-Signals:
- 1-2 bullets that weaken or complicate the dominant narrative

Regulatory Shifts:
- bullet or None

Capital Movements:
- bullet or None

Technical Changes:
- bullet or None

Contradictions:
- bullet or None

Horizon Classification:

0–12 months:
- bullet

12–36 months:
- bullet

36–60 months:
- bullet

## Constraints

- No narrative paragraphs
- No scenario writing
- No interpretation
- Do not fabricate sources, links, dates, or institutions
- Keep language concrete and falsifiable
- Preserve deterministic tone
- Include at least one counter-signal in every non-mock run
