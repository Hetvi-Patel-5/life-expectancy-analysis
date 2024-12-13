# Frequency Analysis for Income Groups

## Overview
Frequency analysis categorizes countries into income groups to explore their distribution and the relationship between income levels and life expectancy.

## Results
- **Income Group Distribution**:
  - High Income: 32.76%
  - Upper Middle Income: 28.16%
  - Lower Middle Income: 25.86%
  - Low Income: 13.22%
- **Key Insight**: Higher-income groups demonstrate better access to healthcare and services, leading to improved life expectancy.

## Code Snippet
```sas
proc freq data=project2;
    tables Income_Group;
run;
