---
title: "Section B: Formal Credit Access"
labels: ["questionnaire", "finance"]
assignees: []
state: open
---

# Section B: Formal Credit Access

## Purpose
Capture farmers' experience with formal credit institutions (banks, cooperatives, government schemes) and assess the role of formal credit in machinery acquisition.

## Proposed Questions

### B1. Ever applied for formal agricultural loan?
- Have you ever applied for a loan from a bank, cooperative, or government scheme for agricultural purposes? (yes/no)
- If yes, which institution(s)? (multiple choice: commercial bank, rural bank, cooperative, government scheme, microfinance institution)
- Year of most recent application.

### B2. Loan approval and terms
- Was the loan approved? (yes/no)
- If approved:
  - Loan amount (local currency)
  - Interest rate (annual percentage)
  - Repayment period (months/years)
  - Collateral required (yes/no, if yes describe)
  - Purpose of loan (multiple: machinery purchase, inputs, land improvement, other)
- If not approved, main reason given by lender (lack of collateral, insufficient income, incomplete paperwork, other).

### B3. Current formal credit status
- Do you currently have an outstanding formal loan for agriculture? (yes/no)
- If yes, remaining balance and monthly repayment amount.

### B4. Satisfaction and constraints
- On a scale of 1 (very difficult) to 5 (very easy), how easy was the application process?
- On a scale of 1 (very dissatisfied) to 5 (very satisfied), how satisfied are you with the terms of the loan (interest rate, repayment period)?
- What are the main barriers to accessing formal credit? (multiple: high interest rates, complex paperwork, lack of collateral, distance to bank, lack of information)

### B5. Government credit schemes
- Are you aware of any government‑subsidized credit schemes for farmers? (yes/no)
- Have you ever used such a scheme? (yes/no)
- If yes, describe the scheme and your experience.

## Notes
- Formal credit is defined as credit from regulated financial institutions.
- If a farmer has never applied, skip B2‑B4.
- Currency amounts should be recorded in local currency; conversion to USD can be done later using historical exchange rates.
- Satisfaction scales should be explained to enumerators to ensure consistent interpretation.

## Linked Variables (for econometric specification)
- `FormalCredit` (binary: 1 if ever applied and approved, 0 otherwise)
- `FormalLoanAmount` (continuous, zero for non‑borrowers)
- `FormalInterestRate` (continuous, missing for non‑borrowers)
- `FormalSatisfaction` (ordinal scale 1‑5)
- `FormalBarriers` (categorical set)