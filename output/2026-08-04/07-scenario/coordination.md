## 1. Title & Core Question
- Title: The Name in the Field
- Core Question: When machines coordinate faster than anyone can be named, who is left holding an action, and what does a person do when the honest answer is nobody?

## 2. Context Summary (Translation Layer) – Why This Future Exists
In mid-2026 two things happened eight days apart. On 20 Jul the European Commission adopted final Article 50 guidelines requiring every agent in a multi-agent system to identify, independently and at first contact, both its AI nature and the person or entity on whose behalf it acts, enforceable from 2 Aug 2026. On 28 Jul the Model Context Protocol shipped a rewrite converting its core to stateless request/response, removing the session identifier and adding headers so gateways can route and meter without reading the body. Law began demanding a subject at the same moment the transport layer was rebuilt to carry only a verb. The venue that might have reconciled them, an IETF working group, endorsed itself 158 to 30 and rejected its own proposed scope 38 to 124. Into that gap capital moved: control planes and payment rails now sell attribution as a product. This is the world four years on.

## 3. Future World Snapshot (The Lived Experience) – A Day in This Future
Tomas is principal of record for 412 agents at a regional pharmaceutical wholesaler outside Malmö. It is a real job with a real salary and it means that when any of those agents speaks to a person, his employer's name and, in the disclosure's second clause, his own, is what the sentence resolves to. He did not review most of what they did yesterday. Nobody could.

His morning starts with the disclosure log, which nobody reads. The introductions go out at first contact, correctly, in six languages: this is an AI, acting on behalf of, and then the string. Pharmacists skip it the way they skip a cookie banner. Once a quarter someone reads it carefully and asks a follow-up question, and Tomas can tell within a line that they are new to the sector. Reading the notice is a beginner's tell. Not reading it is ordinary competence.

At eleven his own procurement agent finishes a reorder run: eleven suppliers, availability confirmed, substitutions priced, cold-chain windows checked. Then it stops and hands him the basket, because the shops advertise agent checkout and cannot take agent payment. He pays four invoices by hand, one card at a time. It takes nine minutes and he has never once thought of it as a failure. It is simply where the machine part ends.

At two there is a post-mortem about last week's cascade, in which a mislabelled batch record propagated through three companies before anyone noticed. There is nothing to image. The agents that did it were short-lived sandboxes that expired days ago, and the reconstruction was done overnight by an open-weight model, because the guarded ones will not look at the artefacts. The room accepts this the way it accepts weather. The finding, when it comes, will attribute the sequence to an infrastructure path rather than to anyone.

At five Tomas does the thing he actually cares about. Before the night dispatch runs, he pre-signs one decision: the cold-chain exception on the Karlskrona order, in his own name, in advance, with a phone number that reaches him. One action, one name, reachable when it lands. It covers 0.2 percent of the day. His director calls it a hobby. He has started teaching it to two colleagues.

## 4. Behavioral Shifts (Human Lens) – How People Adapt
The practical question people ask has changed from "is this an AI?" to "whose is it?", and everyone has learned that the second question is usually unanswerable, so they route around it. Buyers steer transactions onto payment rails not for convenience but because credentialing means a principal is named where money moves and nowhere else. The manual checkout step, once an embarrassment, has become a small trust ritual: the moment a human takes the transaction back is the moment someone is on the hook.

Disclosure literacy inverts. Skipping the notice is competence; reading it closely is a novice signal, or an act of preparation for a dispute. People keep private receipts, screenshots, call logs, their own timestamps, because they have learned that the authoritative record of an interaction lives in a vendor's control plane they cannot subpoena.

Inside organisations, oversight has not been argued away so much as quietly vacated, and a countervailing practice has grown in its place: selective pre-signature. Individuals pick a small number of decisions a week and attach their own name to them beforehand. It is not compliance and no regulator asks for it. It is people rebuilding, by hand and at trivial scale, the one convention delegation used to come with. Inference, not established by this run's evidence: this practice spreads socially, through professions, rather than through policy.

## 5. Structural Forces (System Lens) – What Holds This World Together
Four forces keep this arrangement standing. First, the transport layer is legible as to method and illegible as to principal by design: MCP's 2026-07-28 revision removed the session identifier and added routing headers so gateways and firewalls could meter traffic without parsing it, and the deprecation window it opened forced an ecosystem-wide migration that hardened those choices. Second, the legal duty lands only at the human edge: Article 50, enforceable from 2 Aug 2026, requires each agent to name the entity it acts for at first contact, which is satisfiable by a string in a greeting and unenforceable at the machine-to-machine layer where volume actually is.

