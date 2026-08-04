# Learnings, run 2026-08-04

METHOD_VERSION 2.1. Written for the human, as input to skill development in code
mode. Nothing here has been applied. Formal proposals with diffs live in
`proposals/2026-08-instrument-review.md`.

## 1. The pipeline was scoring itself on retrodictions

15 of the 17 confirmations in this run were satisfied by evidence dated before the
claim's own logging month. The 2026-07 sweep logged as forecasts a set of events
that had already happened, so those confirmations measured retrieval coverage, not
foresight. Logged as CAL-004.

Worked examples: `desire-2026-07-03` cleared by a Washington statute from March,
`belonging-2026-07-02` by a panel study published in March, `power-2026-07-03` by
the Abilene cancellation in March, `autonomy-2026-07-02` by a Norwegian ministry
decision from 19 June, all predating the claims written to predict them.

Mitigation applied this run at the prompt level only: Phase B agents were told to
verify each candidate claim was not already in the public record before appending.
Whether that worked is a question only the September run can answer. Resist reading
a lower confirmation rate next month as a regression; it is more likely the
instrument starting to tell the truth.

Skill implication for consideration: `evidence-sweep` has no structural obstacle to
logging a past event as a future claim. The novelty check currently depends on the
prompt.

## 2. Confirmed grading evidence does not propagate into the sweep

`evidence-sweep` takes the grading file as an input, but nothing obliges it to carry
forward what Phase A just confirmed.

Concrete failure: Phase A graded `responsibility-2026-07-02` confirmed on Washington
HB 2225 (private right of action) and Oregon SB 1546 (statutory damages). The sweep
dropped it. The only mention of a private right of action in the sweep was in the
negative, noting Illinois AISMA lacks one. All six Phase D steps inherited that gap
and concluded that nothing routes remedy to the harmed individual, contradicting the
pipeline's own confirmed grade. Eval 5.8.

This is the most dangerous failure mode found so far, because every downstream
artifact was internally consistent and well cited. Nothing in the citation gate or
the eval rubric catches a true statement built on an incomplete substrate. The
defect was only visible by diffing the grading file against the sweep.

Repair: rebuilt from the sweep down, 5.8 to 6.8. The rebuilt chain found the sharper
truth, that individual remedy exists in a narrow companion-chatbot lane while
frontier-audit regimes route around it, and that Oregon is the only one of 14 state
companion-chatbot laws enacted in 2026 whose text lets a harmed user sue.

## 3. Scenario template convergence, with a controlled test

All five scenario evals independently scored Distinctiveness at 3 or 4 out of 10.
Every scenario opened on a named mid-senior professional at a headcount-specified
organisation on a named weekday in 2029, placed a European entity in the corporate
structure, used the 2 Aug 2026 EU commencement as a structural force, and closed on
the same move: reasonable actors, structural outcome, one scarce good named at the
end.

The responsibility rebuild became an accidental controlled experiment. Same theme,
same skill, same sweep, with the single change being an instruction to abandon the
house form. Distinctiveness moved 3 to 7. That isolates the cause to prompt-level
form rather than to the themes, the evidence, or the model. The 2026-07-03 run
scored 6, 6, 6, 7, 7 on the same dimension, so this is a regression, not a constant.

## 4. Claim quality problems visible only at grading time

Grading surfaced several claims that were unresolvable the day they were written:

- `agency-2026-07-01` named Morgan Stanley and Adobe as trackers for a metric
  neither publishes, and its threshold contradicted Morgan Stanley's actual
  published forecast.
- `alignment-2026-07-02` assumed a publication cadence the institution has never
  stated.
- `belonging-2026-07-03` referenced "the next national survey wave" when the
  relevant survey had dropped the item and another used a different instrument and
  base.

A pre-append check on whether a named data source actually publishes the named
metric would have caught all three.

## 5. Format drift that the gate does not cover

45 ledger `Source:` lines were written without the required month and year. The
citation gate governs sweep bullets, not ledger entries, so this passed silently.
All were backfilled from the date the same URL carries in its sweep file or in the
URL path; none were inferred.

Two smaller items: a regenerated sweep appends a second set of ledger claims on top
of the first pass's, since the append-only invariant forbids removing them
(autonomy and creativity carry 7 and 8 claims rather than 4). And Phase A recorded
Oregon SB 1546 as signed 1 Apr 2026 when the correct date is 31 Mar 2026, caught
during the repair and noted rather than silently overwritten.

## 6. What went right and should not be changed

- The 22-theme grading and sweep layers are complete and the gate held on all 22.
- `theme-selection` behaved exactly as designed. Staleness pushed all five picks
  into the never-dived backlog even though the four largest evidence deltas
  (agency, security, creativity, labor) belonged to July's themes. The coverage
  rule beat the news cycle without anyone overriding it.
- Adversarial evaluation earned its cost twice: the scenario evals found the
  responsibility defect, and the outlook review caught two factual errors in the
  draft essay, a conflated ten-day detection window and a claim that both labs
  disclosed voluntarily when disclosure ran through the victim in OpenAI's case.
- The delta report rejected an incorrect open-claim count it was handed and
  reconciled it two ways instead.

## 7. Known structural gap, unresolved

Phases A and B cover all 22 themes. Phase D narrows to 5. Post-processing that
expects 22 scenarios finds holes. Raised 2026-08-04, deferred by decision, still
open.
