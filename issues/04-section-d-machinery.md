---
title: "Section D: Machinery & Input Decisions"
labels: ["questionnaire", "dependent variable"]
assignees: []
state: open
---

# Section D: Machinery & Input Decisions

## Purpose
Define the dependent variable for the Logit model (acquisition of agricultural machinery) and collect details on the type, cost, financing, and perceived impact of the machinery.

## Proposed Questions

### D1. Machinery acquisition (dependent variable)
- In the last 3 years, have you purchased or leased any of the following agricultural machinery? (multiple selection)
  - Tractor
  - Tractor‑trolley
  - Power tiller
  - Combine harvester
  - Thresher
  - Irrigation pump (diesel/electric)
  - Other (specify)
- If *none*, skip to D4.

### D2. Details of acquisition
- For each piece of machinery acquired:
  - Year of purchase/lease
  - New or used?
  - Purchase price or lease cost (local currency)
  - Source of financing (multiple: own savings, formal loan, informal loan, both formal and informal, government subsidy, other)
  - If loan was used, amount borrowed and interest rate.

### D3. Impact and satisfaction
- On a scale of 1 (no impact) to 5 (very large impact), how much has this machinery improved your farming productivity?
- Has the machinery reduced labour requirements? (yes/no)
- Have you been able to increase the area cultivated because of the machinery? (yes/no)
- On a scale of 1 (very dissatisfied) to 5 (very satisfied), how satisfied are you with the machinery investment?

### D4. Future intentions
- Do you plan to purchase or lease additional machinery in the next 3 years? (yes/no)
- If yes, which type and what are the main expected constraints? (lack of credit, high cost, uncertain returns, lack of information)

### D5. Non‑acquisition reasons (for those who did not acquire machinery)
- What are the main reasons for not acquiring machinery in the last 3 years? (multiple: too expensive, no need, lack of credit, uncertain returns, lack of information, other)

## Notes
- The dependent variable `Machinery` is binary: 1 if the farmer acquired **any** of the listed machinery in the last 3 years, 0 otherwise.
- Leasing is included because it reflects access to machinery even without ownership.
- The 3‑year window aligns with typical agricultural investment cycles and reduces recall bias.
- Financing sources should be cross‑referenced with Sections B and C to verify consistency.

## Linked Variables (for econometric specification)
- `Machinery` (binary, from D1)
- `MachineryType` (categorical set)
- `MachineryCost` (continuous, zero for non‑acquirers)
- `FinancingSource` (categorical: own savings, formal, informal, mixed, subsidy)
- `ProductivityImpact` (ordinal scale 1‑5)
- `FutureIntent` (binary)