# Two-Way ANOVA: Life Expectancy by Income Group and Region

## Overview
The Two-Way ANOVA examines the interaction effects between income group and geographical region on life expectancy. This method accounts for both independent and combined effects of these factors.

## Steps Performed
1. Grouped countries by income and region.
2. Used the `PROC GLM` procedure to model life expectancy as a function of both factors and their interaction.

## Results
- **Overall Model Fit**: F-value of 33.58, with a strong R-squared of 0.8159.
- **Significance**: Interaction effects between income group and region were statistically significant.

## Interpretation
The results highlight the complexity of socio-economic and geographical factors influencing life expectancy. Certain regions within the same income group showed significant variability.

## Code Snippet
```sas
proc glm data=PROJECT2;
    class Income_Group Region;
    model Life_Expectancy_World_Bank = Income_Group Region Income_Group*Region;
    lsmeans Income_Group*Region / slice=Income_Group pdiff adjust=tukey;
    title "Two-Way ANOVA for Life Expectancy by Income Group and Region";
run;
quit;
