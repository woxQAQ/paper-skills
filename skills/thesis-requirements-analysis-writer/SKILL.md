---
name: thesis-requirements-analysis-writer
description: Write and optimize the system requirements analysis chapter in Chinese technical papers and graduation projects. Use when the user needs to draft, rewrite, expand, or polish sections 3.1-3.4 (system overview, requirements elicitation, functional analysis model, non-functional requirements), including UML-oriented requirement artifacts and use-case description tables.
---

# Thesis Requirements Analysis Writer

Follow this workflow to produce or optimize chapter 3 requirements analysis content.

## Workflow

1. Confirm the system scope, stakeholders, and chapter target.
2. Collect requirement sources, interview findings, and business process context.
3. Draft sections 3.1-3.4 in order using `references/requirements-analysis-sop-outline.md`.
4. Build functional artifacts (use-case list, use-case description table, dynamic behavior models).
5. Run quality checks with `references/requirements-analysis-quality-checklist.md` and revise weak parts.

## Input Collection

Collect at least:
- project/system name, target users, and business scenario
- user pain points, implementation motivation, and expected gains
- stakeholder list and elicitation evidence (interview/workshop/document analysis)
- core business process and current workflow bottlenecks
- candidate use cases and priorities
- measurable non-functional constraints (reliability, maintainability, performance, recoverability, deployment)

If input is incomplete, state assumptions explicitly before drafting.

## Writing Rules

- Keep a clear chain: business problem -> requirement source -> model expression -> requirement conclusion.
- Ensure section 3.1 reflects requirement-analysis artifacts, not only narrative text.
- In section 3.2, explain elicitation method and stakeholder mapping, not only final conclusions.
- In section 3.3, provide use-case diagram support and at least one use-case description table using `references/use-case-description-table-template.md`.
- For dynamic behavior, choose suitable UML views (activity/sequence/state) tied to concrete scenarios.
- In section 3.4, express non-functional requirements with quantifiable indicators.

## Optimization Mode

When revising existing chapter text:

1. Diagnose by subsection: missing requirement source, weak model mapping, unquantified constraints, or logical gaps.
2. Preserve valid facts and rewrite only weak or generic paragraphs.
3. Return revised text plus a short gap list of missing evidence/artifacts.
