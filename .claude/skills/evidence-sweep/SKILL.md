---
name: evidence-sweep
description: Real, cited research scan for one theme, what changed since its previous sweep, plus new falsifiable ledger claim candidates. Runs for the run's cohort (11 themes) as Phase B.
---

# evidence-sweep

## Purpose

Produce the factual substrate for the month: verified, dated, sourced
developments per theme, a delta against the theme's ledger, and new
gradeable claims. Replaces the v1 `evidence-layer`.

There is no mock mode in production. Mock output is allowed only when
explicitly invoked with `mock=true` during development, and mock files must
carry a `MOCK, not evidence` first line.

## Input

theme: string
ledger: ledger/<theme>.md (including grades just written in Phase A)
grading: output/YYYY-MM-DD/01-grading/<theme>.md (if present)
calibration: ledger/CALIBRATION.md (active heuristics only)
current_run_date: YYYY-MM-DD
previous_sweep: this theme's sweep file from its previous run (the Delta baseline)
all_open_claims: open claims in every ledger/*.md (to avoid duplicate candidates)

## Research protocol (required)

1. Derive 3–5 sub-questions from the theme's open ledger claims and the
 latest grading surprises.
2. Search primary sources first (regulator docs, filings, standards bodies,
 peer-reviewed research, official announcements); use secondary analysis
 only to fill gaps.
3. Collect 6–12 sources. Every Confirmed bullet needs 2 independent sources.
4. Apply active calibration heuristics as added skepticism, not as facts.
5. If evidence is weak for a subsection, write `None`. Never fabricate
 sources, links, dates, or institutions.
6. Before writing each Ledger Candidate, run one search against the candidate
 itself, asking whether the named event has already happened. If it has,
 either raise the threshold past the current value or discard the candidate.
 Sequential thresholds ("a second state", "a third vendor") require the
 current count, not an assumption about it.
7. Source discipline: open every page you cite and check its publication
 date; never cite from a search-result title or summary. Verify any
 enforcement action, fine, filing or statute against the issuing body's own
 site or two independent reputable outlets; AI-generated aggregators
 fabricate citable-looking regulatory actions. An item that fails
 verification may appear only under Contradictions, marked unverified.
8. A primary source that cannot be opened (HTTP 403, paywall, timeout) is
 unverified, never evidence of absence. Say which page could not be opened.
9. Check at least one non-English source where the theme has a
 non-Anglophone regulatory or market dimension.

## Output format (strict), output/YYYY-MM-DD/02-sweep/<theme>.md

THE CITATION GATE IS HARD: every bullet under Confirmed Developments,
Regulatory Shifts, Capital Movements, and Technical Changes must end with
`(source: URL, Mon YYYY)`, Confirmed bullets with two. Emerging Signals
and Counter-Signals need at least one source each. A file violating this
is invalid and must be regenerated, not patched.

```text
Delta Since Last Sweep:
- 2-4 bullets: what is new vs. the ledger and theme's previous sweep, or "first sweep under method v2". Every dated factual
 assertion here carries `(source: URL, Mon YYYY)`.

Confirmed Developments:
- bullet (source: URL, Mon YYYY) (source: URL, Mon YYYY)

Emerging Signals:
- bullet (source: URL, Mon YYYY)

Counter-Signals:
- 1-2 bullets that weaken or complicate the dominant narrative (source: URL, Mon YYYY)

Regulatory Shifts:
- bullet (source: URL, Mon YYYY) or None

Capital Movements:
- bullet (source: URL, Mon YYYY) or None

Technical Changes:
- bullet (source: URL, Mon YYYY) or None

Contradictions:
- bullet or None

Ledger Candidates:
- 2-4 NEW forward-looking claims. Each names a specific actor, an observable
 expected event, and a resolve-by month, gradeable by a future run.
- Each candidate carries a second line, `Not yet true as of <run date>:`,
 stating the current value of the thing the claim measures (the count, the
 status, the absence) with a source. If that line cannot be written, the
 candidate is not a claim about the future.
- Tag a candidate `(pre-announced)` when it forecasts execution of a plan an
 actor has already published (a promised disclosure, a scheduled vote, the
 next step of a filed rulemaking). Such claims are allowed but carry little
 foresight; prefer candidates the public record does not already imply.
```

## Ledger append (done by the orchestrator, not here)

Do not edit the ledger. The orchestrator collects every sweep's Ledger
Candidates after Phase B, removes duplicates across themes and against all
open ledger claims, and appends the survivors with sequential IDs
`<theme>-YYYY-MM-NN`. Write candidates so they can be compared: name the
actor and the observable event in the first clause.

## Constraints

- No narrative paragraphs, no interpretation, no scenario prose.
- Time-bound every claim; concrete and falsifiable language only.
- Do not repeat a still-open ledger claim as a new Ledger Candidate, in this
 theme or any other theme's ledger.
- A candidate that a competent search at the run date would already grade
 confirmed is invalid, not merely weak. Retrodiction measures this pipeline's
 retrieval coverage, not its foresight.
- Prefer a resolve-by month at which at least one observable event can occur
 within the next two runs of this cohort (about eight weeks), or state why
 the claim is worth a slower clock.
