# Requirement Gathering

## Project

CRM Quote Management Enhancement

## Requirement Gathering Approach

Requirements were gathered through discussions with business users and customers to understand the current quotation process, business needs, pain points, and expected functionality.

The Business Analyst focused on understanding the business problem before defining the solution.

## Key Questions Asked

| # | Question | Business Requirement Identified |
|---|---|---|
| 1 | Why do users need optional products in quotations? | Users need to present alternative products to customers without including them in the final total. |
| 2 | Should optional products be visible in the quotation? | Yes, optional products should remain visible. |
| 3 | Should optional products contribute to the Net Total? | No, optional products should be excluded from the Net Total. |
| 4 | Can a quotation contain both standard and optional products? | Yes. |
| 5 | Should users be able to change a standard product to optional? | Yes. |
| 6 | Should users be able to change an optional product to standard? | Yes. |
| 7 | Should optional products appear in the generated quotation? | Yes. |
| 8 | Should existing quotations be changed automatically? | No, the enhancement should apply to newly updated quotations based on the defined business rules. |

## Business Requirements

### BR-01
The system should allow users to identify a product as Standard or Optional within a quotation.

### BR-02
Optional products should remain visible to users and customers.

### BR-03
Optional products should not contribute to the quotation Net Total.

### BR-04
Users should be able to change the product type between Standard and Optional.

### BR-05
The quotation should clearly distinguish optional products from standard products.

### BR-06
The functionality should work when a quotation contains multiple standard and optional products.

## Business Rules

1. Standard products contribute to the Net Total.
2. Optional products do not contribute to the Net Total.
3. Optional products remain visible in the quotation.
4. A quotation can contain both Standard and Optional products.
5. Users can change the product type when permitted by their access level.
6. Changing a product from Standard to Optional should recalculate the Net Total.
7. Changing a product from Optional to Standard should recalculate the Net Total.

## Example

### Before Enhancement

| Product | Type | Price | Included in Net Total |
|---|---|---:|---|
| Product A | Standard | ₹10,000 | Yes |
| Product B | Standard | ₹5,000 | Yes |
| Product C | Optional | ₹3,000 | Yes |

**Net Total = ₹18,000**

### Expected Behavior After Enhancement

| Product | Type | Price | Included in Net Total |
|---|---|---:|---|
| Product A | Standard | ₹10,000 | Yes |
| Product B | Standard | ₹5,000 | Yes |
| Product C | Optional | ₹3,000 | No |

**Net Total = ₹15,000**

## Requirement Clarifications

During requirement analysis, the following areas should be clarified with stakeholders before development:

- Tax calculation for optional products
- Discounts applicable to optional products
- Display format in quotation PDFs
- User permissions
- Impact on existing quotations
- Reporting and export requirements
- Audit/history requirements
