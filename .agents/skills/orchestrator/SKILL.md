---
name: orchestrator
description: Execute full monthly loop across all themes using step-first folder structure. Maintains a PROGRESS.md file for tracking and resumability.
---

# orchestrator

## Purpose

Execute the full monthly loop across all themes using step-first folder structure. 
Maintain a `PROGRESS.md` file to ensure resumability and strict sequential processing.

## Feature Flag

USE_DEEP_RESEARCH = true

Must be passed to evidence-layer.

## Workflow

1. Read themes from themes/THEMES.md
2. Determine current month in format YYYY-MM
3. Create directory structure:

output/YYYY-MM/
  00-structural-question/
  00_5-evidence/
  01-exploration/
  02-pestle/
  03-forces-feelings/
  04-scenario/
  05-evaluation/

4. Initialize or update `output/YYYY-MM/PROGRESS.md`:
   - List all 22 themes.
   - Mark themes as [ ] Pending, [/] In Progress, or [x] Completed.

5. For each theme labeled [ ] Pending:

   a. Mark theme as [/] In Progress in `PROGRESS.md`.
   
   b. **Step 00: structural-question**
      - Input: theme name.
      - Output: `output/YYYY-MM/00-structural-question/<theme>.md`.

   c. **Step 00_5: evidence-layer**
      - Input: theme name + content of Step 00.
      - Feature Flag: use_deep_research = true.
      - Output: `output/YYYY-MM/00_5-evidence/<theme>.md`.

   d. **Step 01: theme-exploration**
      - Input: theme name + content of Step 00 + content of Step 00_5.
      - Output: `output/YYYY-MM/01-exploration/<theme>.md`.

   e. **Step 02: pestle-analysis**
      - Input: theme name + content of Step 01 + content of Step 00_5.
      - Output: `output/YYYY-MM/02-pestle/<theme>.md`.

   f. **Step 03: forces-feelings**
      - Input: theme name + content of Step 01 + content of Step 02 + content of Step 00_5.
      - Output: `output/YYYY-MM/03-forces-feelings/<theme>.md`.

   g. **Step 04: scenario-generator**
      - Input: theme name + content of Step 01 + content of Step 02 + content of Step 03 + content of Step 00_5.
      - Output: `output/YYYY-MM/04-scenario/<theme>.md`.

   h. **Step 05: scenario-eval**
      - Input: theme name + contents of Steps 01, 02, 03, and 04.
      - Output: `output/YYYY-MM/05-evaluation/<theme>.md`.

   i. Mark theme as [x] Completed in `PROGRESS.md`.

6. Complete the loop until all themes in `PROGRESS.md` are [x] Completed.

## File Writing Rules

- File name must be lowercase theme name.
- Spaces replaced with hyphens.
- Overwrite existing file.
- Confirm file creation in each step.

## Constraints

- Deterministic execution.
- No cross-theme influence (process one theme fully before loading the next).
- Abort on format deviation.
- Do not merge steps into single file.
- Do not skip themes.
