# Calibration memo

Written only by `signal-grading`. Read by `evidence-sweep`,
`scenario-generator`, and `scenario-eval` as context.

Hard bounds: max 10 active heuristics; each must cite >= 2 graded claim IDs;
each has an expiry and is retired unless re-confirmed by new grades.
This file never modifies skills — `instrument-review` is the human-gated
path for method changes.

Heuristic format:

```markdown
### CAL-NNN
- Heuristic: <falsifiable statement about this pipeline's bias>
- Evidence: <claim-id> (<grade>), <claim-id> (<grade>)
- Logged: YYYY-MM
- Expires: YYYY-MM (extend +3 months on re-confirmation)
```

## Active heuristics

None yet — the first grading pass has not run.

## Retired heuristics

None.
