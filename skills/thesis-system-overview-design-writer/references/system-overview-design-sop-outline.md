# System Overview Design SOP Outline

Use this scaffold when drafting chapter 4 system overview design.

## Core Principle

- Describe architecture at macro level: component + connector + rationale.
- Explain "Why this architecture" before "How to implement it".
- Keep common/generic content concise; expand innovative and project-specific parts.

## 4.1 System Static Structure (Required)

Choose suitable views; do not mechanically include every UML diagram.

### 4.1.1 Functional View (optional but common)

- Decompose the system into major functional modules.
- Clarify module goals, boundaries, and external interfaces.
- Suggested figure: functional module diagram.

### 4.1.2 Logical View / Component View (recommended)

- Describe user-facing and supporting modules.
- Define component responsibilities, dependencies, and collaboration interfaces.
- Suggested figure: UML component diagram.

### 4.1.3 Layered Logical Architecture (when layered system is obvious)

- Applicable to Java EE or similar layered systems.
- Explain layers (presentation, business, data, infrastructure) and cross-layer constraints.

### 4.1.4 Deployment View / Physical View (as needed)

- Map executable programs, runtime libraries, middleware, and system software to physical nodes.
- Explain deployment support for reliability, scalability, availability, and maintainability.
- Suggested figure: UML deployment diagram.

## 4.2 System Dynamic Structure (Optional)

Select only flows that are architecturally critical.

### 4.2.1 Process View

- Focus on runtime process/thread/object collaboration and concurrency/synchronization/communication.
- Suggested figures: sequence diagram, activity diagram.
- Activity diagrams should reflect action flow and state/result change.

### 4.2.2 Data Flow View

- Describe end-to-end information transformation from input to output.
- Show key data carriers and transformations on each path.
- Suggested figure: data-flow diagram (DFD), optionally annotate key data on arrows.

## 4.3 System Data Management (Generally Required)

### 4.3.1 Data View and Persistence Strategy

- Describe data flow, persistence model, object-relational mapping, and storage strategy.
- Explain mapping among object model, tables, procedures/triggers (if used).

### 4.3.2 ER Model

- Identify entities, relationships, and attributes.
- Use ER diagram to support communication between business and technical perspectives.

### 4.3.3 Key Data Structures (as needed)

- Present critical entities, relation model, and physical model.
- Explain table design rationale, indexing/partitioning/archival (if relevant).

## 4.4 Other Views (Optional)

### 4.4.1 Security View

- Summarize security architecture and control points.
- Highlight identity/authentication, authorization, auditing, transmission/storage protection, and key security files/configurations.

### 4.4.2 Development/Implementation View

- Describe implementation model: source code organization, executables, web resources, framework layers.
- Clarify framework usage boundaries and self-developed extensions.

## Closing Requirement

When describing architecture ideas, explicitly reflect design patterns or architectural principles where meaningful.
Always provide concrete project-specific structure diagrams instead of generic templates.
