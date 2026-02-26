---
name: thesis-system-detailed-design-implementation-writer
description: Write and optimize the system detailed design and implementation chapter for Chinese technical papers and graduation projects. Use when the user needs to draft, rewrite, expand, or polish content about module-level internal algorithms and data structures, UML detailed design artifacts (class/object/sequence/collaboration/state/activity), database detailed design (DB selection, table schema, table relationships, ORM/object-relational mapping, persistence and storage strategy), and algorithm-focused implementation narratives that avoid raw code dumping.
---

# Thesis System Detailed Design and Implementation Writer

Follow this workflow to produce or optimize a detailed design and implementation chapter.

## Workflow

1. Confirm chapter target, scope boundary, and key business flows.
2. Identify modules with high complexity or clear technical distinctiveness; deprioritize routine modules.
3. Draft detailed design with `references/detailed-design-implementation-sop-outline.md`.
4. Ensure artifact mapping consistency with `references/artifact-mapping-rules.md`.
5. Run quality checks with `references/detailed-design-implementation-quality-checklist.md` and revise weak parts.

## Input Collection

Collect at least:
- system/project name, chapter position, and target readers
- module decomposition and priorities (which modules are difficult, innovative, or high-risk)
- UML evidence for detailed design: class/object relations, sequence/collaboration flows, state transitions, activity paths
- database decisions: DB type selection reason, core tables, key fields, relationships, indexing/storage constraints
- persistence decisions: ORM mapping strategy, transaction boundaries, caching/consistency policy
- implementation focus: key algorithms, core execution steps, performance/stability handling points

If input is incomplete, state assumptions explicitly before drafting.

## Writing Rules

- Describe **problem -> method/pattern -> result -> benefit** in each key subsection.
- Prioritize design rationale (why this design) over exhaustive artifact listing.
- Focus on distinctive, difficult, or complex designs; move routine details to appendix if needed.
- Keep one business flow represented differently by phase: requirements use-case, design sequence/activity, implementation algorithm/flow or pseudocode; avoid duplicated cross-chapter retelling.
- In implementation text, explain algorithm steps and control logic; avoid code accumulation.
- Do not place large code/config blocks in main text. If unavoidable, show concise pseudocode in a text box as an "Algorithm" and config snippets in a text box as a "Figure".

## Optimization Mode

When revising existing text:

1. Diagnose by subsection: weak rationale, diagram-text mismatch, shallow DB design, repeated requirement-level narration, or code-heavy implementation writing.
2. Preserve valid facts and architecture decisions; rewrite only weak sections.
3. Return revised text plus a short gap list of missing diagrams/evidence/appendix items.
