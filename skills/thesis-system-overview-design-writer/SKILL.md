---
name: thesis-system-overview-design-writer
description: Write and optimize the system overview design chapter (typically chapter 4) for Chinese technical papers and graduation projects. Use when the user needs to draft, rewrite, expand, or polish section 4.1-4.4, including static architecture views (functional, logical/component, layered, deployment), optional dynamic views (process/data flow), data management design (ER/model mapping), and optional security/development views while emphasizing design rationale (Why) before implementation details (How).
---

# Thesis System Overview Design Writer

Follow this workflow to produce or optimize chapter 4 system overview design content.

## Workflow

1. Confirm chapter target, system boundary, and scenario.
2. Collect architectural constraints, design drivers, and key technical decisions.
3. Draft section 4.1-4.4 with `references/system-overview-design-sop-outline.md`.
4. Keep architecture discussion at macro level: component + connector + rationale.
5. Run quality checks with `references/system-overview-design-quality-checklist.md` and revise weak parts.

## Input Collection

Collect at least:
- project/system name, core business scenario, and target users
- design drivers: performance, reliability, scalability, security, maintainability, cost, delivery constraints
- candidate architecture options and final selection reason (why this scheme)
- main components/modules and key connectors (API, message bus, DB link, file flow)
- deploy environment (node roles, network, middleware, runtime)
- data model and persistence strategy (core entities, relationships, ORM/persistence mapping)
- optional dynamic cases (critical business flow, concurrency/sync/communication concerns)

If input is incomplete, state assumptions explicitly before drafting.

## Required Output Structure (4.1-4.4)

- 4.1 System static structure (required): choose suitable views from functional, logical/component, layered, and deployment view; do not force all UML diagrams.
- 4.2 System dynamic structure (optional): for key runtime behavior, use process view (sequence/activity) or data-flow view.
- 4.3 System data management (generally required): describe ER model, key table relationships, persistence mapping, and storage strategy.
- 4.4 Others (optional): include security view, development/implementation view, or system-specific highlights.

## Writing Rules

- Start each major subsection with design basis and decision reason (Why), then describe realization path (How).
- Prioritize architecture-level description over low-level implementation details.
- For static structure, make component responsibilities and connectors explicit.
- For dynamic structure, bind diagrams to concrete business scenarios and state transitions.
- For data management, ensure consistency among business objects, logical model, and physical storage.
- Distinguish self-developed work from reused open-source frameworks; clarify what is extended/customized.
- Expand innovative or distinctive parts; keep generic/common parts concise.

## Optimization Mode

When revising existing chapter text:

1. Diagnose by subsection: missing rationale, weak view selection, shallow data design, diagram-text mismatch, or over-detailed implementation.
2. Preserve valid facts and architecture choices; rewrite generic or unsupported claims.
3. Return revised text plus a short gap list of missing evidence/diagrams.
