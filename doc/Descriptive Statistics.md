# Descriptive Statistics for Life Expectancy and Related Factors

## Overview
Descriptive statistics provide an initial summary of the dataset, highlighting central tendencies, dispersion, and overall data distribution. This analysis focuses on key factors related to life expectancy.

## Results
- **Mean Life Expectancy**: 72.59 years (Standard Deviation: 7.71 years)
- **Health Expenditure**: Mean = 6.75% (Standard Deviation: 3.08%)
- **Education Expenditure**: Mean = 4.44% (Standard Deviation: 2.24%)
- **Sanitation**: Mean = 58.94% (Standard Deviation: 30.24%)
- **Key Insight**: Higher investments in health, education, and sanitation are correlated with increased life expectancy.

## Code Snippet
```sas
proc means data=mydata.project2 n mean median std min max;
    var Life_Expectancy_World_Bank Prevalence_of_Undernourishment CO2
        'Health_Expenditure_%'n 'Education_Expenditure_%'n Unemployment
        Corruption Sanitation;
    title 'Descriptive Statistics for Life Expectancy and Related Factors';
run;
