# One-Way ANOVA Analysis

## Overview
One-Way ANOVA (Analysis of Variance) is a statistical method used to determine if there are significant differences between the means of three or more independent groups. In this analysis, we examined how income groups influence life expectancy.

## Steps Performed
1. **Data Preparation**:
   - Grouped countries by income levels (Low, Lower-Middle, Upper-Middle, High).
   - Verified data quality to ensure no missing values for income group or life expectancy.

2. **SAS Procedure**:
   - Used the `proc anova` procedure to perform the analysis.
   - Specified income group as the categorical independent variable and life expectancy as the dependent variable.

   ```sas
   proc anova data=MYDATA.PROJECT2;
       class Income_Group;
       model Life_Expectancy_World_Bank = Income_Group;
       title 'ANOVA for Life Expectancy by Income Group';
   run;
   ```

3. **Results Visualization**:
   - Plotted mean life expectancy for each income group.

## Results
- **Overall Model Fit**:
  - Significant F-value: Indicates differences in life expectancy across income groups.
  - P-value: < 0.05, confirming statistical significance.

- **Key Observations**:
  - Higher-income groups tend to have higher life expectancy.
  - Low-income groups exhibit significantly lower averages.

## Interpretation
The results suggest that income level is a strong determinant of life expectancy. Policymakers should focus on addressing disparities in healthcare access and quality in lower-income regions.
