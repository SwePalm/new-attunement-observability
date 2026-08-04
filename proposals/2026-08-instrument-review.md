# Instrument review, 2026-08

Run date: 2026-08-04
METHOD_VERSION at review time: 2.1
Git SHA of the run reviewed: e355d24b66812101c899ff336a3cb099dda7e6e3
Reviewer: instrument-review (proposals only, nothing applied)

## Inputs read

- `ledger/CALIBRATION.md` (CAL-001 through CAL-004, all active, no retirements)
- `output/2026-08-04/01-grading/` (22 files) and `output/2026-07-03/01-grading/` (22 files)
- `output/2026-08-04/02-sweep/` (22 files), consulted to test propagation claims
- `output/2026-08-04/07-scenario/` and `output/2026-07-03/07-scenario/` (5 + 5)
- `output/2026-08-04/08-evaluation/` (5 files) and `output/2026-07-03/08-evaluation/` (5 files)
- `output/2026-08-04/SELECTION.md`, `output/2026-07-03/SELECTION.md`, `output/2026-08-04/PROGRESS.md`
- `.claude/skills/scenario-generator/`, `evidence-sweep/`, `scenario-eval/`, `forces-feelings/`, `orchestrator/`

Three proposals follow, against the 0 to 5 maximum. Two are recommended for
merge. One is written up in full and recommended for hold, because the
mechanism clears the two-instance bar but the demonstrated harm does not.

---

## Proposal 1: scenario-generator, vantage variation in Section 3

Target skill: `.claude/skills/scenario-generator/SKILL.md`

### Diff, hunk A (Section 3 requirements, lines 30 to 34)

Before:

```text
## 3. Future World Snapshot (The Lived Experience) – A Day in This Future
(300–400 words)
Requirements:
- Integrate at least **two** Normal Absurdities from Forces & Feelings.
- Center the protagonist's struggle around the Irreplaceable Thing.
```

After:

```text
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
```

### Diff, hunk B (Constraints, after line 72)

Before:

```text
- No new major institutions or technical primitives unless implied by sweep_output.
```

After:

```text
- No new major institutions or technical primitives unless implied by sweep_output.
- A regulatory commencement date shared across the corpus (for example an EU
 applicability date) may appear in Section 5 only where the theme's own
 sweep_output carries it as a Confirmed Development or Regulatory Shift, and
 it may not be the first structural force listed.
```

### Diff, hunk C (Section 9, line 62 to 63)

Before:

```text
## 9. Final Insight
(Short closing paragraph; no instructions)
```

After:

```text
## 9. Final Insight
(Short closing paragraph; no instructions)
Do not close on the run's default move (reasonable actors, structural outcome,
the Irreplaceable Thing named in the last clause). The Irreplaceable Thing has
already carried Section 3; if it appears here it must appear as a cost already
paid or a choice already refused, not as a reveal.
```

### Evidence

Scenario-eval subscores, Distinctiveness vs. Other Themes (1 to 10):

| run | theme | score |
|-----|-------|-------|
| 2026-07-03 | agency | 6 |
| 2026-07-03 | creativity | 6 |
| 2026-07-03 | governance | 6 |
| 2026-07-03 | labor | 7 |
| 2026-07-03 | security | 7 |
| 2026-08-04 | alignment | 4 |
| 2026-08-04 | authority | 3 |
| 2026-08-04 | coordination | 3 |
| 2026-08-04 | trust | 3 |
| 2026-08-04 | responsibility (first pass) | 3 |
| 2026-08-04 | responsibility (rebuilt) | 7 |

Mean 6.4 in 2026-07-03 against 3.2 across the five 2026-08-04 first passes.
Five independently run evaluations converged on the same diagnosis without
seeing each other, and `output/2026-08-04/PROGRESS.md` records the convergence
as a flagged method problem rather than a content problem.

Was it latent or new? Both, at different layers, and the diff targets only the
new layer. Convergence at the level of thesis was already present and already
scored in 2026-07-03: `08-evaluation/agency.md` adjusts a weighted 8.75 down to
8.4 for "the corpus-level convergence burden ... this is the 5th instance of the
pattern", and the creativity, governance and security evaluations each name the
shared private-ordering spine as a distinctiveness deduction. That was thesis
convergence, and it scored 6 to 7 because the worlds still looked different.

