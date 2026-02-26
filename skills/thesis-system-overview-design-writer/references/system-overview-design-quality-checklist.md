# System Overview Design Quality Checklist

Mark each item as pass/fail before final output.

## Positioning and Rationale

- [ ] Architecture rationale is explicit: design basis and constraints are stated before solution details.
- [ ] The chapter focuses on overview design (macro architecture), not detailed coding/design minutiae.
- [ ] Distinctive/innovative design points are highlighted and justified.
- [ ] Open-source/framework capabilities and self-developed work are clearly separated.

## 4.1 Static Structure (Required)

- [ ] At least one suitable static view is provided (functional, logical/component, layered, or deployment).
- [ ] Component responsibilities and connectors are clear and consistent with text.
- [ ] Chosen diagrams match project characteristics instead of template-driven "all-in" diagrams.

## 4.2 Dynamic Structure (Optional)

- [ ] If included, dynamic views are bound to critical runtime scenarios.
- [ ] Process view explains concurrency/synchronization/communication where relevant.
- [ ] Data-flow view clearly describes major data transformation paths.

## 4.3 Data Management (Generally Required)

- [ ] Data model includes entities, relations, and key attributes (ER-level clarity).
- [ ] Persistence strategy is explained (ORM/mapping/storage decisions).
- [ ] Key table/relationship design reflects business semantics and system constraints.

## 4.4 Optional Views and Consistency

- [ ] Security/development views are included only when meaningful, and provide concrete control points or implementation structure.
- [ ] Cross-section consistency holds: architecture, dynamic flow, and data model do not conflict.
- [ ] Diagram names, terms, and module names are consistent throughout chapter 4.

## Output Rule

If any critical item fails (rationale missing, static view missing, or data management missing), revise before final delivery and report what was fixed.
