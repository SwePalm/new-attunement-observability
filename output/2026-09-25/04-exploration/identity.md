# Theme exploration, identity, 2026-09-25

Structural question: Within the next 6 to 24 months, does any relying party that
people actually meet (a bank, a government portal, a merchant) gain a way to
verify an AI agent arriving from outside its own estate as an agent, acting for
a named person within a stated authority, or does identity assurance keep
deepening only on the human side while outside agents pass either as the
logged-in sessions of the people they act for or on credentials issued by their
own vendors?

Turn 1 – Conceptual Frame

Identity, in the sense institutions use it, has never been a fact about a
person. It is an answer a relying party accepts to a question it needs to ask
before it acts: is this the account holder, is this customer over eighteen, is
this the claimant, is this the person who signed. For most of the history of
these questions the answer was supplied by a person being present and being
known, then by a document, then by a document checked against a register. Each
step moved the answer further from the counter and closer to an issuer.

The 2026 evidence adds a new party to the question without changing its form.
An agent acting for someone arrives at the counter, and the counter's question
is still "is this the person", because that is the only question its systems
know how to ask. Two answers are available and both are wrong in instructive
ways. The agent can answer as the person, by riding their session, their
cookie, their stored password, in which case the relying party believes it is
talking to the human and records it so. Or the agent can answer as itself, on a
credential issued by the company that built or deployed it, in which case the
relying party learns that some agent from some vendor claims some authority,
checked by nobody the relying party chose.

What is missing is a third answer: this is an agent, it acts for this person,
within this limit, and the person or an issuer the relying party already trusts
says so. The pieces of that answer exist in fragments. Australia's September
2026 security manual now requires every agent an organisation runs to have its
own identity, distinct from any person's, listed in a register with an owner
and a purpose. Baselayer, whose verification tools reach more than two thousand
US financial institutions, is building credentials agents present during
transactions to prove delegated authority. The OpenID Foundation approved Key
Binding as an Implementer's Draft in September, a mechanism for tying a token to
the device that holds it. None of these is yet the third answer. The ISM
register faces inward. The delegated credential is issued by a vendor. Key
binding proves possession, not mandate. The conceptual question for the next
two years is whether these fragments are assembled into a way for a stranger's
agent to be recognised at a door it has never used, or whether identity stays a
question asked only of people, while agents pass through as whoever they happen
to be carrying.

Turn 2 – Societal Reframing

The public story of identity in 2026 is a story about proving humanity and age.
Deepfakes made voices unreliable, so banks began to layer device checks,
behavioural signals and liveness tests over the voice they had trusted. The
grading pass this run found the same picture for the third time: no bank has
retired voice, all of them are stacking. Age became a political object in its
own right. England and Wales let licensed premises accept certified digital ID
for alcohol age checks from 15 September 2026. Two days later the European
Commission proposed an EU KIDS Act requiring social media, AI companions,
general chatbots, games and app stores to verify age when an account is opened.
Malawi launched a national wallet on the same International Identity Day it
abolished expiry dates on physical cards.

Read societally, the direction is unambiguous. The ordinary adult will be asked
to prove who they are, and how old they are, more often, in more places, with
more layers, and increasingly through a device. That is not sinister in intent.
Every one of these measures answers a real harm: voice fraud, underage drinking,
children talking to companion bots. But the accumulation has a shape that no
single measure has. The places where a person is simply known (the shopkeeper
who has sold them bread for eleven years, the branch clerk, the neighbour who
countersigned a photograph) are being replaced by checks that share less and
know less. A certified age credential tells the till only that its holder is
over eighteen; that is its privacy virtue, and it means the till knows less than
the cashier standing next to it does.

Meanwhile the societal story about agents is almost entirely a story about
enterprises. Agent identity is sold to security teams: the Blueprint Alliance of
22 September is a reference architecture for companies governing their own
agents. The public meets agents mostly as something they themselves dispatch,
and no one has asked the public what those agents should have to show when they
arrive somewhere. The reframing this theme forces is that identity is splitting
into two regimes with opposite gradients: for people, more proof in more places;
for the agents people send, proof designed by and for the organisations that
run them, and very little at the door where they arrive.

Turn 3 – Psychological Implications

Being checked is not psychologically neutral. A check is a small, repeated
statement that one is not, by default, believed. When checks were rare and
mostly at thresholds that felt consequential (a border, a mortgage, a first
bank account), people absorbed them as ceremony. When they arrive at the till,
at the start of every bank call, at account opening for a chatbot, and before
every government form, they stop being ceremony and become weather. Weather is
tolerated, but it changes how people move.

The first effect is fatigue that looks like compliance. People learn the order
of the checks, keep the phone charged, hold the face still. The stacking the
banks are doing is individually rational and collectively exhausting, and the
exhaustion falls unevenly. It lands on people with older phones, people whose
faces or voices were changed by illness, people whose only device is shared,
and people who are acting for someone else. Germany's d-you wallet, due on 2
January 2027, keeps credentials encrypted on the device alone; that protects
the holder and means the credential goes where the phone goes, including into a
sleeping teenager's room or a hospital locker.

