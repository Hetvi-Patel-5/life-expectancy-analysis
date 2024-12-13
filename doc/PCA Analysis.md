**PCA Analysis**

# Principal Component Analysis (PCA)

## Overview
PCA was used to reduce dimensionality and identify key drivers of life expectancy. This analysis helps reveal underlying patterns in socio-economic factors.

## Steps Performed
1. Standardized the dataset to ensure all variables have comparable scales.
2. Conducted PCA using `PROC PRINCOMP` in SAS to extract principal components.

## Results
- **Variance Explained**: The first three components explained 82.57% of the variance.
- **Key Variables**: Health expenditure, education expenditure, and sanitation were the top contributors to the variance.

## Interpretation
The PCA results provide a consolidated view of how socio-economic factors interact to influence life expectancy, enabling targeted interventions.

## Code Snippet
```sas
proc princomp data=MYDATA.PROJECT2 out=pca_out;
   var Life_Expectancy_World_Bank Prevalence_of_Undernourishment CO2
       Health_Expenditure_Education_Expenditure Unemployment Corruption Sanitation;
   title 'Principal Component Analysis';
run;

proc print data=pca_out;
   var prin1 prin2 prin3;
   title 'First Three Principal Components';
run;
