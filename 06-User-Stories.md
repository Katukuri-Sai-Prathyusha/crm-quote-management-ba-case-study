# User Stories & Acceptance Criteria

## Project

CRM Quote Management Enhancement

---

## User Story 01 – Mark Product as Optional

### User Story

**As a** Sales User  
**I want** to mark a product as Optional within a quotation  
**So that** I can present alternative products without including them in the Net Total.

### Acceptance Criteria

**AC-01:**  
Given the user is creating or editing a quotation,  
when the user adds a product,  
then the user should be able to select the product type as Standard or Optional.

**AC-02:**  
Given a product is marked as Optional,  
when the quotation is displayed,  
then the product should be clearly identified as Optional.

---

## User Story 02 – Exclude Optional Product from Net Total

### User Story

**As a** Sales User  
**I want** Optional products to be excluded from the Net Total  
**So that** the quotation total reflects only the products selected for purchase.

### Acceptance Criteria

**AC-03:**  
Given a quotation contains Standard and Optional products,  
when the system calculates the Net Total,  
then only Standard products should contribute to the Net Total.

**AC-04:**  
Given a quotation contains an Optional product,  
when the quotation total is calculated,  
then the price of the Optional product should not be included in the Net Total.

---

## User Story 03 – Convert Standard Product to Optional

### User Story

**As a** Sales User  
**I want** to change a Standard product to Optional  
**So that** I can present the product as an alternative without including it in the Net Total.

### Acceptance Criteria

**AC-05:**  
Given a product is currently Standard,  
when the user changes the product type to Optional,  
then the product should be marked as Optional.

**AC-06:**  
Given a Standard product is changed to Optional,  
when the quotation is recalculated,  
then the product price should be removed from the Net Total.

---

## User Story 04 – Convert Optional Product to Standard

### User Story

**As a** Sales User  
**I want** to change an Optional product to Standard  
**So that** I can include the product in the final quotation calculation.

### Acceptance Criteria

**AC-07:**  
Given a product is currently Optional,  
when the user changes the product type to Standard,  
then the product should be marked as Standard.

**AC-08:**  
Given an Optional product is changed to Standard,  
when the quotation is recalculated,  
then the product price should be included in the Net Total.

---

## User Story 05 – Display Optional Products in Quotation

### User Story

**As a** Sales User  
**I want** Optional products to remain visible in the quotation  
**So that** customers can see the available alternatives.

### Acceptance Criteria

**AC-09:**  
Given a quotation contains Optional products,  
when the quotation is generated,  
then Optional products should be displayed.

**AC-10:**  
Given a quotation contains Standard and Optional products,  
when the quotation is generated,  
then both product types should be clearly distinguishable.

---

## User Story 06 – Multiple Optional Products

### User Story

**As a** Sales User  
**I want** to add multiple Optional products to a quotation  
**So that** I can provide multiple alternatives to the customer.

### Acceptance Criteria

**AC-11:**  
Given a quotation contains multiple Optional products,  
when the Net Total is calculated,  
then none of the Optional products should contribute to the Net Total.

**AC-12:**  
Given a quotation contains multiple Standard and Optional products,  
when the quotation is generated,  
then all products should be displayed with their correct product type.
