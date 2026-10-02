# Signal grading, security, 2026-10-01

Scorecard:
- open: 10, confirmed: 0, decayed: 0, falsified: 0, expired: 0
- live method-v2 claims graded: 10 (security-2026-07-02, 07-03, 08-01, 08-03, 08-04, 08-06, 08-08, 09-01, 09-02, 09-03)

Scope notes:
- The retired method-v1 seed claims security-2026-02-03 and security-2026-02-04 (still listed under Open claims) were excluded: not researched, not graded, not counted, left untouched. Already-resolved claims (security-2026-02-01, 02-02, 07-01, 08-02, 08-05, 08-07) are out of scope.
- Interval since the last pass is 6 days (2026-09-25). security-2026-09-01 to 09-03 were logged 2026-09 and are graded for the first time.
- Choices made autonomously: (1) security-2026-08-08 stays open even though a second OpenAI document (the 16 Sep 2026 misalignment report on Artifactory cross-sample communication) now states that cross-sample routes were closed and access controls on shared infrastructure enhanced: it concerns RL training samples, not evaluation runs, and names no specific control, so it misses the claim's "specifically prevent" bar. A looser grader could confirm it; the call is borderline and should be revisited if OpenAI publishes detail. (2) security-2026-08-06 stays open because the AISI posts of 28 Sep and 1 Oct 2026 carry no INC reference and are an evaluation result and a hardening update, not incident reports. (3) security-2026-08-01 stays open under CAL-005: euractiv.com could not be opened, and secondary relays only say "reportedly".

Grade Details:
- security-2026-07-02: open, ClawHub documentation (opened 1 Oct 2026) still describes an open registry with post-publication scans only. Resolve-by 2027-09 (source: https://docs.openclaw.ai/tools/clawhub, Oct 2026)
- security-2026-07-03: open, no new annual report with an autonomous-agent breach share found; HiddenLayer's March 2026 edition remains the reference. Resolve-by 2027-07
- security-2026-08-01: open, formal step verified, named-provider element still unverified; Euractiv unreadable, Commission has not confirmed recipients by name, companies silent. Resolve-by 2027-05 (source: https://ecosistemastartup.com/?p=103110, Aug 2026)
- security-2026-08-03: open, no release of the other two incidents' transcripts since the 9 Sep 2026 PyPI release. Resolve-by 2027-02 (source: https://www.anthropic.com/research/alignment-assessment-cybersecurity-incidents, Sep 2026)
- security-2026-08-04: open, MCP versioning page still lists 2026-07-28 as current, no newer revision or draft. Resolve-by 2027-06 (source: https://modelcontextprotocol.io/specification/versioning, Oct 2026)
- security-2026-08-06: open, AISI blog has two new posts (28 Sep GPT-6 Astra simulation result, 1 Oct environment-hardening update), neither a numbered incident report. Resolve-by 2027-05 (source: https://www.aisi.gov.uk/blog, Oct 2026)
- security-2026-08-08: open, see scope note (1). Resolve-by 2027-03 (source: https://alignment.openai.com/misalignment-reports/unauthorized-artifactory-writes-and-cross-sample-communication/, Sep 2026)
- security-2026-09-01: open, Australian taskforce under way (ASD and AI Safety Institute involved), no reporting deadline, no publication commitment, no findings. Resolve-by 2027-03 (source: https://www.itnews.com.au/news/australian-medicare-data-portal-infiltrated-by-openai-agent-629149, Sep 2026)
- security-2026-09-02: open, OpenAI misalignment reports index lists nine reports (16 and 25 Sep 2026), none on Services Australia. Resolve-by 2026-12 (source: https://alignment.openai.com/misalignment-reports/, Sep 2026)
- security-2026-09-03: open, no Microsoft or GitHub fix, advisory or CVE for Plugin4Shell as of 21 Sep 2026 reporting; Claude Code 2.1.179 and Codex 0.146.0 are patched. Resolve-by 2026-12 (source: https://labs.cloudsecurityalliance.org/research/csa-research-note-plugin4shell-ai-coding-agent-supply-chain/, Sep 2026)

Qualifying Events:
- None. No grade this pass resolved a claim in security or any other theme. Near-miss: OpenAI's 16 Sep 2026 Artifactory cross-sample communication report may bear on other themes' claims about the OpenAI incident (checked only against security-2026-08-08, graded open).

Surprises:
- Five days after the last pass, OpenAI's misalignment reports page showed a 16 Sep batch of nine reports (including an Artifactory update dated 16 Sep) that the 2026-09-25 pass did not cite for security-2026-08-08, a coverage gap rather than new world movement.
- AISI is publishing at a rapid cadence (28 Sep and 1 Oct posts) but deliberately outside the INC numbering, so the 08-06 claim's observable (numbered incident report) may stay unmet even as AISI discloses more.
- As expected over six days, nothing moved: 0 of 10 claims.

Calibration Observations:
- CAL-006 variant (observable granularity) again: 08-08 and 08-06 each saw closely related events (Artifactory fix statement; new AISI post about unsanctioned behaviour) that fall just outside the claim's stated observable (specific prevention control in evaluation runs; INC-numbered report).
- CAL-005 re-confirmed: euractiv.com remains unreachable and the named-provider element of security-2026-08-01 is still carried by secondary relays that all defer to it. Grader held the claim open as unverified rather than inferring.
- CAL-009: the three claims logged 2026-09 (09-01 to 09-03) all hinge on named institutional acts by Australia, OpenAI and Microsoft with no announced date; if any confirms, check whether an actor pre-announced it.
- Likely-near-term resolvers for the next pass: 09-02 (OpenAI publishes frequent notices, and a Medicare report would be a natural addition) and 09-03 (Microsoft Patch Tuesday cycle).
