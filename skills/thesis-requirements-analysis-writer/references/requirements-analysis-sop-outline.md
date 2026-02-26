# Requirements Analysis SOP Outline (Chapter 3)

Use this structure to draft section 3.1-3.4.

## 3.1 System Overview

Goal:
- Explain what users need from the new system.
- Explain why these needs drive system implementation.
- Explain what value users gain after system delivery.

Required content:
- Business background, core user roles, and usage scenario.
- Problem statement and implementation motivation.
- High-level requirement artifacts reference (use-case diagram, activity diagram, sequence diagram, business process diagram).

Suggested paragraph flow:
1. Scenario and stakeholders.
2. Existing pain points and requirement triggers.
3. System positioning and expected user value.
4. Transition to requirement elicitation.

## 3.2 Requirements Elicitation

Goal:
- Present how initial requirements are derived.
- Show stakeholder list and elicitation method.
- Clarify user problems and target outcomes.

Required content:
- Initial user needs summary.
- Stakeholder list (primary users, operators, managers, maintainers, external systems).
- Elicitation method and engineering approach (interview, observation, workshop, document analysis, prototype feedback).
- Initial system definition (narrative + table/figure).
- Current business flow and overall requirement constraints.

Suggested output format:
- Stakeholder table: role, concern, requirement focus.
- Elicitation record summary: method, object, key findings.
- Initial requirement list grouped by business domain.

## 3.3 Analysis Model (Functional Requirements)

Goal:
- Convert elicited requirements into analyzable functional models.
- Describe information domain, behavior domain, and interaction domain.

Required content:
- Use-case diagram with actor and system boundary.
- Use-case list and priority.
- Use-case description tables for key use cases.
- Dynamic modeling with suitable UML artifacts:
  - Activity diagram for business flow
  - Sequence diagram for interaction timing
  - State diagram for lifecycle-sensitive objects (if needed)

Minimum recommended coverage:
- At least one overall use-case diagram.
- At least three key use-case description tables.
- At least one dynamic diagram that matches a key scenario.

## 3.4 Non-Functional Requirements

Goal:
- Define quality attributes and constraints of a satisfactory system.
- Express requirements with measurable indicators.

Required content:
- Reliability (e.g., fault rate, availability, recoverability).
- Maintainability (e.g., mean repair time, modularity, diagnosability).
- Performance (e.g., response time, throughput, concurrent users).
- Security/compliance (if applicable).
- Deployment and development environment constraints.

Suggested presentation:
- Use a measurable requirement table:
  - attribute
  - indicator definition
  - target value
  - verification method

Check:
- Avoid vague expressions such as "high performance" or "good stability" without metrics.
