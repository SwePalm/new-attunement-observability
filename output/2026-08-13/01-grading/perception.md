# Signal grading, perception, 2026-08-13

Scope note: this run falls nine days after the 2026-08-04 grading pass. Every
live open claim was researched, but a grade line was appended to the ledger
only where the resolve-by month had arrived or where evidence dated after
2026-08-04 materially moved the claim. Neither condition was met for any
claim, so `ledger/perception.md` is unmodified this run. The
perception-2026-02-NN entries still listed under "Open claims" are retired
method-v1 seed claims and were not re-graded.

Scorecard:
- open: 6, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- unchanged since 2026-08-04 (not re-graded): 6
- retired method-v1 seed claims skipped: 2 (perception-2026-02-03,
  perception-2026-02-04)

Grade Details:
- perception-2026-07-01: open, unchanged. The claim turns on the 2 Dec 2026
  Article 50(2) machine-readable marking date holding without further
  deferral. The Digital Omnibus on AI signed 8 Jul 2026 deferred the high-risk
  obligations but explicitly did not touch Article 50, and the core
  transparency duties went live on 2 Aug 2026 as scheduled. The 2 Dec grace
  window for generative systems already on the market before 2 Aug 2026 stands
  unchanged, and no new deferral has been proposed in the nine-day interval.
  The operative date has not arrived. Resolve-by is 2027-01.
  (context: https://labs.cloudsecurityalliance.org/research/csa-research-note-eu-ai-act-article-50-transparency-20260729/, Jul 2026)
- perception-2026-07-03: open, unchanged. No mainstream postmortem has
  attributed a market-moving or election-affecting outcome materially to
  synthetic media. The 2026 incident record remains fraud-shaped and
  investor-targeted rather than market-moving in the claim's sense: the Bombay
  Stock Exchange CEO impersonation (Jan 2026) drew an exchange warning about
  fraudulent stock tips, and the fabricated Stanley Druckenmiller crash-forecast
  video (Feb 2026) circulated without a documented price effect. The still-cited
  benchmark for an actual index move remains the May 2023 Pentagon explosion
  hoax. The Nov 2026 US midterms are the near-term test. Resolve-by is 2027-09.
- perception-2026-08-01: open, unchanged. The Oregon Secretary of State's
  Elections Division investigation of Jonathan Lockwood, opened in Jul 2026
  after a complaint over unlabeled synthetic videos of Rep. Janelle Bynum,
  remains in progress. Coverage dated 12 Aug 2026 reports the office
  describing the investigation as ongoing; no written determination, civil
  penalty, referral, or dismissal has issued. Lockwood continues to contest
  the complaint as unconstitutional, which raises the odds the eventual
  determination is litigated rather than final. This is post-2026-08-04 but is
  a status-quo report, not material movement, so no grade line was appended.
  Resolve-by is 2027-03.
  (context: https://azcapitoltimes.com/news/2026/07/21/state-ai-deepfake-laws-face-first-big-test-in-2026-midterm-elections/, Jul 2026)
- perception-2026-08-02: open, unchanged. Article 50 became enforceable on
  2 Aug 2026 and national market surveillance authorities gained power from
  that date to accept complaints and open investigations. The Commission's
  2 Aug 2026 announcement set out the enforcement posture but named no
  provider or deployer and opened no Article 50 proceeding. Grok has drawn
  scrutiny over non-consensual deepfakes, but nothing in the record ties that
  scrutiny to a formal Article 50 marking or labelling action. The claim's
  trigger, a publicly announced first formal action against a named party, has
  not occurred. Resolve-by is 2027-06.
  (context: https://www.jurist.org/news/2026/08/european-commission-announces-ai-companies-to-face-tighter-eu-oversight-over-deepfakes-and-cyber-threats/, Aug 2026)
- perception-2026-08-03: open, unchanged. iOS 27 is still in beta. General
  release is expected in Sep 2026 alongside the iPhone 18 line, so the claim's
  triggering event is structurally unreachable before then. Beta coverage
  through 11 Aug 2026 continues to describe the rebuilt Image Playground on
  Private Cloud Compute carrying an automatic SynthID watermark on generated
  images, consistent with the 8 Jun 2026 announcement, but general release is
  the threshold and it has not happened. Resolve-by is 2027-01.
  (context: https://www.macrumors.com/2026/08/11/new-things-iphone-can-do-ios-27/, Aug 2026)
- perception-2026-08-04: open, unchanged. No platform announced a new
  friction-based treatment in the interval. The nearest existing mechanisms
  point the wrong way for this claim: TikTok, Meta, and YouTube apply
  distribution reduction and monetization penalties to creators who fail to
  disclose, and to mass-produced or duplicated content, which is enforcement
  against non-disclosure rather than friction applied to correctly labeled AI
  content. TikTok's own direction of travel since passing 1.3 billion labeled
  AI videos is toward better detection (invisible watermarking, C2PA reading),
  not toward heavier user-facing treatment. Resolve-by is 2027-06.

Surprises:
- Nine days produced zero ledger movement across six open claims, and the
  reason is structural rather than incidental. Four of the six are pinned to
  dated institutional events that cannot occur before autumn at the earliest
  (2 Dec 2026 for the EU marking runway, Sep 2026 for iOS 27 general release,
  Nov 2026 for the midterms as the deepfake test, an open Oregon investigation
  with no statutory clock). Re-grading a claim whose trigger date is months
  out cannot generate signal; it can only manufacture the appearance of work.
- perception-2026-08-04 is drifting away from what it was meant to measure.
  It was written to detect platforms moving beyond the small overlay label
  toward real friction. What actually exists is the mirror image: friction is
  being applied to creators who fail to label, not to viewers encountering
  labeled synthetic content. Every platform mechanism found in this pass sits
  on the disclosure-enforcement side of that line. As written the claim can be
  satisfied by evidence that does not demonstrate the shift it was after, so
  it is a candidate for sharper restatement rather than repeated grading.
- Against CAL-002, the EU held the Article 50 line for a second consecutive
  pass: the Digital Omnibus signed 8 Jul 2026 deferred high-risk obligations
  by more than a year while leaving Article 50 untouched, and the transparency
  duties applied on 2 Aug 2026 on schedule. Two of this theme's claims
  (perception-2026-07-01, perception-2026-08-02) now depend on that selective
  firmness, which is worth noting because CAL-002 would predict the opposite.
- CAL-004 has a clean live test forming here. perception-2026-08-02 was logged
  on 2026-08-04, two days after the Article 50 enforcement date it depends on,
  and it correctly requires a named party rather than the enforcement regime
  merely existing. That construction is what kept it open in this pass instead
  of confirming off the 2 Aug 2026 announcement, which is the retrodiction
  failure mode CAL-004 describes.
