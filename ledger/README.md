# Signals ledger

The persistent memory of the observatory. One file per theme, append-only.
Claims go in when a sweep logs them; grades go in when a later run checks
them against reality. Nothing is ever rewritten or deleted.

## Claim format

```markdown
### <theme>-YYYY-MM-NN
- Claim: <specific actor + observable expected event + timeframe>
- Horizon: <0–12 | 12–36 months> (logged YYYY-MM, resolve by YYYY-MM)
- Source: <URL, Mon YYYY that motivated the claim>
- Status: open | confirmed | decayed | falsified | expired
- Grades:
  - YYYY-MM: <grade> — <one sentence> (source: URL, Mon YYYY)
```

Rules:

- IDs are sequential within theme and month, never reused.
- `Status` mirrors the latest grade; `open` claims live under "Open claims",
  anything else under "Resolved claims".
- A grade other than `open` requires a source.
- Only `evidence-sweep` adds claims; only `signal-grading` adds grades.

## Seeded claims (2026-02)

Claims tagged `Source: none — seeded from pre-ledger 2026-02 run (method v1,
ungrounded)` were extracted from the February 2026 run's Horizon
Classification bullets. That run performed no real research, so treat these
as low-confidence statements of model priors. Grading them is still
valuable: it measures the ungrounded baseline that method v2 must beat.

## CALIBRATION.md

Bounded memo of the pipeline's observed biases. Written only by
`signal-grading`; read by `evidence-sweep`, `scenario-generator`, and
`scenario-eval`. Max 10 active heuristics, each citing >= 2 graded claim
IDs, each expiring after 3 months unless re-confirmed. See the learning
contract in CLAUDE.md.