What is new in 2026-08-04 is surface convergence, which the July scenarios do
not show. Checked directly against `07-scenario/*.md` Section 3 openers:

- named weekday in the opening lines: 4 of 5 in August (alignment Tuesday,
 authority Thursday, trust Tuesday, coordination by daypart sequence), 1 of 5
 in July (governance "Her Tuesday begins").
- explicit in-world year 2029 in the opening lines: 2 of 5 in August
 (alignment, authority), 0 of 5 in July.
- organisation headcount or entity size in the first sentence: 3 of 5 in August
 (300 staff plus a 40-person subsidiary, about 1,100 staff, 412 agents), 0 of 5
 in July.
- European entity inside the corporate structure: 4 of 5 in August (Dublin,
 Dublin, Malmo, Rotterdam), 1 of 5 in July (a mid-sized European HR-tech firm).
- mid-senior professional inside the institution as protagonist: 5 of 5 in
 August first passes, 3 of 5 in July (agency's protagonist is a consumer,
 creativity's is a freelance illustrator).

The rebuilt responsibility scenario is the controlled test. It is the only
August artifact that abandons the template (a tenant with no claim, in a rented
room, no headcount, no weekday, no professional vantage), and it is the only one
whose Distinctiveness moved, 3 to 7, on the same theme, same sweep and same
method version. `08-evaluation/responsibility.md` attributes the move to exactly
this: "the artifact abandons the run's professional-insider template".

Mechanism, which is why the fix has to sit inside the skill: `orchestrator`
Phase D runs different themes in parallel subagents, so `scenario-generator`
never sees a sibling scenario. Nothing in the skill varies the vantage and one
line actively fixes it ("Center the protagonist's struggle around the
Irreplaceable Thing", with `forces-feelings` producing exactly one scarce
pursuable good per theme). Convergence is the skill's default output, not an
execution lapse, and no calibration heuristic can reach it.

### Expected measurable effect

- Distinctiveness vs. Other Themes subscore in `08-evaluation/` returns to the
 6 or above band on at least 4 of 5 scenarios in the next run.
- Vantage declarations across a run's selected themes show at least three
 distinct role classes, countable directly from the new one-line field.
- Weighted total moves little (distinctiveness carries 5%, so the expected
 direct gain is about 0.15 to 0.20 per scenario). The real target is the
 corpus, not the score: `outlook-generator` currently has to synthesise five
 worlds that read as one voice.

### Drift risk

Forcing the vantage away from the institution can push a scenario away from
where its evidence actually sits, buying distinctiveness with grounding. A
partial instance is already visible: the responsibility rebuild gained
Distinctiveness (3 to 7) and Cross-Layer Grounding (5 to 7) but lost Signal
Integrity (8 to 7) by reaching for an underwriting bridge its evidence did not
support. A future review detects overshoot as Distinctiveness rising while
Institutional Realism or Cross-Layer Grounding falls across the same run, or as
scenarios choosing "person subject to the system" for themes whose sweep
evidence is entirely regulatory and corporate. Secondary risk: the vantage line
is meta-commentary of a sort, and the skill already forbids meta-commentary; it
should be stripped by `outlook-generator` and never reach a reader.

---

## Proposal 2: evidence-sweep, forward-looking test on Ledger Candidates

Target skill: `.claude/skills/evidence-sweep/SKILL.md`

### Diff, hunk A (Output format, Ledger Candidates, lines 71 to 73)

Before:

```text
Ledger Candidates:
- 2-4 NEW forward-looking claims. Each names a specific actor, an observable
 expected event, and a resolve-by month, gradeable by a future run.
```

After:

```text
Ledger Candidates:
- 2-4 NEW forward-looking claims. Each names a specific actor, an observable
 expected event, and a resolve-by month, gradeable by a future run.
- Each candidate carries a second line, `Not yet true as of <run date>:`,
 stating the current value of the thing the claim measures (the count, the
 status, the absence) with a source. If that line cannot be written, the
 candidate is not a claim about the future.
```

### Diff, hunk B (Research protocol, after line 36)

Before:

```text
5. If evidence is weak for a subsection, write `None`. Never fabricate
 sources, links, dates, or institutions.
```

After:

```text
5. If evidence is weak for a subsection, write `None`. Never fabricate
 sources, links, dates, or institutions.
6. Before writing each Ledger Candidate, run one search against the candidate
 itself, asking whether the named event has already happened. If it has,
 either raise the threshold past the current value or discard the candidate.
 Sequential thresholds ("a second state", "a third vendor") require the
 current count, not an assumption about it.
```

### Diff, hunk C (Constraints, after line 86)

Before:

```text
- Do not repeat a still-open ledger claim as a new Ledger Candidate.
```

After:

```text
- Do not repeat a still-open ledger claim as a new Ledger Candidate.
- A candidate that a competent search at the run date would already grade
 confirmed is invalid, not merely weak. Retrodiction measures this pipeline's
 retrieval coverage, not its foresight (CAL-004).
```

### Evidence

CAL-004 (logged 2026-08, expires 2026-11): 15 of this run's 17 confirmations
were satisfied by evidence dated before the claim's own logging month. Verified
against `output/2026-08-04/01-grading/`, which records 17 confirmations across
autonomy, belonging (2), dependency, desire (2), governance, identity,
intelligence, meaning (2), memory, perception, power, responsibility, security
and truth.

Graded claim IDs supporting the change, each confirmed on evidence predating the
July 2026 logging month, with the qualifying date from the grading file:

- `desire-2026-07-03`: threshold "a second state" already cleared by Washington
 HB 2225 (24 Mar 2026), twelve states by Jun 2026. The grading file states the
 threshold "was cleared before the claim was written".
- `responsibility-2026-07-02`: Washington HB 2225 (Mar 2026) and Oregon SB 1546
 (Apr 2026). Grading Surprises: "already satisfied before it was written".
- `memory-2026-07-02`: both qualifying vendor shipments public 2 Mar and 26 Mar
 2026, "both predating the month the claim was logged".
- `perception-2026-07-02`: Google Pixel default Sep 2025, Samsung Feb 2026.
- `power-2026-07-03`: Abilene cancellation Mar 2026, reporting Apr 2026.
- `truth-2026-07-03`: Munich ruling 28 May 2026. The 2026-08-04 truth sweep
 itself calls it a ruling "which retroactively satisfied truth-2026-07-03".
- `belonging-2026-07-02`: Folk and Dunn panel study Mar 2026.
- `autonomy-2026-07-02`: Norwegian ministry decision announced 19 Jun 2026.
- `identity-2026-07-02`: confirmed on Apr 2026 evidence; the sweep notes the
 consumer-facing launch only posted 23 Jul 2026.
- `intelligence-2026-07-01`: benchmark target near-met at logging time.
- `desire-2026-07-01`: both limbs "already met by major vendors" (Jun 2026).

Eleven graded instances against a bar of two.

Why this belongs in the instrument rather than in calibration. CAL-004 is
correctly written as an instruction to the grader: treat a fast confirmation as
a suspected retrodiction. The learning contract routes calibration to
`evidence-sweep` as "added skepticism, not as facts", which is skepticism about
the world. The defect is not in how the sweep reads evidence, it is in how the
sweep constructs claims, and no wording of a calibration heuristic reaches that
step. CAL-004 can make every future run correctly identify retrodictions after
the fact and still produce a corpus that is 88% retrodictive. This is the
difference between recalibrating and regrinding, and it is the case the skill's
telescope principle is written for.

The change is additive (a required line and one search), which the skill's rules
hold to a lower bar than removing a constraint.

### Expected measurable effect

- Share of confirmations satisfied by evidence predating the claim's logging
 month falls from 15 of 17 to under 40% by the 2026-10 grading pass, countable
 directly from the Grade Details date against the claim ID's month segment.
- Expect the absolute confirmation count to fall and the open count to rise.
 That is the intended direction, not a regression, and `delta-report` should
 be read accordingly at the next run.
- Secondary: `theme-selection` grade-surprise scores should become more
 informative, since a retrodictive confirmation currently scores as a surprise
 while carrying no forecast information.

### Drift risk

The sweep can satisfy the constraint by writing claims that are un-retrodictable
because they are unresolvable: pushing resolve-by months past the review
horizon, or picking thresholds so obscure that no future run can grade them.
That converts CAL-004's failure into CAL-001's failure ("no path to resolution
before 2029-02"). A future review detects it as the mean gap between logging
month and resolve-by month lengthening, as the open share climbing while
confirmed, decayed and falsified all fall toward zero, or as a rise in expired
grades. If confirmations fall below roughly 5% of graded claims for two
consecutive runs, the constraint has overshot and the threshold language should
be loosened rather than the search requirement removed.

---

## Proposal 3: evidence-sweep, carry this run's grades forward (RECOMMEND HOLD)

Target skill: `.claude/skills/evidence-sweep/SKILL.md`

### Diff (Output format, Delta Since Last Sweep, lines 47 to 48)

Before:

```text
Delta Since Last Sweep:
- 2-4 bullets: what is new vs. the ledger and previous sweep, or "first sweep under method v2"
```

After:

```text
Delta Since Last Sweep:
- 2-4 bullets: what is new vs. the ledger and previous sweep, or "first sweep under method v2"
- Plus one bullet headed "Grades carried forward", naming every claim this
 run's grading file graded confirmed, decayed or falsified, and for each
 either the sweep bullet that carries its qualifying evidence or an explicit
 note that later evidence supersedes it. A grade written in Phase A may not
 vanish in Phase B. Downstream steps read this bullet as settled for the
 theme.
```

### Evidence

The documented failure. `01-grading/responsibility.md` graded
`responsibility-2026-07-02` confirmed on Washington HB 2225 (private right of
action, signed 24 Mar 2026) and Oregon SB 1546 ($1,000 per violation, signed
1 Apr 2026). The first-pass `02-sweep/responsibility.md` carried neither, and the
deep-dive chain built on it concluded that no remedy routes to a harmed
individual, which is the negation of the pipeline's own confirmed grade.
`08-evaluation/responsibility.md` records the result: a 5.8 score, the finding
described as "the most serious single defect in the run" in PROGRESS.md, and a
six-step chain regeneration. The repaired sweep and the rebuilt scenario score
6.8. Cost of the miss: one full theme chain, plus a sweep regeneration.

Does the mechanism recur? Checked all 17 confirmations in this run against the
same theme's sweep file. Three sweeps reconcile the confirmed grade explicitly
(`belonging-2026-07-01`, where the sweep records that New York S9051B is still
unsigned and thereby catches a bad grade; `identity-2026-07-02`, where the sweep
flags the confirmation as resting on April evidence; `truth-2026-07-03`, flagged
as retroactive). Six drop the qualifying substrate entirely:

- `responsibility-2026-07-02`: Washington HB 2225 and Oregon SB 1546, absent.
- `dependency-2026-07-01`: the APRA 30 Apr 2026 letter, absent.
- `perception-2026-07-02`: Pixel and Samsung C2PA capture defaults, absent.
- `security-2026-07-01`: the Check Point Mexican-agency campaign, absent.
- `meaning-2026-07-02`: the SAG-AFTRA ratification, absent.
- `memory-2026-07-02`: Anthropic and Google memory portability, absent.

Six graded instances, against a bar of two. So the mechanism clears the bar.

Why the recommendation is still hold. Five of those six drops are harmless, and
arguably correct. `evidence-sweep` is a delta instrument; not restating
month-old evidence is its job. In dependency, perception, security, meaning and
memory the sweep replaced the dropped substrate with newer evidence pointing the
same direction (UK Critical Third Parties designation and the ESRB warning; the
C2PA distribution layer and Apple SynthID; the Hugging Face and Anthropic
containment escapes; the SUNY contract; system-written memory and MemGhost). No
downstream artifact contradicted a grade in any of them.

The harmful conjunction is a drop plus a deep dive, and it occurred once. It
could only have occurred once: of the five themes selected in `SELECTION.md`,
only responsibility had any confirmation in Phase A (alignment, authority,
coordination and trust recorded zero confirmations each). So the observed rate
is 1 of 1 opportunity, which is not a rate. The prior run gives no comparison
either: every 2026-07-03 confirmation was a retired v1 boilerplate claim
(`*-2026-02-01` and `*-2026-02-02`), so no method-v2 grade was available to
contradict.

The honest position is that the mechanism is real and the harm is unmeasured.
The pipeline also caught this defect unaided, at `scenario-eval`, which is the
instrument working as designed, expensively. Re-test in 2026-09 and 2026-10 by
counting, for each deep-dived theme, whether it carried a confirmed grade and
whether the chain contradicted it. Two harmful instances make this proposal
merge-ready without further argument.

### Expected measurable effect (if merged)

- Zero instances of a Phase D artifact asserting the negation of a grade written
 in the same run's Phase A, checkable as a `scenario-eval` Signal Integrity
 finding.
- Zero chain regenerations attributable to dropped grading evidence (one this
 run).
- Confirmed grades whose substrate is absent from the same-run sweep falls from
 6 of 17 toward zero.

### Drift risk

`evidence-sweep` exists to answer "what changed". Obliging it to restate
evidence that is by definition not new bloats the file and dilutes the signal
`theme-selection` scores. A future review detects this as evidence-delta scores
in `SELECTION.md` compressing toward the top of the range across all 22 themes,
removing selection discrimination, or as Confirmed Developments sections growing
while the Delta section repeats them. Placing the requirement in Delta rather
than in Confirmed Developments is the mitigation: it is a reconciliation line,
not an evidence line, and it should not carry new sources.

---

## Assessed and not proposed

**Scenarios naming calibration heuristics in reader-facing prose.**
`08-evaluation/responsibility.md` finds that 7.2 "invokes CAL-003 as a warrant
when a calibration heuristic is a statement about the pipeline, not about the
world", and PROGRESS.md flags the pattern. Checked: every scenario in both runs
names a CAL heuristic exactly once, 5 of 5 in 2026-08-04 and 5 of 5 in
2026-07-03, so this is stable, not drift. More decisively, the rule already
exists. `scenario-generator` Constraints already say "No meta-commentary", and a
calibration ID in Section 7.2 is meta-commentary. Adding a second constraint for
a defect the first constraint already covers is instrument bloat, not learning.
This belongs in the eval's Narrative Inflation Control finding and, if it
persists at the reader-facing layer, in `outlook-generator`'s stripping pass.

**Reweighting Distinctiveness in scenario-eval.** At 5% the subscore that
diagnosed the run's largest method problem moves the reported score by at most
0.2. Raising the weight would make the signal visible, but changing a scoring
weight breaks comparability across every prior scorecard for a benefit that
Proposal 1 delivers without touching the scale. Noted for a future review if
Proposal 1 merges and distinctiveness does not recover.

**CAL-001, CAL-002, CAL-003 as instrument changes.** None proposed. CAL-001's
evidence is entirely retired v1 seed claims and does not describe method-v2
claim construction. CAL-002 and CAL-003 both carry live counter-signals in the
memo (`trust-2026-07-01` and `governance-2026-07-01` against CAL-002;
`autonomy-2026-07-03` and `dependency-2026-07-02` against CAL-003) and are
working correctly as attentional corrections. All three were extended to 2027-01
this run and should stay in calibration.

---

## Recommendation

**Merge some.**

- Proposal 1 (scenario-generator, vantage variation): merge. Ten scored
 instances across two runs, a controlled within-theme test showing the fix
 works, and a mechanism no calibration heuristic can reach.
- Proposal 2 (evidence-sweep, forward-looking test on Ledger Candidates):
 merge. Eleven graded instances, and CAL-004 is structurally unable to fix
 the step where the defect occurs.
- Proposal 3 (evidence-sweep, grades carried forward): hold. The mechanism
 recurs six times but the harm has one instance out of one opportunity.
 Re-test at 2026-09 and 2026-10 and merge on a second harmful instance.

If the human merges any proposal, bump METHOD_VERSION in `CLAUDE.md`.

**Scorecard comparability resets at the version boundary.** Scenario-eval
subscores, weighted totals, grading scorecards and `theme-selection` dimension
scores produced under 2.1 are not comparable with those produced after any merge
here. In particular the 2026-07-03 band (8.1 to 8.5) and the 2026-08-04 band
(5.8 to 7.3, or 6.2 to 7.3 counting the responsibility rebuild) close as a
series at that boundary, and the first run under the new version starts a new
series rather than continuing this one. Proposal 2 is expected to move the
Phase A scorecard shape as well, lowering confirmations and raising opens, so
the confirmation-rate series also resets rather than declining.

Nothing in this file has been applied. No skill file, ledger file or
CALIBRATION.md was modified by this review.
