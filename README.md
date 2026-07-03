# Attunement Monthly Observatory

A monthly foresight loop across 22 Human–AI themes that treats deep research
as **re-search**: every run grades the previous runs' claims against reality
before making new ones. The project transforms abstract philosophical
questions into grounded, institutional near-future scenarios, and keeps a
public score of how its own claims fare.

## 🚀 Mission

Produce evidence-anchored foresight artifacts on a 0–5 year horizon, with a
compounding memory (the signals ledger) and an honest monthly scorecard.

## 🛠 Architecture (method v2)

Agent skills for Claude Code, orchestrated as a phased monthly loop.

- **Entry point**: `CLAUDE.md` (learning contract, invariants, loop definition)
- **Skills**: `.claude/skills/`, `orchestrator` is the only monthly entry skill
- **Themes**: `themes/THEMES.md` (22 themes)
- **Memory**: `ledger/`, append-only per-theme claims + bounded `CALIBRATION.md`
- **Output**: `output/YYYY-MM/`
- **Method changes**: `proposals/`, quarterly `instrument-review`, human-merged

## 🔄 The monthly loop

1. **Grade** (`signal-grading`), research every open ledger claim; grade it
 confirmed / decayed / falsified / expired / open, with sources. Distill
 recurring errors into bounded calibration heuristics.
2. **Sweep** (`evidence-sweep`), real, cited research across all 22 themes.
 Hard citation gate: no URL + date, no claim. Each sweep logs 2–4 new
 falsifiable claims to the ledger.
3. **Select** (`theme-selection`), rank themes by evidence delta; pick 4–6
 for deep dives. Every theme is covered at least once per 5 months.
4. **Deep-dive** (selected themes only), structural-question → exploration →
 PESTLE → forces-feelings → scenario → epistemic eval.
5. **Outlook** (`outlook-generator`, manual after human review), the monthly
 essay, opening with the scorecard and what changed since last month.

## 🧠 The learning contract

Three layers, three speeds (details in `CLAUDE.md`):

| Layer | Where | Changes | Gate |
|-------|-------|---------|------|
| State | `ledger/*.md` | every run | append-only |
| Calibration | `ledger/CALIBRATION.md` | monthly | max 10 heuristics, evidence-cited, auto-expiring |
| Instrument | `.claude/skills/` | quarterly at most | human merges proposals, METHOD_VERSION bump |

Calibration corrects the pipeline's observed biases without touching the
skills; skills only change through human-reviewed proposals, so scorecards
stay comparable within a method version.

## 🗓 Monthly operating procedure

Target run date: the 25th of each month.

1. Run `orchestrator` (Phases A–D).
2. Review the grading scorecards, SELECTION.md, and the deep-dive evals.
3. Regenerate weak artifacts if needed.
4. Run `outlook-generator` in `debug` mode; review for readability and grounding.
5. Run `outlook-generator` in `production` mode for publication.

## 📜 History

The `output/2026-02/` run predates method v2 (built with a different
architecture and no real research). Its forward-looking horizon claims were
seeded into the ledger, marked ungrounded, so the first v2 run can grade
the old baseline.
