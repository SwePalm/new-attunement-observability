# Attunement Monthly Observatory

A deterministic foresight engineering pipeline designed to execute a monthly loop across 22 Human–AI themes. The project transforms abstract philosophical questions into grounded, institutional near-future scenarios through a multi-step orchestration process.

## 🚀 Mission
To produce high-fidelity, evidence-anchored foresight artifacts that explore the structural consequences of AI-Human attunement on a 0–5 year horizon.

## 🛠 Project Architecture
The project is built on a modular "Agent Skill" architecture, where an **Orchestrator** manages a sequential workflow of specialized functional skills.

- **Entry Point**: `AGENTS.md`
- **Themes**: `themes/THEMES.md` (22 core themes)
- **Skills**: Located in `.agents/skills/` (Compliant with [Agent Skills Specification](https://agentskills.io/specification))
- **Output**: Located in `output/YYYY-MM/`

## 🔄 The 7-Step Workflow
Each theme is processed through a strict, sequential pipeline. Outputs from earlier steps serve as inputs for subsequent ones:

1.  **Step 00: Structural Question** (`00-structural-question/`)
    - Identifies the most consequential question for the theme within a 6–24 month horizon.
2.  **Step 00.5: Evidence Layer** (`00_5-evidence/`)
    - Compiles verified developments, signals, and shifts using deep research with source citation.
3.  **Step 01: Theme Exploration** (`01-exploration/`)
    - Produces a 1,500+ word deep dive into conceptual, societal, and psychological implications.
4.  **Step 02: PESTLE Analysis** (`02-pestle/`)
    - Translates exploration insights into concrete Political, Economic, Social, Technological, Legal, and Environmental forces.
5.  **Step 03: Forces & Feelings** (`03-forces-feelings/`)
    - Defines the "DNA" of the world: Systemic Contradictions and the "Single Irreplaceable Thing."
6.  **Step 04: Scenario Generator** (`04-scenario/`)
    - Generates a grounded, narrative-driven Pathfinder Scenario (0–5 year horizon).
7.  **Step 05: Scenario Eval (Epistemic Audit)** (`05-evaluation/`)
    - Conducts a disciplined audit of the scenario to validate structural compliance and narrative inflation risk.

## 📂 Folder Strategy
Outputs follow a **step-first** folder structure to allow for easy cross-theme comparison of specific stages:

```text
output/YYYY-MM/
├── 00-structural-question/
├── 00_5-evidence/
├── 01-exploration/
├── 02-pestle/
├── 03-forces-feelings/
├── 04-scenario/
├── 05-evaluation/
└── PROGRESS.md
```

## 📊 Progress Tracking
The `PROGRESS.md` file in the current month's folder ensures resumability and strict sequential processing across all 22 themes. It tracks which themes are Pending `[ ]`, In Progress `[/]`, or Completed `[x]`.

## ⚙️ Feature Flags
- `USE_DEEP_RESEARCH`: Set to `true` for production monthly runs. When set to `false`, `evidence-layer` may run in mock/development mode.

---
*Created by Antigravity for the Attunement Observatory.*
