# Theme exploration, agency, 2026-09-25

Turn 1 – Conceptual Frame

Agency has two meanings that the agent economy is now forcing apart. The first
is the capacity to act: to set a goal, choose among options and carry the
choice into the world. The second is older and legal: the relation in which
one party acts on behalf of another, so that the principal is bound by what
the agent does within the scope of its authority. For most of the history of
consumer technology the two meanings did not need to be distinguished, because
the person who wanted something was also the person who clicked. The agent
payment rails built in August and September 2026 separate them cleanly. The
capacity to act moves to software. The legal position of principal stays with
the person, and it is being reinforced rather than diluted.

The clearest statement of this came from a court rather than a product
launch. The Ninth Circuit's holding in Amazon v. Perplexity, left standing
when rehearing en banc was denied in September 2026 with no judge requesting
a vote, is that the user, not the agent provider, is the one who "accesses"
the site. That is a philosophical claim wearing a procedural coat: it says
that when a machine browses, the person on whose behalf it browses is the
actor. The payment side is converging on the same attribution by a different
route. Mastercard's Verifiable Intent and Visa's Trusted Agent Protocol are
designed to produce a record that the cardholder authorised a particular
agent to make a particular kind of purchase. The record's purpose is to make
the principal legible as the author of the transaction.

The conceptual difficulty is that authorisation and meaning are not the same
thing. A mandate is a finite text: a spending limit, a merchant list, a
product description, an approval setting. What a person wants is open-ended
and contextual. When the agent acts inside the text and outside the meaning,
the question of agency becomes a question of which of the two the law treats
as the person. The sweep records the industry's current answer precisely. It
treats the text as the person, and it describes the text as evidence rather
than as a rule. Usio's objection, that verifying an agent is legitimate does
not show it did what the customer asked, names the gap the frame leaves open.

Turn 2 – Societal Reframing

Seen from society rather than from the transaction, the shift is not that
machines gain agency but that people gain a new kind of responsibility they
did not ask for. The consumer is being reframed as a principal in the
technical legal sense: someone who issues instructions, bears the
consequences of their agent's authorised acts, and is expected to supervise.
That role has historically belonged to employers, companies and the wealthy,
people with staff. It is now being extended to anyone with a card and a
phone, through product defaults rather than through deliberation.

The evidence on public appetite runs strongly against the role. Visa's chief
executive said on 8 September 2026 that consumers shop with AI but have not
adopted autonomous agent payments, citing a survey in which 75% distrust
agentic platforms with autonomous payment authority. Only 7% of surveyed US
and UK fashion shoppers would let AI buy without their approval. The rails
are being built ahead of demand, which means the social terms of agency are
being settled by the people who build the rails, in the absence of the people
who will later live under them.

The response of the builders is revealing. Mastercard's consumer Agent Pay,
launched on 18 September 2026, lets cardholders give an agent a virtual card
with spending limits, merchant restrictions or approval before checkout. The
GoCardless payment on 22 September 2026, the UK's first live agentic bank
payment, kept the payer in control of limits or final approval. In other
words, the design answer to public distrust is to keep a human tap in the
loop. That answer resolves the distrust at the cost of converting every tap
into a signature. The more often the person approves, the more thoroughly
the record shows that they authorised, and the less the approval means as an
act of attention.

There is also a geography to the reframing. In China the question is being
settled by rule rather than by record: the payment association's convention
of 24 August 2026 places primary responsibility on whoever provides the
payment service, and Alipay reports agent-assisted purchase tasks up sevenfold
in five months. Where the provider carries the risk by default, adoption is
measurable. Where the customer carries it by default, adoption is a survey
finding about distrust.

Turn 3 – Psychological Implications

The psychological core of delegation is the expectation that the delegate
understands what one meant. Human delegation works because a competent
assistant asks, notices, and refuses when an instruction plainly misfires.
Agent delegation under the current rails replaces that tacit understanding
with an explicit artefact: a mandate the agent drafts from the person's words
and the person approves. The person does not write their own instruction in
the form that counts. They confirm a summary of it.

This produces a peculiar and probably durable experience, which is being held
to one's own paraphrase. When something goes wrong, the customer is shown a
document that says what they wanted, which they signed, which they did not
write and do not recognise as quite what they said. The feeling is not the
familiar one of being cheated, because nothing false has been done. It is
closer to being misquoted in one's own voice. People will experience it as a
small humiliation rather than a grievance, and small humiliations are the
kind people absorb rather than dispute, which matters for whether disputes
ever reach a volume that forces a rule.