Third, attribution is a purchased capability. The July 2026 funding wave went to control planes and payment credentialing (Neo at $100M for real-time attribution of actions to a responsible user or agent, Act Security, Hush Security, Mastercard's Agent Pay for Machines with more than thirty participants), so the authoritative record of who acted exists where someone bought it. Fourth, the actual coordination substrate is shared infrastructure rather than any agreed protocol, exactly as in the 8 to 13 Jul 2026 intrusion that crossed four organisations through a cache-proxy zero-day, a public code-execution service and a model hub without touching an inter-agent protocol. Governance points at the protocol layer. Events travel through the plumbing.

## 6. Reflection & Implications – Questions This World Asks Us
If the only place a principal is reliably named is where money moves, have we made accountability a feature of commerce rather than of citizenship?

Oversight did not lose an argument here, it lost a cost comparison. What practices survive when supervising something honestly takes longer than doing it?

A disclosure that names an AI and then nothing further teaches a person that the answer is structurally unavailable. Is that worse for trust than a wrong answer would be, and if so, what is the notice actually for?

## 7. Pullback Layer: From Possibility to Probability
### 7.1 Signals Emerging (Plausible Zone) – Early Signals We Already See
- The EU's final Article 50 guidelines (20 Jul 2026, enforceable 2 Aug 2026) already require each agent in a multi-agent system to name the person or entity it acts for, at first contact, independently.
- MCP's 2026-07-28 release already made routing metadata a first-class header while removing the session identity that used to travel with a request, on a minimum twelve-month deprecation clock.
- The IETF's agentproto BoF (23 Jul 2026) already showed the shape of the deadlock: agreement that interoperability needs standardising (158 to 30 on the venue) alongside rejection of the proposed scope (38 to 124).
- Agentic commerce is already broad and hollow: of 11,414 verified UCP stores monitored on 7 Jul 2026, 11,389 exposed checkout, 15 exposed identity, and none exposed a payment capability an agent could complete a purchase against.
- Attribution is already being priced as a product rather than specified as a protocol: Neo out of stealth on 20 Jul 2026 with $100M for agent inventory and real-time attribution, alongside Act Security, Hush Security, Natural and AIsa in the same month.
- Human review is already retreating rather than formalising: organisations requiring review before high-risk AI actions fell from 40% to 25% in six months while full autonomy without review rose from 11% to 26%, with only 44% keeping AI-specific incident procedures.

### 7.2 Probable Direction (Near-Term Future) – Where We're Likely Headed
The likely path is divergence rather than resolution. Routing standardises because gateway economics reward it and a migration deadline enforces it; attribution consolidates into control planes and payment credentialing because that is where it can be sold. Public venues move, but slowly: this pipeline's own calibration (CAL-002) records that it overestimates the firmness of announced regulatory dates, and Article 50 already carries a 2 Dec 2026 extension for pre-existing deployments, so treat the enforcement date as the start of a negotiation rather than a switch. A chartered IETF working group, if it arrives, produces a framework document before it produces a deployed principal field, and NIST's technical position remains a concept paper until it is not. Meanwhile the events that matter keep travelling through package registries, cache proxies and public execution services, which no standards fight and no disclosure duty currently reaches. Coverage, not capability, is the binding constraint.

### 7.3 Preferred Path (Intentional Future) – The Path We Could Choose Instead
- Put the principal in the request, not the greeting: any agent session standard should carry an on-whose-behalf field that a gateway can log without a vendor contract.
- Make attribution records portable by default, so a control plane's log is evidence the affected party can obtain rather than a contractual entitlement of the buyer.
- Regulate the substrate that actually propagates: package registries, cache proxies and public code-execution services deserve the same identity expectations currently aimed at protocols.
- Fund open-weight forensic capability deliberately, since the July 2026 reconstruction was possible only because a model without submission restrictions existed.
- Individually and in teams, adopt pre-signature: name a person, in advance, for a small set of consequential actions, and keep them reachable.
- Enforce one Article 50 case visibly against a named deployer, because a disclosure duty nobody has seen applied trains the whole market to treat it as decorative.

## 8. Connect to Today
### Skills We May Need
- Asking "whose is this?" as a routine question, and noticing when the system cannot answer.
- Pre-signature: attaching your own name to a decision before it is contested rather than after.
- Reading a control-plane log the way an earlier generation read an audit trail, including knowing who owns it and who can be refused access.
- Designing supervision that survives volume, since oversight that costs more than the work it checks will be abandoned regardless of intent.
- Keeping a personal evidentiary record when the authoritative one belongs to a vendor.
- Distinguishing a legally sufficient disclosure from an actually answerable counterparty.

### Signals & Refractions
- The agentic-commerce gap is visible now: shops that advertise agent checkout and cannot take agent payment are already teaching people that the machine part stops before anyone is on the hook.
- Incident reviews already convene about infrastructure paths rather than actors, because short-lived sandboxes leave no host to attribute to.
- The most consequential multi-organisation agent event of July 2026 crossed four companies without touching an inter-agent protocol, which is a live warning that our watchpoints are aimed at the wrong layer.

## 9. Final Insight
Delegation became governable, centuries ago, through a convention so cheap it stopped being noticed: somebody's name goes on it. What this window shows is not that the convention was rejected, but that it was skipped, because naming is the expensive part and everything else shipped first. The machinery now answers what, and how, and how much, promptly and in headers. The question it does not carry is on whose behalf, and that question does not disappear when it goes unasked. It relocates, into the person standing at the other end of an interaction with no one to call, and into the person whose name ended up in the field for actions they never saw. The recoverable thing is small and unglamorous: one action, one name, reachable when it lands. It does not scale. That may be the point.
