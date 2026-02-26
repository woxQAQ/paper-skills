---
name: project-technology-section-writer
description: Write and optimize the project-related technology section in Chinese technical papers. Use when the user needs to draft or revise technology/platform sections that must focus on technology selection rationale (why this platform/framework, what alternatives were considered, what problems are solved), instead of copying generic framework introductions.
---

# Project Technology Section Writer

Follow this workflow to draft or polish the project technology section.

## Workflow

1. Confirm project scenario, constraints, and target capabilities.
2. Identify candidate technologies and selected stack.
3. Explain selection rationale with explicit problem-solution mapping.
4. Draft by the structure in `references/technology-selection-sop-outline.md`.
5. Verify with `references/technology-selection-quality-checklist.md` and revise.

## Input Collection

Collect at least:
- project type, business scenario, and core requirements
- non-functional constraints (performance, maintainability, cost, deployment)
- candidate technologies/platforms and the final choice
- known pain points that the selected technology should solve
- implementation boundaries (team skill, timeline, existing system compatibility)

If user input is incomplete, state assumptions before writing.

## Writing Rules

- Do not paste generic framework history or official feature lists.
- Explain "why choose" before "what it is".
- Tie each selected technology to concrete project problems.
- Compare with at least one feasible alternative when possible.
- Keep arguments verifiable: requirement -> criterion -> selection -> expected benefit.

## Optimization Mode

When revising existing text:

1. Remove template-like introductions and empty slogans.
2. Strengthen the chain: requirement/constraint -> selection criterion -> platform choice.
3. Add concise comparative reasoning if alternatives are missing.
4. Keep only project-relevant technical details.