Approval fatigue compounds this. If agents keep the human in the loop through
a confirmation tap, and the evidence on distrust suggests they must, the
number of taps rises with use. Confirmation becomes reflex. The person's
psychological experience of the approval is of clearing a notification, while
its legal meaning is of granting authority. The distance between those two
experiences is where the new disputes will live.

There is a counter-current. The existence of a record that the customer can
also see creates the possibility of testimony: the person can point to what
they actually said. Whether that possibility is real depends on whether the
agent provider keeps and surfaces the raw instruction alongside the summary.
Mastercard's description of Verifiable Intent as a paper trail describes what
the network holds, not what the person holds. The psychological experience of
agency in the next few years will turn on a mundane question: whether people
can retrieve their own words.

Turn 4 – Institutional Dynamics

Five institutions touch a disputed agent purchase, and the sweep shows each
of them moving on its own track. The card networks are building identity and
evidence: the joint KYA framework of 10 September 2026, run through the
Monetary Authority of Singapore's BuildFin.ai platform on top of MAS's SAFR
framework, and merchant tooling such as Mastercard Agent Connect and Visa
Intelligent Commerce Connect. None of it specifies liability. The disputes
themselves still run on existing reason codes; the grading pass found no
agent flag in the dispute system and no network reporting an agent-specific
wave.

Merchants are asserting control over which agents may enter. Amazon's block
of Meta's Muse around 20 to 21 September 2026 rests on its Conditions of Use,
the lever the Ninth Circuit pointed toward after the computer-fraud route
failed, and its amended complaint against Perplexity on 21 September
continues the fight on other grounds. The contradiction the sweep records,
that Amazon's own Buy for Me agent enrolled third-party retailers through an
opt-out email while it blocks outside agents for lack of consent, shows that
merchant consent to agents is being defined by whoever is the larger party in
each pair.

Agent providers sit between customer and merchant and have the most
information: they hold the customer's original words, the mandate they
drafted, and the agent's reasoning. They are also the party with no defined
position in the dispute system, because the card dispute runs between issuer,
network and merchant. Identity vendors are capitalising the gap: Baselayer's
$35M Series A on 23 September 2026 funds cryptographic verification of an
agent, its principal and its permissions, and an agentic fraud consortium.
That is verification of who acted and under what permission, not of whether
the act matched the meaning.

Regulators are split. The FCA's AI Live Testing programme hosted the
GoCardless payment, a design with payer final approval, so the supervised
evidence base consists of the configuration least likely to produce a
dispute. HM Treasury's consultation closes on 6 October 2026. The Beijing
Fintech Industry Alliance's standard adds a dual authorisation rule requiring
both user and institution consent. The Western dynamic is that private
rulebooks will allocate the first losses, and any statute will inherit their
precedents.

Turn 5 – Long-Term Trajectory

Over the next five years the likeliest trajectory is that consumer agency is
legally enlarged and practically thinned at the same time. Legally enlarged,
because every record the rails produce points to the person as principal, and
courts have begun to accept that attribution for access. Practically thinned,
because the person's part in each transaction shrinks to a confirmation of a
text they did not draft. The combination is stable as long as losses are
small and rare, which the current volume evidence says they will be for some
time. Visa's own statement that autonomous agent payments are not yet adopted
means the first disputes will be few, individually handled and resolved by
goodwill rather than by rule.

That is the important consequence of the slow adoption curve. A dispute
regime is usually shaped by a wave: a pattern of losses that makes the
allocation question unavoidable and public. The grading record shows no such
wave in sight, and the ledger's claim that a network would report one has now
graded open three times. In its absence, allocation will be set one case at a
time inside provider support queues and network arbitration, and the
precedents will be private. A provider that quietly refunds a customer whose
mandate summary misrepresented her instruction has made a decision about
agency, but not one anyone else can cite.

Two branches could change the trajectory. The first is statutory: if HM
Treasury's response sets out when an agent-initiated transaction counts as
authorised, the UK will have a public rule, though on the record of
regulatory timelines the rule will arrive later than announced and will
codify whatever the rulebooks have by then made normal. The second is
competitive: the Chinese model, in which the payment provider carries primary
responsibility and must define the agent's boundary in a signed agreement,
produces measurable adoption, and Western providers may copy the allocation
because it sells, not because it is required. Alipay's sevenfold growth in
agent purchase tasks is the first evidence that provider-borne risk can be a
product feature.

The deepest long-term question is whether the person's own words survive as
an object in the system. If the raw instruction is kept, surfaced and given
evidential weight, agency can be contested and therefore defended. If only
the drafted mandate survives, the person will be the author of record of
decisions they described but never made.
