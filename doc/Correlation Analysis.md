# Correlation Analysis Between Life Expectancy and Expenditures

## Overview
Correlation analysis measures the strength and direction of relationships between life expectancy and key factors like health and education expenditure.

## Results
- **Health Expenditure**: Correlation with life expectancy = 0.4094 (Moderate Positive).
- **Education Expenditure**: Correlation with life expectancy = -0.00278 (Negligible).
- **Key Insight**: Investments in healthcare significantly impact life expectancy, while the relationship with education expenditure is negligible in this dataset.

## Code Snippet
```sas
ods noproctitle;
ods graphics / imagemap=on;

proc corr data=MYDATA.PROJECT2 pearson nosimple noprob plots=none;
	var 'Health_Expenditure_%'n 'Education_Expenditure_%'n;
	with Life_Expectancy_World_Bank;
run;
