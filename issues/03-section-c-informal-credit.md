---
title: "Section C: Informal Credit Sources"
labels: ["questionnaire", "finance"]
assignees: []
state: open
---

# Section C: Informal Credit Sources

## Purpose
Document farmers' reliance on informal credit channels (money lenders, input suppliers, rotating savings groups) and assess their role in financing machinery purchases.

## Proposed Questions

### C1. Borrowing from money lenders
- In the past 3 years, have you borrowed money from a local money lender (non‑bank individual)? (yes/no)
- If yes:
  - Approximate total amount borrowed in the last 3 years (local currency)
  - Typical interest rate (per month or per season)
  - Collateral required (yes/no)
  - Main purpose of the loan (machinery, inputs, consumption, emergency, other)

### C2. Input suppliers on credit
- Do you ever obtain seeds, fertilizer, or other inputs on credit from a supplier? (yes/no)
- If yes:
  - Typical credit period (days/months)
  - Is interest charged? (yes/no, if yes approximate rate)
  - Do you pay a higher price for inputs when buying on credit? (yes/no)

### C3. Rotating savings and credit associations (ROSCAs)
- Are you a member of a rotating savings group (e.g., chit fund, merry‑go‑round, susu)? (yes/no)
- If yes:
  - How much do you contribute per cycle?
  - How often does the group meet (weekly, monthly, seasonally)?
  - Have you ever used the lump‑sum payout for agricultural investment? (yes/no)

### C4. Family and friends
- In the past 3 years, have you borrowed from relatives or friends for agricultural purposes? (yes/no)
- If yes, approximate amount and whether interest was charged.

### C5. Reasons for using informal credit
- Why do you prefer informal credit over formal credit? (multiple choice: faster access, less paperwork, no collateral, flexible repayment, lower interest, trust‑based, lack of access to banks)
- On a scale of 1 (very unreliable) to 5 (very reliable), how reliable do you find informal credit sources?

### C6. Repayment experience
- Have you ever defaulted on an informal loan? (yes/no)
- If yes, what were the consequences (social pressure, asset seizure, etc.)?

## Notes
- Informal credit includes any credit arrangement not supervised by a financial regulatory authority.
- Interest rates may be quoted in non‑standard terms (e.g., "10% per season"); enumerators should clarify and convert to annual equivalent if possible.
- For rotating savings groups, distinguish between pure ROSCAs and those that allow borrowing against future contributions.

## Linked Variables (for econometric specification)
- `InformalCredit` (binary: 1 if used any informal source in last 3 years, 0 otherwise)
- `InformalAmount` (continuous, total borrowed from informal sources)
- `InformalInterestRate` (continuous, average if multiple sources)
- `InformalSource` (categorical: money lender, input supplier, ROSCA, family/friends)
- `InformalPreference` (categorical set of reasons)
- `InformalReliability` (ordinal scale 1‑5)