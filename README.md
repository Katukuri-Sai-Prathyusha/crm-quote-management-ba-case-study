# CRM Quote Management Enhancement – Business Analyst Case Study

## 📌 Project Overview

This portfolio project demonstrates the end-to-end Business Analysis lifecycle for a CRM quotation management enhancement.

The project focuses on a business requirement to allow users to include optional products in customer quotations without including those products in the quotation Net Total.

The case study demonstrates how a Business Analyst gathers requirements, analyzes the existing process, documents the proposed solution, creates user stories, defines acceptance criteria, and prepares UAT scenarios.

---

## 🎯 Business Problem

Users need to present alternative products to customers as optional items within quotations.

However, optional products may be included in the quotation Net Total, resulting in inaccurate quotation values and additional manual effort.

### Business Impact

- Incorrect quotation totals
- Manual calculations
- Increased risk of pricing errors
- Additional customer clarification
- Limited flexibility in quotation preparation

---

## 💡 Proposed Solution

Introduce a Standard/Optional classification for products within quotations.

### Standard Product

A Standard product contributes to the quotation Net Total.

### Optional Product

An Optional product remains visible in the quotation but does not contribute to the Net Total.

### Example

| Product | Type | Price | Included in Net Total |
|---|---|---:|---|
| Product A | Standard | ₹10,000 | Yes |
| Product B | Standard | ₹5,000 | Yes |
| Product C | Optional | ₹3,000 | No |

**Net Total = ₹15,000**

---

## 👩‍💼 Business Analyst Responsibilities

This case study demonstrates the following BA activities:

- Requirement Gathering
- Stakeholder Analysis
- Business Requirement Analysis
- Gap Analysis
- As-Is / To-Be Process Analysis
- PRD Creation
- Functional Requirements
- User Story Creation
- Acceptance Criteria
- UAT Test Case Preparation
- Requirements Traceability
- Change Management

---

## 📂 Project Deliverables

| Document | Description |
|---|---|
| [Business Problem](01-Business-Problem.md) | Business problem, impact, and objectives |
| [Stakeholder Analysis](02-Stakeholder-Analysis.md) | Stakeholders and responsibilities |
| [Requirement Gathering](03-Requirement-Gathering.md) | Requirement elicitation and business requirements |
| [As-Is / To-Be Process](04-As-Is-To-Be-Process.md) | Current and proposed business process |
| [PRD](05-PRD.md) | Product and functional requirements |
| [User Stories](06-User-Stories.md) | User stories and acceptance criteria |
| [UAT Test Cases](07-UAT-Test-Cases.md) | User acceptance testing scenarios |
| [Requirements Traceability Matrix](08-Requirements-Traceability-Matrix.md) | Requirement-to-testing traceability |

---

## 🔄 Business Analysis Lifecycle

```text
Customer / Business Need
          ↓
Requirement Gathering
          ↓
Requirement Analysis
          ↓
As-Is Process Analysis
          ↓
To-Be Process
          ↓
PRD / Functional Requirements
          ↓
User Stories
          ↓
Acceptance Criteria
          ↓
Development
          ↓
UAT
          ↓
Implementation
🛠️ BA Skills Demonstrated

Requirements:
Requirement Gathering, Requirement Analysis, Business Requirements, Functional Requirements, Gap Analysis

Documentation:
PRD, User Stories, Acceptance Criteria, Process Documentation, RTM

Stakeholder Management:
Customer Communication, Stakeholder Collaboration, Requirement Clarification

Testing:
UAT Planning, Test Scenarios, Expected Results, Requirement Validation

Methodology:
Agile / Scrum, Requirement-to-Delivery Lifecycle

📌 Disclaimer

This is a portfolio case study created for demonstrating Business Analysis skills.

The scenario uses fictionalized business data and does not contain confidential customer, company, or proprietary information.
