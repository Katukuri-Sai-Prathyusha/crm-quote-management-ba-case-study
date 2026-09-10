# As-Is and To-Be Process Analysis

## Project

CRM Quote Management Enhancement

---

## 1. As-Is Process

The current quotation process does not clearly distinguish between standard and optional products.

### Current Process Flow

```text
User Creates Quote
        ↓
Adds Product
        ↓
Enters Quantity and Price
        ↓
System Calculates Line Total
        ↓
Product Contributes to Net Total
        ↓
Quote Generated
Current Process Example
Product	Type	Price	Included in Net Total
Product A	Standard	₹10,000	Yes
Product B	Standard	₹5,000	Yes
Product C	Optional	₹3,000	Yes

Current Net Total = ₹18,000

Problems Identified
No clear distinction between standard and optional products
Optional products are included in the Net Total
Users may need to perform manual calculations
Increased possibility of quotation errors
Additional clarification may be required with customers
2. To-Be Process

The proposed process introduces a product type that allows users to identify products as Standard or Optional.

Proposed Process Flow
User Creates Quote
        ↓
Adds Product
        ↓
Selects Product Type
        ↓
   ┌───────────────┐
   │               │
Standard        Optional
   │               │
   ↓               ↓
Included in     Excluded from
Net Total       Net Total
   │               │
   └───────┬───────┘
           ↓
     Quote Generated
Expected Process Example
Product	Type	Price	Included in Net Total
Product A	Standard	₹10,000	Yes
Product B	Standard	₹5,000	Yes
Product C	Optional	₹3,000	No

Expected Net Total = ₹15,000

3. Process Improvement
Area	As-Is	To-Be
Product Classification	No clear distinction	Standard / Optional
Optional Products	Included in total	Excluded from Net Total
Manual Calculation	May be required	Reduced
Quotation Accuracy	Higher risk of errors	Improved
User Flexibility	Limited	Improved
Customer Clarity	Limited	Improved
4. Business Analyst Analysis

The analysis identifies a gap between the current quotation functionality and the business requirement.

The proposed process addresses the identified gap by introducing product classification and defining clear calculation rules for optional products.

The proposed process should be reviewed and approved by relevant business and product stakeholders before development.
