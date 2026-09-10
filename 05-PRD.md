# Product Requirements Document (PRD)

## Project

CRM Quote Management Enhancement

## 1. Purpose

The purpose of this enhancement is to allow users to identify products within a quotation as either Standard or Optional.

Optional products should remain visible in the quotation but should not contribute to the Net Total.

---

## 2. Business Objective

The enhancement aims to:

- Improve quotation accuracy
- Reduce manual calculations
- Provide flexibility when presenting alternative products
- Clearly distinguish optional products from standard products
- Improve the customer quotation experience

---

## 3. Scope

### In Scope

- Marking products as Standard or Optional
- Displaying product type in the quotation
- Excluding Optional products from Net Total
- Recalculating Net Total when product type changes
- Displaying Optional products in generated quotations
- Supporting multiple Standard and Optional products

### Out of Scope

- Changes to product master data
- Changes to product pricing
- Changes to customer master data
- Changes to tax configuration
- Changes to user authentication
- Changes to unrelated quotation functionality

---

## 4. Functional Requirements

### FR-01 – Product Type

The system shall allow users to identify a quotation product as either:

- Standard
- Optional

### FR-02 – Optional Product Display

The system shall clearly identify Optional products within the quotation.

### FR-03 – Net Total Calculation

The system shall include Standard products when calculating the Net Total.

The system shall exclude Optional products from the Net Total.

### FR-04 – Product Type Change

The system shall allow authorized users to change a product from Standard to Optional and from Optional to Standard.

### FR-05 – Automatic Recalculation

The system shall recalculate the Net Total when the product type is changed.

### FR-06 – Multiple Products

The system shall support quotations containing multiple Standard and Optional products.

### FR-07 – Quotation Output

Optional products shall remain visible in the generated quotation.

---

## 5. Business Rules

| Rule ID | Business Rule |
|---|---|
| BR-01 | Standard products contribute to Net Total. |
| BR-02 | Optional products do not contribute to Net Total. |
| BR-03 | Optional products remain visible in quotations. |
| BR-04 | A quotation can contain both Standard and Optional products. |
| BR-05 | Changing product type triggers Net Total recalculation. |
| BR-06 | Only authorized users can change product type. |

---

## 6. Assumptions

- Existing quotation functionality will continue to work.
- Existing product pricing logic will remain unchanged.
- Existing user permissions will be reused where applicable.
- Optional products will use the same product and pricing information as standard products.
- The enhancement will not change the underlying product master.

---

## 7. Dependencies

The enhancement may depend on:

- Quotation module
- Product module
- Pricing calculation logic
- User permission configuration
- Quotation PDF generation
- Existing tax and discount calculation rules

---

## 8. Acceptance Criteria – High Level

The enhancement will be considered successful when:

1. Users can mark products as Optional.
2. Optional products are clearly identified.
3. Optional products do not contribute to Net Total.
4. Standard products continue to contribute to Net Total.
5. Changing product type recalculates Net Total correctly.
6. Multiple Standard and Optional products are supported.
7. Optional products remain visible in generated quotations.

---

## 9. Success Criteria

The enhancement should reduce manual calculation effort and improve the accuracy and flexibility of quotation creation while meeting the defined business requirements.

---

## 10. Stakeholder Approval

The PRD should be reviewed and approved by relevant business, product, and technical stakeholders before development begins.
