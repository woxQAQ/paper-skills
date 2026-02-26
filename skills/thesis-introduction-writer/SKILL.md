---
name: thesis-introduction-writer
description: Write and optimize the Introduction chapter of Chinese technical papers and graduation projects. Use when the user needs to draft, rewrite, expand, or polish sections 1.1-1.5 (background/significance, domestic and international status, main problems solved, main work, chapter organization), strengthen technical positioning, and make the work uniqueness and references concrete.
---

# Thesis Introduction Writer

Follow this workflow to produce or optimize an introduction chapter.

## Workflow

1. Confirm paper type and context.
2. Collect core inputs (topic, scenario, technical route, related work, solved gaps).
3. Draft section 1.1-1.5 in order using the fixed structure in `references/introduction-sop-outline.md`.
4. Run quality checks with `references/introduction-quality-checklist.md` and revise weak parts.
5. Return the final polished version plus a short list of missing evidence (if any).

## Input Collection

Collect at least:
- project/topic name and application scenario
- development motivation, pain points, and expected value
- comparable domestic/foreign systems, methods, or products
- limitations of prior work and the target gap
- this project/paper concrete work items
- expected chapter arrangement (or infer a reasonable structure)

If inputs are missing, state assumptions clearly before drafting.

## Required Output Structure (1.1-1.5)

Use these exact section goals:

- 1.1 System development background and significance: Explain real context, urgency, and practical/technical value.
- 1.2 Domestic and international status of similar topics (or technology): Compare technical routes and summarize strengths/limitations.
- 1.3 Main problems solved: State specific problems, constraints, and challenge points.
- 1.4 Main work of this paper: Describe implemented work items; for non-research papers, avoid "main contribution" wording.
- 1.5 Organization of this paper: Briefly map each chapter's role.

## Writing Requirements

- Keep the logic chain explicit: "why this work" -> "what is lacking" -> "what we do".
- Base section 1.2 on technical analysis, not only narrative description.
- Make "features/innovation/challenges" concrete and verifiable; avoid vague claims.
- Concentrate citation placeholders mainly in sections 1.1 and 1.2 when evidence is required.
- Prefer concise academic Chinese and avoid exaggerated language.

## Optimization Mode

When rewriting an existing introduction:

1. Diagnose by section: missing logic, weak technical comparison, unsupported claims, repetition, or chapter mismatch.
2. Keep valid factual content; rewrite only weak paragraphs.
3. Produce:
   - revised full text, or
   - "before -> after" key paragraph upgrades if the user asks for incremental edits.
