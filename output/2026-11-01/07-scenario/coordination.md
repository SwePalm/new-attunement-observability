# Scenario, coordination, 2026-11-01

## 1. Title & Core Question
- Title: Targets Spec As Of
- Core Question: When the rooms that write the rules multiply faster than anyone can be paid to sit in them, what does it cost an unpaid person to keep a seat, and what does she give up to keep it?

## 2. Context Summary (Translation Layer) – Why This Future Exists
Standards for how software agents work across companies are being made in more places every month. A chartered Internet standards group began work in October with a first draft due only at the end of the year. A neutral foundation now hosts ten agent projects, four of them added in a single day. The best-known protocol keeps rewriting itself, retiring pieces under a year-long notice, and its group on agent work was turned from a decision-making body into a discussion circle. Yet the pieces that move money are used by a few dozen stores while the plain checkout runs on seventeen thousand, and one donated standard still has no numbered release. Governance has grown faster than anything that can be pointed to and relied on. This world is the one where the rooms are many, the editions are few, and keeping up is a job that only some people are paid to do.

## 3. Future World Snapshot (The Lived Experience) – A Day in This Future
Vantage: outsider or volunteer with no contract / a one-person payments-integration shop. Form: a case file, one working-group mailing-list thread and its replies, in the order posted. The Irreplaceable Thing is reachable only from this vantage, because the unpaid are the ones whose seat can be lost by a change of group status.

Subject: use-cases draft, delegated payment section, please review.

Ines, unpaid, to the list: "I maintain the connector that lets a buyer's agent pay a seller's, for eleven small shops. The draft says an agent 'may present a mandate'. In my traffic the mandate is bound on a few dozen stores and plain checkout on thousands. Please say what a seller does when no mandate arrives. Targets spec as of: this morning."

Chair: "Thanks. Out of scope for the use-cases document. Raise it when we reach the protocol drafts."
Ines's own note, kept in the file: The protocol drafts are months off. The last group I spoke in became a discussion circle the week after I joined it.

Vendor engineer, paid, same hour: "Agree on scope. We handle this in our product and will contribute text." Forty pages attached.
Ines's note: The call where the forty pages were discussed ran during shop hours. I was at the till. The minutes say no objections.

Ines to the list, three weeks on: "The same paragraph is now being rewritten in two other foundations, each with its own call and its own date. I follow three of the four. Which edition are we writing against?"
Chair: "Whichever you have."

Ines's note: On the shelf behind the till are four lanyards, one per foundation. A new customer asked what they were for. I said they prove I was in a room once.

Chair, private message: "Nobody has taken the glossary. It means defining 'mandate' once, for everyone. It is a chair, and it comes with the call invitation."

Ines's note: I said yes. I will lose a fifth of my working week, and the one client who pays by the hour.

Ines, to the list, glossary entry one: "Mandate: a signed instruction from a buyer that a seller can check without calling the buyer. Comments welcome. Targets spec as of: the draft above."

Chair: "Added to the agenda."

The seat is a line in an invitation list. When the call is moved to a time she cannot make, she keeps the line by dialling in from the till with the sound low, and says her one sentence into a shop full of customers.

## 4. Behavioral Shifts (Human Lens) – How People Adapt
Small integrators learn to treat a specification as a weather report: useful today, silent about next month. They write "targets spec as of" on tickets, pin the version they tested, and keep a private list of which counterpart is on which edition. Paid delegates from large vendors treat the rooms as part of their job and arrive with text prepared, so the draft tends to reflect what their products already do. Volunteers find that influence comes less from argument than from taking the dull task nobody wants, such as a glossary or a test table, because the person who defines the terms is hard to remove. People collect badges and credentials, the certification that matches an edition, the conformance tier of a software kit, and see that these age with the edition they certify. Some quit the rooms and rely on bilateral deals with the two or three counterparts that matter, which is cheaper and invisible. Customers rarely notice any of this until a handoff between two agents fails, and then they learn to route around it by phone. Managers at small firms ask a new question when hiring: whether the person can read a changelog and a mailing list without being paid to.

## 5. Structural Forces (System Lens) – What Holds This World Together
Three things keep the arrangement in place. First, the places that write the rules keep multiplying while their outputs arrive slowly. The Internet standards group's first deliverable is a document about use cases, not a protocol, and the foundation's newest projects joined without a tagged release or a new dated snapshot. Drafts and first editions are late more often than they are early, so the sensible assumption is that a frozen, widely adopted edition is still some way off. Second, the most used protocol changes underneath its users on a calendar of its own, retiring features after a year's notice and moving the group that worked on agent text into a looser status. Anyone who integrates has a dated maintenance bill. Third, private arrangement does the work that public standards have not yet done. Two companies write down which edition each will honour, and a conformance badge or a public adoption table decides in practice what counts as working. Agreement between two parties is cheap to make, and agreement among all parties has to wait. A bill to make operators liable for agents that attack other systems has been announced, and nothing about it is settled; for now the answer to who owns a failed handoff is whatever the two firms signed.

