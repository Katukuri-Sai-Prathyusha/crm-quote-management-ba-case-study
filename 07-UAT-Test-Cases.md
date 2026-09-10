# UAT Test Cases

## Project

CRM Quote Management Enhancement

## Purpose

The purpose of User Acceptance Testing (UAT) is to validate that the quotation enhancement meets the defined business requirements and behaves as expected from the end-user perspective.

---

## UAT Scenarios

### UAT-01 – Add Standard Product

**Objective:**  
Verify that a Standard product is included in the Net Total.

**Precondition:**  
User has access to create or edit a quotation.

**Steps:**

1. Create a new quotation.
2. Add a product.
3. Select product type as Standard.
4. Enter quantity and price.
5. Save the quotation.

**Expected Result:**  
The Standard product is displayed in the quotation and its value contributes to the Net Total.

**Expected Example:**

Product Price = ₹10,000

Net Total = ₹10,000

**Status:** Pass

---

### UAT-02 – Add Optional Product

**Objective:**  
Verify that an Optional product does not contribute to the Net Total.

**Steps:**

1. Create or edit a quotation.
2. Add a product.
3. Select product type as Optional.
4. Enter quantity and price.
5. Save the quotation.

**Expected Result:**  
The Optional product is displayed in the quotation but its value is excluded from the Net Total.

**Expected Example:**

Product Price = ₹3,000

Net Total impact = ₹0

**Status:** Pass

---

### UAT-03 – Standard and Optional Products Together

**Objective:**  
Verify Net Total calculation when both Standard and Optional products exist.

**Test Data:**

| Product | Type | Price |
|---|---|---:|
| Product A | Standard | ₹10,000 |
| Product B | Standard | ₹5,000 |
| Product C | Optional | ₹3,000 |

**Expected Result:**

Net Total = ₹15,000

The Optional product should not contribute to the Net Total.

**Status:** Pass

---

### UAT-04 – Change Standard to Optional

**Objective:**  
Verify that changing a Standard product to Optional recalculates the Net Total.

**Steps:**

1. Open an existing quotation.
2. Select a Standard product.
3. Change the product type to Optional.
4. Save the quotation.

**Expected Result:**  
The product is displayed as Optional and its value is removed from the Net Total.

**Status:** Pass

---

### UAT-05 – Change Optional to Standard

**Objective:**  
Verify that changing an Optional product to Standard recalculates the Net Total.

**Steps:**

1. Open a quotation containing an Optional product.
2. Change the product type to Standard.
3. Save the quotation.

**Expected Result:**  
The product is displayed as Standard and its value is included in the Net Total.

**Status:** Pass

---

### UAT-06 – Multiple Optional Products

**Objective:**  
Verify that multiple Optional products are excluded from the Net Total.

**Test Data:**

| Product | Type | Price |
|---|---|---:|
| Product A | Standard | ₹10,000 |
| Product B | Optional | ₹3,000 |
| Product C | Optional | ₹2,000 |
| Product D | Standard | ₹5,000 |

**Expected Result:**

Net Total = ₹15,000

Both Optional products remain visible but do not contribute to the Net Total.

**Status:** Pass

---

### UAT-07 – Generated Quotation

**Objective:**  
Verify that Optional products remain visible in the generated quotation.

**Steps:**

1. Create a quotation containing Standard and Optional products.
2. Save the quotation.
3. Generate the quotation output/PDF.

**Expected Result:**  
Both Standard and Optional products are displayed, and Optional products are clearly identified.

**Status:** Pass

---

## UAT Summary

| Test Case | Scenario | Expected Result | Status |
|---|---|---|---|
| UAT-01 | Standard Product | Included in Net Total | Pass |
| UAT-02 | Optional Product | Excluded from Net Total | Pass |
| UAT-03 | Standard + Optional | Correct Net Total | Pass |
| UAT-04 | Standard → Optional | Net Total recalculated | Pass |
| UAT-05 | Optional → Standard | Net Total recalculated | Pass |
| UAT-06 | Multiple Optional Products | Correct Net Total | Pass |
| UAT-07 | Generated Quotation | Optional products displayed | Pass |

## UAT Outcome

The defined UAT scenarios validate the core business requirements for the CRM Quote Management Enhancement.

All test scenarios are expected to pass before the enhancement is approved for production implementation.
