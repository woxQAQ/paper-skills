# Detailed Design and Implementation Quality Checklist

Mark each item pass/fail before final output.

## Design Rationale

- [ ] Each key section shows problem -> method/pattern -> result -> benefit.
- [ ] Distinctive/complex modules are prioritized; routine modules are compressed or moved to appendix.
- [ ] Diagram choice matches purpose (static vs interaction vs behavior).

## UML and Narrative Consistency

- [ ] Class/object relationships are reflected in text logic.
- [ ] Sequence/collaboration/activity/state descriptions are scenario-bound and not generic.
- [ ] No contradiction between diagram semantics and written explanation.

## Database Design Depth

- [ ] DB selection includes comparison and reason, not only a final statement.
- [ ] Core table design includes keys/constraints/relationships.
- [ ] ORM/persistence/storage strategy and trade-offs are explicitly discussed.

## Implementation Writing Quality

- [ ] Implementation emphasizes algorithm steps and control logic.
- [ ] Large raw code/config dumps are removed frommain text.
- [ ] If code-like content is necessary, it is expressed as concise pseudocode (Algorithm) or config figure.

## Cross-Chapter Alignment

- [ ] Same business flow is not redundantly repeated across requirements/design/implementation sections.
- [ ] Chapter transitions are clear and each chapter keeps its own abstraction level.

## Output Rule

If critical items fail, revise before final delivery and report what was fixed.
