# Project Brief: The Living Almanac

A kickoff document for a NEW project and a NEW conversation. It is written to
be read cold, with no access to the conversation that produced it. If you are
a fresh Claude session: read this top to bottom, then help the maintainer
build the smallest first step described near the end. Do not assume prior
context.

## One-line summary

Build a small monthly publication that harvests the compounding value of the
Attunement Observatory: not its scenarios (which are abundant and easy to
generate), but its graded track record of predictions over time.

## Background: where the data comes from

There is an existing project called the Attunement Monthly Observatory.
- Repo: github.com/SwePalm/new-attunement-observability
- Local checkout (on the maintainer's machine): ~/experiements/new-attunement-observability
- What it does: once a month it runs a foresight pipeline across 22
  "Human-AI" themes. It grades its own past predictions against reality,
  gathers cited evidence, picks the themes that moved most, and writes
  deep-dive future scenarios plus a synthesis essay.

The Living Almanac is a SEPARATE project. It does not change the observatory.
It reads the observatory's output as a data source and turns it into
something people can follow month over month. Recommended: make it its own
repo, and have it read the observatory either from a local clone or by
cloning the public GitHub repo.

## The core insight (do not lose this)

The observatory produces several kinds of output. Ranked by how valuable they
are to harvest over time:

1. HIGH VALUE, and unique: the signals ledger and its drift. Every month the
   pipeline logs falsifiable predictions with due dates, then grades them as
   they come due (confirmed, decayed, falsified, expired). Over a year this
   becomes a public batting average. Nobody else has this. It is worth MORE
   every month. This is the asset the almanac is built on.
2. MEDIUM VALUE: the monthly Outlook essay (the readable synthesis).
3. LOW VALUE to harvest, high engagement: the scenarios ("a day in this
   future"). Vivid and shareable, but abundant. Anyone can generate these.
   Use them as the hook, not the substance.

The mistake to avoid: building a pretty browser ("explorer app") over the
scenarios. That presents static content and asks the reader to dig, with no
payoff, and it does not compound. Build on the track record instead.

## What the Living Almanac is

A monthly publication with three layers, in order of importance:

1. The spine: a public SCORECARD. Every prediction the observatory has made,
   its due date, and its current status as it ages from open to confirmed or
   falsified. This is the part that grows more compelling every month and that
   cannot be faked, because it takes real elapsed time to accrue. Show the
   drift: how the pipeline's accuracy and its self-corrections evolve.
2. The front page: THIS MONTH'S OUTLOOK essay, the readable story that makes a
   stranger care.
3. The feature: ONE scenario per issue, the "video in your head" piece. This
   is the shareable hook. A generated video or a NotebookLM audio piece of
   this one scenario is a fine distribution channel. It is not the project.

Why a publication beats an app: a publication with a track record tells a
story that changes and earns trust as it ages. The drift becomes the product,
not a byproduct.

## The data contract (what to read)

All paths are inside the observatory repo.

- Ledger (the prediction record): `ledger/<theme>.md`, one file per theme,
  append-only. Each claim is a markdown block roughly like:
  ```
  ### <theme>-YYYY-MM-NN
  - Claim: <specific actor + observable expected event + timeframe>
  - Horizon: 0–12 months (logged YYYY-MM, resolve by YYYY-MM)
  - Source: <URL, Mon YYYY>
  - Status: open | confirmed | decayed | falsified | expired
  - Grades:
    - YYYY-MM-DD: <grade>, <one sentence> (source: URL, Mon YYYY)
  ```
  Claims live under "## Open claims" or "## Resolved claims". A parser should
  extract: id, claim text, resolve-by date, status, and each dated grade line.
- Calibration memo (what the pipeline learned about its own biases):
  `ledger/CALIBRATION.md`.
- Run outputs: `output/YYYY-MM-DD/` (one folder per run, keyed to the day it
  ran, since a month can hold more than one run). Notably:
  - `09-outlook/outlook.md` (the essay, published piece)
  - `09-outlook/delta-report.md` (the accountability companion: scorecard,
    what changed, claims on the clock)
  - `07-scenario/<theme>.md` (the scenarios, section "3. Future World
    Snapshot" is the "a day in this future" passage)
  - `SELECTION.md` (which themes were chosen and why)
- Method contract: `CLAUDE.md` in the observatory repo explains the whole
  pipeline if you need more detail.

Note: the delta-report already assembles much of the scorecard material each
month. The almanac can lean on it rather than re-deriving everything.

## Hard constraints and preferences

- NO em-dashes anywhere in any output. Use commas, periods, colons, or
  parentheses. This is a firm maintainer preference across all their work.
  (En-dashes in numeric ranges like "0-12 months" are fine.)
- Plain, accessible language. Define terms; do not assume the reader knows
  jargon.
- The maintainer thinks visually ("plays out like a video in my head"). Favor
  scannable, visual, timeline-style presentation of the drift over dense text.
- Do not modify the observatory repo or its pipeline. Read only.
- Keep the human in the loop: the observatory deliberately has a human review
  gate before publishing. The almanac should assume a human curates each issue.

## Smallest first step (build this first, nothing more)

Do not build an app or pick a framework yet. Build ONE static page that:
1. Reads all `ledger/*.md` files and renders a single scorecard: every claim,
   its resolve-by date, and its status, sorted so the soonest-to-resolve and
   the recently-graded are visible first.
2. Shows this month's `outlook.md` above it as the front page.
3. Nothing else.

This is roughly a weekend. It exists to test one thing: whether the
track-record framing has real pull. If it does, grow it into the full
almanac. If it does not, very little was spent finding out.

In parallel, as a separate distribution test, the maintainer may turn one
scenario into a short video or NotebookLM piece to see how the hook travels.
Treat that as a channel experiment, not the project.

## Non-goals

- Not an "explorer" that just presents the existing scenarios more prettily.
- Not a scenario-video generator as the core product.
- Not a rebuild or fork of the observatory pipeline.

## Open questions for the maintainer (resolve early in the new conversation)

- Audience: is this just for you, or public? (Changes hosting, tone, polish.)
- Hosting: static site (simplest) versus something interactive later.
- How to visualize "drift" over time: a timeline, an accuracy trend, a
  claim-by-claim aging view? Pick one for v0.
- How much automation: regenerate the page when the observatory updates, or
  curate each issue by hand?

## Suggested kickoff prompt for the new conversation

"I want to build the Living Almanac described in docs/living-almanac-brief.md
in my observatory repo (github.com/SwePalm/new-attunement-observability). Read
that brief, then let's build only the smallest first step: one static page
that renders the signals ledger as a scorecard plus this month's outlook.
Start by showing me how you'll parse the ledger files, and ask me the open
questions in the brief before writing code."
