# Test Analysis and Case Design Guide

Use this guide to strengthen section 6.2 and 6.3 quality.

## Explicit Requirement Mining

- Build a source-to-test-point trace table: source document -> requirement item -> test point.
- Prioritize test points tied to high risk, high frequency, or critical business paths.
- Separate functional and non-functional requirements (performance, reliability, usability, security, compatibility).

## Implicit Requirement Mining

- Infer hidden constraints from domain habits and user expectations.
- Ask targeted questions to stakeholders for ambiguous behaviors.
- Execute exploratory runs to discover undocumented edge cases.
- Convert inferred needs into verifiable test points with clear pass/fail criteria.

## Multi-Level Requirement Selection

- Do not force all levels to be detailed in main text; choose representative levels based on scope and risk.
- Keep the selection rationale explicit (for example: system + regression are detailed because release risk is highest).
- Summarize omitted similar tests as "same pattern" with one bridge explanation.

## Case Design Method Selection

Common methods to combine for key tests:
- equivalence partitioning
- boundary value analysis
- decision table
- cause-effect graph
- state transition testing
- scenario/use-case based testing
- error guessing

Use at least two methods for priority test modules and explain method-to-problem fit.

## Output Form Suggestions

- Requirement-to-test-point trace table
- Representative test case table with method labels
- Execution result summary table
- Defect distribution and residual issue summary
