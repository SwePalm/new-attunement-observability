# Attunement Monthly Observatory

## Entry Skill

orchestrator

This is the only entrypoint skill.

## Mission

Execute a deterministic monthly foresight pipeline across 22 Human–AI themes.

This agent is NOT autonomous.
It follows a fixed phase order.

## Current Implementation Scope

Full monthly pipeline (Step 00 to Step 05):

For each theme:

1. Generate structural question
2. Generate evidence layer
3. Generate theme exploration
4. Generate PESTLE analysis
5. Generate forces-feelings
6. Generate scenario
7. Run scenario evaluation
8. Write output to step-first folder structure

## Feature Flag

USE_DEEP_RESEARCH = true

Deep Research is required for Step 00_5 while this flag is true.
If toggled to false, mock mode may be used for development only.

## Folder Strategy

All outputs must follow step-first structure:

output/YYYY-MM/
  00-structural-question/
  00_5-evidence/
  01-exploration/
  02-pestle/
  03-forces-feelings/
  04-scenario/
  05-evaluation/
  PROGRESS.md

Each theme gets one file per step.

## Execution Rules

- Sequential theme processing
- No cross-theme influence
- Strict output format adherence
- Abort if format deviates
- Overwrite existing files for the same month
- Maintain PROGRESS.md with [ ] Pending, [/] In Progress, [x] Completed
