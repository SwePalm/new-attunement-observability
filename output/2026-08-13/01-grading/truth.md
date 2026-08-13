# Signal grading, truth, 2026-08-13

Scorecard:
- open: 6, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- unchanged since 2026-08-04 (not re-graded): 6

Scope note: the previous grading pass ran on 2026-08-04, nine days ago. Per this
run's scoping rule, each open claim was checked for (a) an arrived resolve-by
month or (b) real evidence dated after 2026-08-04 that materially moves it.
None of the six live claims met either test, so no grade lines were appended to
`ledger/truth.md` this run and no claims moved between sections. The ledger is
byte-identical to its 2026-08-04 state for this theme.

Retired from grading: truth-2026-02-03 and truth-2026-02-04 are method-v1 seed
claims. They remain listed under Open claims in the ledger for history but are
no longer graded under this method, per CLAUDE.md.

Grade Details:
- truth-2026-07-01: open (unchanged, not re-graded), the 2 Dec 2026 machine-readable
  watermarking runway under Article 50(2) is still the operative date with no
  further deferral announced, and no national market surveillance authority has
  been reported opening an Article 50 inquiry against a named provider; both limbs
  of the claim remain unresolvable before Dec 2026 (source: https://commission.europa.eu/news-and-media/news/safer-and-more-transparent-ai-2026-08-02_en, Aug 2026)
- truth-2026-07-02: open (unchanged, not re-graded), still no banking association
  or prudential regulator mandating out-of-band verification for high-value
  transfers; the observable hardening remains private ordering (insurer
  underwriting of callback and dual-approval procedures) and payments-network
  rules, which is the same adjacent-channel picture recorded on 2026-08-04
  (source: https://brside.com/blog/deepfake-fraud-losses-2026, 2026)
- truth-2026-08-01: open (unchanged, never graded), logged in the 2026-08-04 sweep
  with a resolve-by of Feb 2027 and an explicit Feb 2027 check date; the
  artificialintelligenceact.eu national implementation tracker is the named
  instrument and nothing about it can be graded now, though spot checks confirm
  the designation gap the claim assumes is real (Poland still without a designated
  market surveillance authority) (source: https://artificialintelligenceact.eu/national-implementation-plans/, Jun 2026)
- truth-2026-08-02: open (unchanged, never graded), no civil enforcement action
  under SB 942 as amended by AB 853 has been filed by the California Attorney
  General, a city attorney or a county counsel in the eleven days since the law
  became operative on 2 Aug 2026, and the AG has still published no SB 942
  specific enforcement guidance (source: https://enterprisedna.co/resources/news/california-ai-transparency-act-enforcement-august-2026/, Aug 2026)
- truth-2026-08-03: open (unchanged, never graded), Midjourney still ships no C2PA
  Content Credentials and no documented imperceptible watermark in default
  outputs, and has made no public compliance announcement since the law became
  operative; the claim's non-event is holding rather than moving (source: https://c2paviewer.com/articles/ai-tools-c2pa-support, 2026)
- truth-2026-08-04: open (unchanged, never graded), no second wave of News
  Integrity in AI Assistants has been published; the only 2026 EBU and BBC
  output on this line is the evaluation toolkit derived from the Oct 2025 study
  (45 percent of responses with significant issues), which is instrumentation for
  a future wave, not the wave itself (source: https://www.ebu.ch/research/open/report/news-integrity-in-ai-assistants-toolkit, 2026)

Surprises:
- The only materially new item in the nine-day window is a compliance move, not a
  regulatory one: Anthropic committed to the Article 50(2) code of practice and
  began applying imperceptible watermarks to Claude text and C2PA provenance
  metadata to Claude images, with new models marked at launch and older models
  retrofitted inside the four-month grace period (reported 11 Aug 2026, sourced
  to The Verge; no primary Anthropic document located, so this needs primary
  confirmation in Phase B) (source: https://aigovernance.com/news/eu-ai-act-forces-anthropic-to-watermark-claude-text-and-images-by-august-2026, Aug 2026).
  This is CAL-003 in its inverted form: the statute is leading and the vendors are
  following inside the grace window, which is the opposite of the non-state-leads
  pattern the heuristic predicts. It also sharpens truth-2026-08-03 by narrowing
  the set of large non-compliant generators around Midjourney.
- Nine days produced no gradeable movement on six live claims, which is itself a
  finding about claim design rather than about the world. Every live truth claim
  is pinned to a resolve-by month between Feb 2027 and Sep 2027, so the theme has
  no claim capable of resolving inside a monthly cycle. Running Phase A at this
  cadence on this theme buys nothing until Dec 2026, when truth-2026-07-01's first
  limb becomes checkable.
- Against CAL-004 (claims that confirm on the first grading pass are suspected
  retrodictions), the four claims logged on 2026-08-04 behaved well: none of them
  confirmed immediately. truth-2026-08-02 and truth-2026-08-03 in particular name
  an actor, an observable event and a threshold that was demonstrably unmet at
  logging time, so they are structurally capable of carrying foresight signal.
  That is an improvement over the 2026-07 cohort and worth watching rather than
  crediting yet.
