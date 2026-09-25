# PESTLE, identity, 2026-09-25

### Political
Core Shift Thesis:
States are hardening identity for the agents they run and for the humans they
serve, but not for the outside agents that visit them, so the political gap
over the next two years is ownership of the public front door rather than the
back office.

Forces:
1. Inward agent-identity mandates for government estates. Australia's ISM
   September 2026 release (4 Sep 2026) adds ISM-2133 to ISM-2135 (a unique
   identity per AI agent and an agent register with owner, purpose, credentials
   and tools) and ISM-2156 to ISM-2159 (task-scoped tool authorisation and
   logging), binding on agencies at IRAP reassessment within 24 months, with no
   control addressed to agents arriving from outside (sweep, Confirmed
   Developments and Regulatory Shifts, Sep 2026).
2. Incident-led political attention on outside agents at public portals. The
   Medicare Statistics Reporting Portal incident (OpenAI agent, 18 Jun 2026,
   disclosed 23 to 24 Sep 2026) produced a prime-ministerial taskforce and
   reported urgent ASD authentication guidance to agencies, but no published
   requirement that visiting agents identify themselves (sweep, Confirmed
   Developments and Emerging Signals, Sep 2026; tracked by ledger claim
   identity-2026-09-03, open).
3. National wallets as state identity infrastructure launched late and in
   stages. Germany's BMDS set d-you for 2 Jan 2027, after the end-2026 eIDAS
   deadline, with about 40 partners including the Bundesagentur fuer Arbeit,
   Deutsche Post and the Sparkassen association; a 2 Sep 2026 tracker found no
   member state with a live production EUDI wallet (sweep, Delta and Confirmed
   Developments, Sep 2026).
4. Age as a political identity axis. The Commission's EU KIDS Act proposal (17
   Sep 2026) would oblige social media, AI companions, general chatbots, games
   and app stores to verify age at account opening through the EU age
   verification tool or another public-authority solution, extending mandatory
   identity checks to the entry point of AI products themselves (sweep,
   Regulatory Shifts, Sep 2026).

### Economic
Core Shift Thesis:
Capital is flowing to identity for agents sold to banks and enterprises and to
authenticity checks for human voices and faces, so the paying customer shapes
which identity questions get answered, and the ordinary person is a payer of
checks rather than a buyer of them.

Forces:
1. Know Your Agent as a bank-facing product line. Baselayer's $35 million
   Series A (22 Sep 2026, M13 lead) funds an Agentic Identity Suite issuing
   credentials agents present during transactions to prove delegated authority,
   sold into a base of more than 2,000 US financial institutions (sweep,
   Capital Movements and Emerging Signals, Sep 2026).
2. Vendor coalitions as the market structure for agent identity. The Blueprint
   Alliance (Okta plus AWS, CrowdStrike, Databricks, Docker, Google Cloud,
   Lovable, Proofpoint, Salesforce, ServiceNow, Wiz, Zscaler, 22 Sep 2026) sets a
   shared reference architecture that treats agents as identities, with
   Microsoft outside it, so interoperability arrives as ecosystem membership
   (sweep, Confirmed Developments, Sep 2026; ledger claim identity-2026-09-01).
3. Deepfake detection absorbed into professional-services fraud offerings.
   KPMG LLP's minority stake in Reality Defender (Sep 2026) embeds real-time
   voice and video authenticity checks into audit-firm fraud and cyber services,
   which makes stacked human verification a billable layer rather than a bank's
   internal choice (sweep, Capital Movements, Sep 2026).
4. Stacking rather than replacement as the bank cost model. Banks are adding
   behavioural, device, liveness and transaction-context checks on top of voice
   rather than retiring it, so verification cost per human interaction rises
   while the legacy channel stays open (grading file, identity-2026-07-01 graded
   open 2026-09-25, source infosecfederation.com, Aug 2026).

### Social
Core Shift Thesis:
Everyday life acquires more identity checkpoints per week while the places
where people are recognised without a check thin out, and the burden of the
checks falls hardest on people with limited devices, changed faces or voices,
or responsibility for someone else.

Forces:
1. Digital proof of age moves to the till. SI 2026/1022 (in force 15 Sep 2026)
   lets licensed premises in England and Wales accept DVS-certified digital ID
   for alcohol age checks, but supermarket groups and pub companies were still
   taking advice and no large retailer had named a rollout date (sweep,
   Regulatory Shifts and Emerging Signals, Sep 2026; ledger claim
   identity-2026-09-02, open).
2. The launch-reach gap in wallet adoption. Malawi's Nzika wallet launched on
   16 Sep 2026 with over 22,000 sign-ups against 99 percent physical ID
   coverage, 33 percent smartphone ownership and 12.5 percent basic internet
   skills; the government abolished card expiry dates the same day, keeping the
   physical card as the durable credential (sweep, Confirmed Developments and
   Counter-Signals, Sep 2026).
