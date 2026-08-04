# Calibration memo

Written only by `signal-grading`. Read by `evidence-sweep`,
`scenario-generator`, and `scenario-eval` as context.

Hard bounds: max 10 active heuristics; each must cite >= 2 graded claim IDs;
each has an expiry and is retired unless re-confirmed by new grades.
This file never modifies skills, `instrument-review` is the human-gated
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
- Evidence: trust-2026-02-01 (confirmed, near-unfalsifiable), governance-2026-02-01 (confirmed, identical text), agency-2026-02-04 (confirmed early, specific), coordination-2026-02-04 (decayed on a different survey than the one that confirmed its identically worded siblings), truth-2026-02-03 (open, second identical open verdict on different sources), trust-2026-02-04 (open, second identical open verdict), power-2026-02-03 (open, no path to resolution before 2029-02)
- Logged: 2026-07
- Expires: 2027-01 (extend +3 months on re-confirmation)

### CAL-002
- Heuristic: The pipeline overestimates the firmness of announced regulatory timelines. Statutory deadlines slip under competitiveness pressure (EU Digital Omnibus deferred Annex III/I obligations by 16–24 months, Jun 2026). Apply added skepticism to any claim that treats a published compliance date as fixed.
- Evidence: trust-2026-02-03 (open, mechanism delayed), labor-2026-02-03 (open, mechanism delayed), agency-2026-02-03 (open, second recorded deferral of the same mechanism, Omnibus in force 29 Jul 2026), security-2026-02-03 (open, Annex III moved to Dec 2027 and embedded product to Aug 2028), coordination-2026-02-04 (decayed, Jun 2026 proposal became binding law), learning-2026-02-03 (open, deferral now statutory rather than political); counter-signal: trust-2026-07-01 (open, replacement Annex III date holding with no further deferral), governance-2026-07-01 (confirmed, low-cost transparency duties landed on schedule)
- Logged: 2026-07
- Expires: 2027-01 (extend +3 months on re-confirmation)

### CAL-003
- Heuristic: The pipeline underweights non-state hardening mechanisms. Private ordering, insurance exclusions and products, procurement gates, collective bargaining, moved faster than statute in 2026 and was largely absent from the v1 corpus. Expect market and contractual mechanisms to lead regulation, not follow it.
- Evidence: agency-2026-02-04 (confirmed ahead of 12–36 month horizon), labor-2026-02-02 (confirmed via union contracts, channel unanticipated by v1), meaning-2026-07-02 (confirmed via SAG-AFTRA ratification and 2026 nurse contracts, not the named employer or regulator), meaning-2026-07-03 (confirmed via bargained and grievance channels), agency-2026-07-02 (open, card networks built agent liability products pre-emptively with no incident trigger), security-2026-07-02 (open, vendor-scoped registries moved while the named marketplace mandate did not); counter-signal: autonomy-2026-07-03 (open, motion was state-led via NIST and GSA rather than vendor-led), dependency-2026-07-02 (open, channel was state compulsion plus market exit)
- Logged: 2026-07
- Expires: 2027-01 (extend +3 months on re-confirmation)

### CAL-004
- Heuristic: The pipeline logs claims whose triggering event is already in the public record at logging time, so the claim confirms on the first grading pass and the confirmation measures retrieval coverage rather than foresight. 15 of this run's 17 confirmations were satisfied by evidence dated before the claim's own logging month. Treat any confirmation that lands within one grading cycle of logging as a suspected retrodiction until the qualifying event is shown to postdate the claim.
- Evidence: desire-2026-07-03 (confirmed, threshold cleared by Washington HB 2225 in Mar 2026 and twelve states by Jun 2026, before the claim was written), memory-2026-07-02 (confirmed, both qualifying vendor shipments public 2 Mar and 26 Mar 2026), perception-2026-07-02 (confirmed, Google default shipped Sep 2025 and Samsung Feb 2026), power-2026-07-03 (confirmed, Abilene cancellation Mar 2026 and Utility Dive reporting Apr 2026), truth-2026-07-03 (confirmed, Munich ruling handed down 28 May 2026), belonging-2026-07-02 (confirmed, Folk and Dunn panel study published Mar 2026), autonomy-2026-07-02 (confirmed, qualifying ministry decision announced 19 Jun 2026), identity-2026-07-02 (confirmed on evidence predating the logging month), responsibility-2026-07-02 (confirmed, already satisfied by Mar and Apr 2026 statutes), intelligence-2026-07-01 (confirmed, benchmark target near-met at logging time)
- Logged: 2026-08
- Expires: 2026-11 (extend +3 months on re-confirmation)

## Retired heuristics

None.