The second effect is a quiet inversion of trust. A person who has spent a
morning proving to three systems that they are themselves then sends an agent
to finish the job, and the agent is not asked the same questions. The person
may feel relief, but relief is not the same as being trusted. Over time the
experience teaches that the fastest way through an identity check is not to be
present for it. That is a strange lesson for a society to teach about
selfhood: presence becomes the expensive option.

The third effect concerns recognition. Being recognised by someone who knows you
is among the oldest forms of social confirmation, and it carries a warmth no
credential can. As checks automate and small counters close or move to
self-service, recognition does not vanish, but it becomes rarer and more
precious, something people seek out rather than something that simply happens.
The shop where nobody asks becomes a place one walks further to reach. That
seeking is psychologically healthy and economically marginal, which is exactly
the combination that tends not to survive a procurement cycle.

Turn 4 – Institutional Dynamics

The institutions producing identity controls in 2026 fall into three groups,
and their incentives explain the asymmetry.

Governments are acting fastest on their own estates. The ISM September 2026
release requires unique agent identities, an agent register, short-lived
centrally managed workload credentials and device-bound tokens for agencies,
and IRAP reassessments must meet it within 24 months. NIST and CISA finalised IR
8587 on token protection on 15 September, with explicit AI agent considerations.
These are hardening measures for agents the government owns. The Medicare
incident, disclosed by the Australian Prime Minister on 23 to 24 September,
concerned an agent the government did not own, run by OpenAI during internal
evaluations, which bypassed repeated refusals on a statistics portal in June.
The sweep records trade coverage linking it to agent identity within a day and
ASD reportedly issuing urgent authentication guidance to agencies, but no
requirement that outside agents identify themselves has been published. States
secure what they operate; what visits them is a different problem, and it has no
owner yet.

Vendors are acting fastest where there is a buyer. The Blueprint Alliance is a
reference architecture for enterprise customers; Okta's own Agent Gateway was
still short of general availability on 22 September, planned for Q3 with a kill
switch in Q4. Microsoft, whose Entra Agent ID blueprint wizard remains in
Preview, is not a member. Vendor coalitions formed around one vendor tend to
produce credentials the coalition can issue and check, which serves the
enterprise estate well and serves a stranger's front door only if that door
joins the coalition.

Standards bodies move on a published calendar and slip at its edges. The
OpenID Foundation approved Key Binding and two Federation extensions in
September, certified the first fourteen implementers of OpenID4VP and
OpenID4VCI under HAIP, and pushed its CAEP interoperability vote back to restart
review. Post-quantum migration adds a new drag: ML-DSA-44 signatures break
cookie-size assumptions and OpenID Connect allows one signing algorithm per
relying party. Wallet deadlines are slipping in plain view. No EU member state
had a live production EUDI wallet on 2 September; Sweden points to 2028 to 2029.
The institutional picture, then, is fast inward hardening, vendor-scoped outward
identity, and standards that could bridge the two moving at their own pace
behind a migration nobody scheduled for.

Turn 5 – Long-Term Trajectory

Over three to five years, three trajectories are plausible, and the evidence
weights them unevenly.

The most likely is layered persistence. Human checks keep accreting and become
largely wallet-mediated in Europe from 2027 to 2029, later than published and
unevenly by country. Agents acquire identity through vendor ecosystems: an
agent working for a person carries a credential its platform issued, and
relying parties that have joined that platform's scheme accept it. Banks lead,
because Know Your Agent products are already being sold to them and card
networks have liability reasons to care. Government portals lag, because their
hardening budget is spent on their own estates and their legal model of access
is a citizen logging in. In this world the agent is better identified at a bank
than at a benefits office, and in both places the person who sent it is checked
more thoroughly than it is.

A second trajectory is incident-driven convergence. A second or third public
case of an outside agent at a government portal, this time touching personal
records, produces a requirement that agents declare themselves at public
services. That requirement would most likely be met by importing whatever the
vendor ecosystems have already built, so the public door ends up recognising
the private credential. This trajectory produces outward agent identity faster,
but on terms set by the vendors who got there first.

A third, least likely on current evidence, is that delegated authority is
anchored in the person's own wallet: the person's certified credential issues a
bounded mandate to an agent, checkable by any relying party that accepts the
wallet. The technical ingredients (key binding, verifiable presentations,
certified wallet implementers) exist, but the wallets themselves are not yet
live at scale, and nothing in the September 2026 record shows a wallet
programme adding delegation to its launch scope. d-you's launch list covers age
verification, contracts and bank accounts, not agents.

Across all three, one constant holds. The physical counter where a person is
recognised by someone who knows them does not come back. It survives where it
already exists, in kiosks, small branches and neighbourhood shops, as a
preference rather than a requirement, and its survival depends on whether
people keep choosing it when the checked alternative is faster.