3. Device-bound credentials as a household coordination problem. d-you stores
   credentials encrypted on the device only, and OpenID Connect Key Binding
   (approved as Implementer's Draft 10 Sep 2026) ties tokens to the holding
   device, so acting for a family member increasingly means physical access to
   their phone rather than a delegable permission (sweep, Confirmed
   Developments, Sep 2026; grading file, identity-2026-08-05).
4. Proof-of-human badges normalised on consumer platforms. World ID's
   verified-human badges run in production at Tinder, Zoom and Docusign (ledger,
   identity-2026-07-02 confirmed 2026-08-04, source world.org, Apr 2026, drawn
   from the ledger rather than this run's sweep).

### Technological
Core Shift Thesis:
The technical primitives for binding identity to devices, tokens and verifiable
presentations are maturing fast, but they are being assembled for enterprise
estates and human wallets, and the assembly that would let a stranger's agent
prove a person's mandate is not yet being built by anyone in the record.

Forces:
1. Token binding and short-lived credentials as the baseline. NIST IR 8587
   (finalised 15 Sep 2026) addresses forged and stolen tokens with explicit AI
   agent identity considerations and points to the OIDF Shared Signals
   Framework and CAEP; ISM-2141 to ISM-2147 require short-lived, centrally
   managed workload credentials and device-bound tokens (sweep, Confirmed
   Developments, Sep 2026).
2. Wallet-grade credential exchange reaching certification. OIDF announced the
   first fourteen organisations self-certified to OpenID4VP and OpenID4VCI with
   HAIP on 24 Sep 2026, the first certification cohort for EUDI-grade exchange
   (sweep, Technical Changes, Sep 2026; grading file, identity-2026-08-07).
3. Post-quantum migration as an unplanned drag on federation. An OIDF post of
   17 Sep 2026 reports ML-DSA-44 signatures (2,420 bytes) break cookie-size
   assumptions, JWT libraries fail on unknown AKP key types, and OpenID Connect
   allows one signing algorithm per relying party; Czech MojeID shipped
   post-quantum key exchange in September (sweep, Emerging Signals and Technical
   Changes, Sep 2026).
4. Interoperability profiles slipping at the edges. The OIDF CAEP
   Interoperability Profile vote scheduled for 26 Sep to 10 Oct 2026 was pushed
   back when the working group restarted review, and Okta Agent Gateway remained
   pre-GA on 22 Sep 2026 (sweep, Delta and Confirmed Developments, Sep 2026;
   grading file, identity-2026-08-03).

### Legal
Core Shift Thesis:
Law is making identity checks lawful and mandatory for humans at specific
points of access while leaving an agent's authority to act for a person to
contract and vendor terms, so legal certainty grows on one side of the
transaction only.

Forces:
1. Statutory permission for digital age proof tied to a certification scheme.
   SI 2026/1022 admits only providers certified under the DVS trust framework
   overseen by OfDIA, which makes the certification body, not the retailer, the
   gatekeeper of which credentials count (sweep, Regulatory Shifts, Sep 2026).
2. Mandatory age verification proposed for AI products at account opening. The
   EU KIDS Act proposal (17 Sep 2026) bars independent accounts under 13 and
   requires supervised accounts from 13 to 15, using a public-authority
   verification route; as a proposal it faces the ordinary legislative calendar
   (sweep, Regulatory Shifts, Sep 2026).
3. Compliance baselines applied at reassessment rather than immediately. IRAP
   systems must meet the September 2026 ISM at reassessment within 24 months
   and existing authorisations remain valid, so agent-identity controls phase in
   across 2027 and 2028 rather than at publication (sweep, Regulatory Shifts,
   Sep 2026).
4. Delegated agent authority defined by vendor credentials and terms. The only
   delegated-authority instruments in the record are commercial: Baselayer's
   credentials for agents in transactions and the Blueprint Alliance's
   cross-vendor integrations on MCP, OCSF, SSF and CAEP; no statute in the sweep
   defines when an agent may act as or for a person at a relying party (sweep,
   Capital Movements and Confirmed Developments, Sep 2026).

### Environmental
Core Shift Thesis:
Identity's environmental footprint is less about energy than about physical
infrastructure: phones, cards, counters and capacity, and the shift to
device-bound credentials makes identity depend on hardware lifecycles and peak
loads that differ sharply across places.

Forces:
1. Device dependency and hardware replacement cycles. Device-only credential
   storage (d-you) and device-bound tokens (ISM-2147, Key Binding) tie identity
   to a working, current phone, so identity continuity follows handset
   replacement, loss and battery life (sweep, Confirmed Developments, Sep 2026).
2. The durable physical card as the low-resource fallback. Malawi abolished
   expiry dates on biometric national ID cards as its wallet launched, keeping a
   no-energy, no-connectivity credential valid indefinitely where only a third of
   the population owns a smartphone (sweep, Confirmed Developments and
   Counter-Signals, Sep 2026).
3. Peak-load capacity as an identity risk. The Czech DIA's public eDoklady
   stress test (13 Aug 2026) drew about 30,000 users; the system held with
   longer response times, and the follow-up analysis named slow Application
   Gateway scaling and committed to added capacity before elections (grading
   file and ledger, identity-2026-08-06, source dia.gov.cz, Aug 2026, drawn from
   grading rather than this run's sweep).
4. Heavier signatures in constrained environments. Post-quantum signatures of
   2,420 bytes break cookie and header size assumptions, which raises payload
   and compute demands on every federated login and falls hardest on older
   devices and thin networks (sweep, Emerging Signals, Sep 2026).
