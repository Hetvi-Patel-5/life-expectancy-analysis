# Regression Analysis: Factors Influencing Life Expectancy

## Overview
Regression analysis was used to quantify the impact of key factors like health expenditure and sanitation on life expectancy.

## Steps Performed
1. Applied linear regression to evaluate relationships between life expectancy and:
   - Health Expenditure
   - Sanitation
   - Other factors like unemployment and undernourishment.
2. Used `PROC REG` in SAS for model fitting and diagnostics.

## Results
- **Health Expenditure**: Each 1% increase raises life expectancy by ~1.21 years (R-squared = 0.1676).
- **Sanitation**: Each unit increase in sanitation raises life expectancy by ~0.18 years (R-squared = 0.4845).

## Interpretation
Investments in health and sanitation significantly improve life expectancy, though other factors like education and undernourishment may play complex roles.

## Code Snippet
```sas
proc reg data=MYDATA.PROJECT2;
   model Life_Expectancy_World_Bank = Health_Expenditure_Sanitation;
   title 'Regression Analysis for Life Expectancy';
run;
quit;
