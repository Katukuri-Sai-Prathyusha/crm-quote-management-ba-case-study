# Requirements Traceability Matrix (RTM)

## Project

CRM Quote Management Enhancement

## Purpose

The Requirements Traceability Matrix maps business requirements to functional requirements, user stories, acceptance criteria, and UAT test cases.

This ensures that each requirement is addressed and validated during the implementation lifecycle.

---

## Requirements Traceability Matrix

| Requirement ID | Business Requirement | Functional Requirement | User Story | Acceptance Criteria | UAT Test Case |
|---|---|---|---|---|---|
| BR-01 | Users should identify products as Standard or Optional | FR-01 | US-01 | AC-01 | UAT-01, UAT-02 |
| BR-02 | Optional products should remain visible | FR-02 | US-05 | AC-02, AC-10 | UAT-07 |
| BR-03 | Optional products should not contribute to Net Total | FR-03 | US-02 | AC-03, AC-04 | UAT-02, UAT-03 |
| BR-04 | Users should change product type | FR-04 | US-03, US-04 | AC-05, AC-07 | UAT-04, UAT-05 |
| BR-05 | Product type should be clearly displayed | FR-02 | US-01, US-05 | AC-02, AC-10 | UAT-07 |
| BR-06 | Multiple Standard and Optional products should be supported | FR-06 | US-06 | AC-11, AC-12 | UAT-06 |
| BR-07 | Net Total should recalculate after product type changes | FR-05 | US-03, US-04 | AC-06, AC-08 | UAT-04, UAT-05 |

---

## Traceability Flow

The requirement lifecycle can be represented as:

```text
Business Requirement
        ↓
Functional Requirement
        ↓
User Story
        ↓
Acceptance Criteria
        ↓
UAT Test Case
        ↓
Validation

Coverage Summary
Area	Count
Business Requirements	7
Functional Requirements	7
User Stories	6
Acceptance Criteria	12
UAT Test Cases	7
BA Validation

The traceability matrix provides visibility from the original business requirement through to validation.

It helps identify missing requirements, ensures that requirements are covered by user stories and acceptance criteria, and supports UAT planning.

Change Management

If a business requirement changes during the project, the corresponding functional requirements, user stories, acceptance criteria, and UAT test cases should be reviewed and updated to maintain traceability.
