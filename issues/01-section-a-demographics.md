---
title: "Section A: Household & Farm Demographics"
labels: ["questionnaire", "demographics"]
assignees: []
state: open
---

# Section A: Household & Farm Demographics

## Purpose
Collect basic socio‑economic and farm‑characteristic variables that serve as control variables in the Logit model.

## Proposed Questions

### A1. Household head characteristics
- Age (in years)
- Gender (male, female, other)
- Highest education level (none, primary, secondary, tertiary)
- Years of farming experience

### A2. Household composition
- Number of household members
- Number of working‑age adults (15‑64 years)
- Number of children (<15 years)

### A3. Farm characteristics
- Total cultivable land owned (hectares)
- Total cultivable land operated (including leased/rented) (hectares)
- Main crop(s) grown (multiple selection: rice, wheat, maize, vegetables, fruits, other)
- Access to irrigation (yes/no)
- If yes, source of irrigation (tube well, canal, rainwater harvesting, other)

### A4. Income diversification
- Does any household member have off‑farm employment? (yes/no)
- If yes, type of off‑farm work (casual labour, salaried job, self‑employment)
- Approximate share of household income from off‑farm sources (<25%, 25‑50%, >50%)

### A5. Asset ownership
- Owns a smartphone (yes/no)
- Owns a motorcycle/scooter (yes/no)
- Owns livestock (yes/no, if yes list types)

## Notes
- All questions are mandatory.
- Land size should be recorded in local units with a conversion factor to hectares documented.
- Education levels should be mapped to ISCED categories for cross‑country comparability.
- Off‑farm income is a potential confounder for credit access and machinery investment; capture as precisely as possible.

## Linked Variables (for econometric specification)
- `LandSize` (continuous)
- `Education` (categorical ordinal)
- `Age` (continuous)
- `HouseholdSize` (continuous)
- `FarmExperience` (continuous)
- `Irrigation` (binary)
- `OffFarmIncome` (binary)
- `Region` (categorical, from sampling frame)