## 6. Reflection & Implications – Questions This World Asks Us
- If anyone may attend but only the paid can follow, what has openness actually given?
- Who should pay for a seat that the whole field benefits from, the people who hold it, the vendors who gain from it, or no one?
- When the person who defines the word is a volunteer, what does it cost her to keep defining it, and what do we owe her?

## 7. Pullback Layer: From Possibility to Probability
### 7.1 Signals Emerging (Plausible Zone) – Early Signals We Already See
- The IETF approved the agentproto working group's charter on 8 Oct 2026, with a use-cases draft due Dec 2026 and protocol drafts in Mar 2027 (source: https://datatracker.ietf.org/doc/charter-ietf-agentproto/history/, Oct 2026).
- The Agentic AI Foundation announced four new hosted projects on 22 Oct 2026, taking its roster to ten (source: https://aaif.io/news/agentic-ai-foundation-announces-four-new-projects, Oct 2026).
- The MCP Agents group was converted from a Working Group to an Interest Group on 16 Oct 2026 (source: https://modelcontextprotocol.io/community/interest-groups/agents.md, Oct 2026).
- The Agent Skills repository has no tag or release, and its last commit predates its donation (source: https://github.com/agentskills/agentskills, Nov 2026).
- The commerce protocol monitor shows AP2 Mandate bound on 37 stores against 17,056 on Checkout (source: https://ucpchecker.com/capabilities, Nov 2026).
- MCP's 2026-07-28 specification deprecated several features under a twelve-month minimum window (source: https://modelcontextprotocol.io/specification/2026-07-28/changelog.md, Jul 2026).

### 7.2 Probable Direction (Near-Term Future) – Where We're Likely Headed
The more probable path is continued growth in venues, slow arrival of frozen editions, and bilateral arrangements filling the gap. The IETF group will likely produce its first drafts, but early milestones on first publications have a record of slipping, so the architecture and protocol drafts are more likely to arrive late than on schedule. The foundation will probably keep adding projects, since adding a hosted project is a single announcement, while tagged releases and dated snapshots arrive project by project and unevenly. MCP will keep changing on its own calendar, and integrators will track its deprecation windows. Contracts and conformance programmes, which are cheaper than standards, will define what counts as compatible between most pairs of firms well before any common edition does. Small integrators will increasingly rely on one or two large counterparts' gateways instead of the open specification (inference). Expect the seats that matter to be held by paid staff of the larger vendors, with a few durable volunteers in roles like editing and testing. A liability bill is more likely to appear as hearings and drafts than as law inside two years.

### 7.3 Preferred Path (Intentional Future) – The Path We Could Choose Instead
- Standards projects publish a dated, tagged edition early and say how long it will hold still.
- Foundations fund seats for unpaid contributors, such as glossary and test editors, from the fees large members already pay.
- Groups that change status from decision-making to discussion say plainly where decisions now happen.
- Integrators write the specification edition and the responsible operator into their contracts.
- Public monitors of adoption show payment and authorisation layers beside plain checkout, so buyers see the gap.
- Vendors who bring forty pages to a call also bring a plain-language summary and post it ahead of time.

## 8. Connect to Today
### Skills We May Need
- Reading a changelog and a mailing list as a duty, not a favour.
- Taking the dull task that gives standing in a room.
- Writing a definition once so that others can cite it.
- Pinning a version and naming it in a contract.
- Saying one sentence in a meeting you can barely attend.
- Telling adoption from announcement.

### Signals & Refractions
- A ticket field reading "targets spec as of" with only a date is a refraction of governance that outruns tagged editions.
- A public adoption table consulted before a sales call refracts the gap between Checkout and the mandate.
- A group renamed from working to interest refracts the loss of a place where drafting text was decided.

## 9. Final Insight
Ines still has the seat, and the call is still moved to hours she cannot attend. She turned down, in the spring, a large vendor's offer to take the glossary over and pay her for it, because the terms were that the vendor's lawyers would review each entry first. The client who paid by the hour has gone. The invitation list shows her name under the word "editor", and nobody has asked whether she will be there next year.
