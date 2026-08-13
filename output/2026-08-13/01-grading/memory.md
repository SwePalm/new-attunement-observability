# Signal grading, memory, 2026-08-13

Scorecard:
- open: 5, confirmed: 1, decayed: 0, falsified: 0, expired: 0
- unchanged since 2026-08-04 (not re-graded): 5

Scope notes:
- The scorecard covers the 6 gradeable claims only. memory-2026-02-03 and
  memory-2026-02-04 are retired method-v1 seed claims and were not re-graded,
  per CLAUDE.md. They remain in the ledger's Open claims section untouched.
- The previous grading pass ran on 2026-08-04, nine days ago. Per this run's
  scoping rule, a claim gets a new ledger grade line only if its resolve-by
  month has arrived or real post-2026-08-04 evidence materially moves it.
  Only memory-2026-08-01 met that bar, and it met it by resolving outright.
- memory-2026-08-01 through memory-2026-08-04 were logged by Phase B of the
  2026-08-04 run and had never been graded. All four were researched this run
  as a first pass, including the CAL-004 retrodiction check. Three of them
  found no qualifying event and so received no ledger line.

Grade Details:
- memory-2026-08-01: confirmed, Microsoft already ships an explicit
  confirmation control before persistent memory writes, documented in official
  Microsoft developer and product documentation. The Visual Studio Copilot
  Memories post states that whenever Copilot is ready to save a new memory or
  update an existing one the user receives a confirmation nudge and can review,
  accept or adjust before preferences are updated, and the Microsoft 365 Copilot
  memory support page states that Copilot asks the user whether to save
  information it judges worth remembering. The claim's confirmation condition
  was satisfied roughly seven months before the claim was written (source:
  https://devblogs.microsoft.com/visualstudio/copilot-memories/, Jan 2026;
  https://support.microsoft.com/en-us/topic/manage-copilot-memory-in-microsoft-365-copilot-b3231eae-9e60-4b3c-ac58-81fddbe56279,
  Aug 2026)
- memory-2026-08-02: open, unchanged, no ledger line appended. Researched this
  run: no deletion-propagation guarantee exists in either vendor's help
  documentation, and OpenAI's own Memory FAQ documents the opposite position,
  that deleting a chat does not remove saved memory derived from it and the
  memory store must be managed separately. That is a standing counter-signal
  rather than post-2026-08-04 movement, and the claim is a disjunction over
  OpenAI or Anthropic with resolve-by 2027-06 still ahead, so it is not yet
  falsified.
- memory-2026-08-03: open, unchanged, no ledger line appended. Researched this
  run: the 2026-07-28 specification remains the most recent MCP release, with
  nothing dated after it on the release blog or the GitHub releases page, and
  the officially listed extensions remain ext-auth and ext-apps. No memory or
  persistent-state primitive exists as a spec section or official extension.
  The 2026-07-28 release moved the protocol core toward statelessness, which
  runs against the claim's mechanism.
- memory-2026-08-04: open, unchanged, no ledger line appended. Researched this
  run: no disclosed security incident involving unauthorised access to customer
  memory stores at Mem0, Letta, Zep, Supermemory or Engram, and no memory-layer
  component in the CISA KEV catalog. The August 2026 KEV additions were IBM
  Langflow, N-able N-central and Apache Tomcat (4 Aug) and Progress LoadMaster
  (7 Aug), none of them memory-layer components. CVE-2026-59705 (OpenMemory)
  remains catalogued in NVD without KEV listing.
- memory-2026-07-01: open, unchanged, no ledger line appended. No DPA or state
  AG action naming persistent assistant memory as its subject has surfaced
  since the 2026-08-04 pass. Resolve-by 2027-09.
- memory-2026-07-03: open, unchanged, no ledger line appended. No documented
  incident of leaked or subpoenaed assistant memory harming a named individual
  has surfaced since the 2026-08-04 pass. Resolve-by 2027-09.

Surprises:
- memory-2026-08-01 confirmed on its first grading pass, against documentation
  published seven months before the claim was logged. This is the second
  consecutive retrodiction in this theme: memory-2026-07-02 confirmed the same
  way on 2026-08-04. The 2026-08-04 sweep wrote a forward-looking claim with a
  2027-04 horizon about a control Microsoft had already shipped and documented
  in January 2026, and the sweep's own source (the MemGhost write-attack
  reporting) framed memory-write confirmation as an unmet need. The claim
  surveyed the two vendors in the news rather than the four vendors it named.
  This is direct new evidence for CAL-004 and should extend it.
- The direction of travel on memory-2026-08-03 is actively away from the claim,
  not merely short of it. MCP's 2026-07-28 release made the protocol core
  stateless and pushed durable concerns into extensions, so a memory primitive
  landing in the core spec is now less likely than when the claim was written
  on 2026-08-04, nine days earlier. A claim can decay through an architectural
  decision that predates it.
- memory-2026-08-02 is contradicted in spirit by documentation that was already
  public when it was logged. OpenAI's Memory FAQ states plainly that deleting a
  chat does not delete memories derived from it. The claim predicts a guarantee
  that one of its two named vendors currently documents the negation of, which
  makes it closer to a falsification candidate than an open forecast, and it
  survives to 2027-06 only on the Anthropic half of the disjunction.
