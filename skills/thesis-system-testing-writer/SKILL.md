---
name: thesis-system-testing-writer
description: Write and optimize the system testing chapter for Chinese technical papers and graduation projects. Use when the user needs to draft, rewrite, expand, or polish chapter 6 testing content, including software development process testing and software product testing, test overview, explicit/implicit test requirement analysis, multi-stage test requirement selection (unit/integration/configuration item/system/acceptance/regression), test case design methods, and execution records with coverage/defect/residual risk based conclusions.
---

# Thesis System Testing Writer

Follow this workflow to produce or optimize a thesis system testing chapter.

## Workflow

1. Confirm chapter goal, scope boundary, and test-level selection strategy.
2. Split testing content into development-process testing and product testing.
3. Draft sections 6.1-6.4 with `references/system-testing-sop-outline.md`.
4. Apply test-demand mining and case-design guidance from `references/test-analysis-and-case-design-guide.md`.
5. Run quality checks with `references/system-testing-quality-checklist.md` and revise weak parts.

## Input Collection

Collect at least:
- system/project name, chapter target, and thesis length constraints
- process-testing artifacts to sample (documents/modules/components and why selected)
- product-testing objects (product description, user documents, software media/package)
- available requirement sources and known constraints
- selected test levels and rationale (unit/integration/configuration item/system/acceptance/regression)
- planned metrics and evidence (coverage, defect statistics, unresolved issues, resource consumption)

If input is incomplete, state assumptions explicitly before drafting.

## Writing Rules

- Prioritize test analysis and test case design depth over exhaustive test listing.
- Explain both explicit test requirements (from visible documents) and implicit test requirements (from experience, inquiry, and system probing).
- Keep chapter content tailorable: detail key tests and summarize similar tests due to length constraints.
- For key test parts, describe at least two different test case design methods.
- In execution and conclusion, report measurable data, process metrics, product quality metrics, residual defects, and pass/fail judgment.
- Keep narrative evidence-based and avoid unsupported "all passed" style claims.

## Optimization Mode

When revising existing testing text:

1. Diagnose by subsection: weak test scope declaration, shallow demand analysis, single-method case design, missing metrics, or weak conclusion traceability.
2. Preserve valid facts and measured data; rewrite only weak or generic sections.
3. Return revised text plus a short gap list of missing evidence/tables/records.
