# Econometric Specification

## Logit Model

The probability of machinery acquisition is modeled using a binary Logit model:

```
P(Machinery = 1 | X) = 1 / (1 + e^-(β₀ + β₁·InformalCredit + β₂·FormalCredit + β₃·LandSize + β₄·Education + ... + ε))
```

Where:
- **Machinery** is the binary dependent variable (1 if farmer acquired machinery in reference period, 0 otherwise).
- **X** is a vector of independent variables.
- **β₀** is the intercept.
- **β₁, β₂, ...** are coefficients to be estimated.
- **ε** is the error term.

## Variable Definitions

| Variable Name | Description | Source (Questionnaire Section) | Expected Type |
|---------------|-------------|--------------------------------|---------------|
| **Machinery** | Dummy variable indicating acquisition of agricultural machinery (tractor, tractor‑trolley, etc.) in the last 3 years | Section D | Binary (0/1) |
| **InformalCredit** | Access to informal credit sources (money lenders, input suppliers, rotating savings groups) | Section C | Binary or categorical |
| **FormalCredit** | Access to formal credit (bank loans, government schemes) | Section B | Binary or categorical |
| **LandSize** | Total cultivable land owned/operated (hectares) | Section A | Continuous |
| **Education** | Highest education level of household head | Section A | Categorical (ordinal) |
| **Age** | Age of household head | Section A | Continuous |
| **HouseholdSize** | Number of household members | Section A | Continuous |
| **FarmExperience** | Years of farming experience | Section A | Continuous |
| **CropType** | Main crop grown (categorical) | Section A | Categorical |
| **Irrigation** | Access to irrigation (binary) | Section A | Binary |
| **OffFarmIncome** | Presence of off‑farm income sources | Section A | Binary |
| **Region** | Geographic region (dummy variables) | Section A | Categorical |

## Expected Signs

- **InformalCredit**: Positive (informal credit facilitates machinery purchase).
- **FormalCredit**: Positive (formal credit also facilitates, but may have stricter conditions).
- **LandSize**: Positive (larger farms have greater need/ability to invest).
- **Education**: Positive (higher education may improve awareness and access).
- **Age**: Uncertain (older farmers may be more risk‑averse, but may have more savings).
- **OffFarmIncome**: Positive (additional income reduces liquidity constraints).

## Estimation

The model will be estimated using maximum likelihood. Marginal effects will be computed to interpret the magnitude of each variable's impact on the probability of machinery acquisition.