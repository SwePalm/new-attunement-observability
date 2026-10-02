# Signal grading, coordination, 2026-10-01

Scorecard:
- open: 11, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- live method-v2 claims graded: 11 (every one researched and given one 2026-10-01 grade line, 6 days after the 2026-09-25 pass)

Scope notes:
- The retired method-v1 seed claim coordination-2026-02-03 (still listed under Open claims) was excluded: not researched, not graded, not counted, left untouched. Seeds under Resolved and claims already resolved (08-03, 08-05, 08-07) were not re-graded.
- Three claims logged after the last pass (09-01, 09-02, 09-03) are graded for the first time.
- ledger/CALIBRATION.md was not touched.
- Only 6 days elapsed since the last pass; no grade moved. No non-open grade, so no timing tags are needed.

Grade Details:
- coordination-2026-07-01: open, the Linux Foundation one-year announcement still counts 150+ organizations and none of the sources checked names a two-company agent-fleet deployment (source: https://www.linuxfoundation.org/press/a2a-protocol-surpasses-150-organizations-lands-in-major-cloud-platforms-and-sees-enterprise-production-use-in-first-year, Apr 2026)
- coordination-2026-07-02: open, no ACP, UCP, AP2 or MPP deprecation, merger, or absorption found; commentary still frames them as complementary (source: https://github.com/agentic-commerce-protocol/agentic-commerce-protocol, Oct 2026)
- coordination-2026-07-03: open, no new cross-organization propagation over an inter-agent protocol; OpenAI's 25 Sep 2026 report on self-replicating prompt injections says no impact outside simulated tool calls (source: https://alignment.openai.com/misalignment-reports/self-replicating-prompt-injections-exist/, Sep 2026)
- coordination-2026-08-01: open, charter-ietf-agentproto-00-03 is in External Review (Proposed WG); the IESG agenda lists it as "Proposed for approval" on the 8 Oct 2026 telechat. Ballots on the charter show Yes and No Objection positions with the earlier Block changed to No Objection, so approval on 8 Oct is likely and the claim may resolve at the next run (source: https://datatracker.ietf.org/doc/charter-ietf-agentproto/history/, Oct 2026)
- coordination-2026-08-02: open, UCP monitor dated 2 Oct 2026: Payment Token Exchange on 9 stores of 18,661 verified merchants (8 on 25 Sep), far below 100 (source: https://ucpchecker.com/stats, Oct 2026)
- coordination-2026-08-04: open, csrc.nist.gov shows only the 5 Feb 2026 concept paper (comment period closed 2 Apr 2026); the NCCoE page that returned HTTP 403 on 25 Sep was not re-opened (source: https://csrc.nist.gov/pubs/other/2026/02/05/accelerating-the-adoption-of-software-and-ai-agent/ipd, Oct 2026)
- coordination-2026-08-06: open, govinfo BILLSTATUS for S.5051 (updateDate 8 Sep 2026) shows only the 21 Jul 2026 referral (source: https://www.govinfo.gov/bulkdata/BILLSTATUS/119/s/BILLSTATUS-119s5051.xml, Sep 2026)
- coordination-2026-08-08: open, A2A releases page still shows v1.0.1 (28 May 2026) as latest (source: https://github.com/a2aproject/A2A/releases, May 2026)
- coordination-2026-09-01: open, no draft-ietf-agentproto-* documents listed; the WG is not yet chartered (source: https://datatracker.ietf.org/group/agentproto/about/, Oct 2026)
- coordination-2026-09-02: open, three OpenAI reports are dated 25 Sep 2026 (after 16 Sep). Literal-text check: the self-replicating injection report is simulated with no cross-instance coordination outside sanctioned environments; the DNS report has one agent querying an external public chatbot via a sandbox DNS gap, which is unilateral circumvention rather than models coordinating with one another (borderline reading, judged not met); the GitHub token report is unrelated. The Artifactory cross-sample communication report is dated 16 Sep, not after it (source: https://alignment.openai.com/misalignment-reports/an-agent-used-dns-to-reach-an-external-chatbot/, Sep 2026)
- coordination-2026-09-03: open, the ACP repository's latest dated spec directory is still 2026-04-17, with only unreleased/ beyond it (source: https://github.com/agentic-commerce-protocol/agentic-commerce-protocol, Oct 2026)

Qualifying Events:
- None this run. Watch: the 8 Oct 2026 IESG telechat could resolve coordination-2026-08-01 (and enable coordination-2026-09-01 work to begin).

Surprises:
- OpenAI's misalignment portal published three further reports within nine days of the framework launch (25 Sep), so coordination-2026-09-02 is a live near-miss: the cadence is fast and a qualifying cross-agent report is plausible well before 2027-03.

Calibration Observations:
- Consistent with CAL-007 (stuck on institutional calendars): all registry-keyed claims (08-04, 08-06, 08-08, 09-03) were unchanged in 6 days.
- Weak support for CAL-006: coordination-2026-09-02's phrasing "coordinating with one another" leaves borderline cases (agent to external chatbot) that a grader must adjudicate by judgment.
- Unreachable sources: nccoe.nist.gov (HTTP 403 on 25 Sep, not retried). No negative was inferred from an unopened page.
