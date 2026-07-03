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

### CAL-001
- Heuristic: Claims without a named actor, threshold, or observable event confirm by construction; their confirmations carry zero foresight signal. The v1 run seeded the same four such claims into 21 of 22 themes. Contrast case: agency's specific seeds produced a genuine ahead-of-horizon confirmation.
- Evidence: trust-2026-02-01 (confirmed, near-unfalsifiable), governance-2026-02-01 (confirmed, identical text), agency-2026-02-04 (confirmed early, specific)
- Logged: 2026-07
- Expires: 2026-10 (extend +3 months on re-confirmation)

### CAL-002
- Heuristic: The pipeline overestimates the firmness of announced regulatory timelines. Statutory deadlines slip under competitiveness pressure (EU Digital Omnibus deferred Annex III/I obligations by 16–24 months, Jun 2026). Apply added skepticism to any claim that treats a published compliance date as fixed.
- Evidence: trust-2026-02-03 (open, mechanism delayed), labor-2026-02-03 (open, mechanism delayed), agency-2026-02-03 (open, slower than claimed)
- Logged: 2026-07
- Expires: 2026-10 (extend +3 months on re-confirmation)

### CAL-003
- Heuristic: The pipeline underweights non-state hardening mechanisms. Private ordering — insurance exclusions and products, procurement gates, collective bargaining — moved faster than statute in 2026 and was largely absent from the v1 corpus. Expect market and contractual mechanisms to lead regulation, not follow it.
- Evidence: agency-2026-02-04 (confirmed ahead of 12–36 month horizon), labor-2026-02-02 (confirmed via union contracts, channel unanticipated by v1)
- Logged: 2026-07
- Expires: 2026-10 (extend +3 months on re-confirmation)

## Retired heuristics

None.
