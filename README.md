# Life Expectancy Analysis

## Overview
This repository contains an in-depth analysis of life expectancy and its relationship with socioeconomic and environmental factors. The analysis aims to uncover insights that can inform global health policies and interventions, focusing on trends and disparities observed in 2019.

### Key Features:
- **Techniques Used**: Regression, Canonical Correlation Analysis (CCA), ANOVA, Principal Component Analysis (PCA), and K-Means Clustering.
- **Data Source**: Datasets sourced primarily from Kaggle.
- **Objective**: To identify and analyze the key drivers of life expectancy disparities across regions and income groups.
- **Highlights**: Includes analysis scripts, results, and comprehensive documentation for reproducibility.

## Research Objectives

### Primary Question:
What socioeconomic and environmental factors most significantly impact life expectancy across different regions and income groups in 2019?

### Sub-Questions:
- How do these factors interplay to create disparities in life expectancy?
- What patterns emerge when analyzing countries with similar profiles?

## Analytical Methods

### Statistical Techniques:
- **Descriptive Statistics**: Summarizes key variables such as health expenditure, education expenditure, and sanitation.
- **Correlation Analysis**: Evaluates relationships between variables, e.g., health expenditure and life expectancy.
- **Regression Analysis**: Quantifies impacts of factors like sanitation and health expenditure on life expectancy.
- **ANOVA**:
  - One-Way ANOVA: Examines life expectancy by income group.
  - Two-Way ANOVA: Assesses the interaction between income group and region.
- **PCA**: Reduces dimensionality and identifies main drivers of life expectancy.
- **K-Means Clustering**: Segments countries into clusters based on life expectancy and related factors.

### Visualizations:
- Pie Charts: Illustrate income group distribution.
- Histograms: Show the spread of life expectancy values.
- Regression Plots: Visualize relationships between key variables.
- Correlation Heatmaps: Highlight strengths and directions of relationships.

## Data Source
Primary dataset was sourced from Kaggle. Additional data references may be included for comprehensive analysis.

## Repository Structure

```
LifeExpectancyAnalysis/
├── data/                   # Raw and processed datasets
├── scripts/                # SAS scripts for analysis
├── results/                # Output visualizations and tables
├── docs/                   # Documentation and methodology details
├── README.md               # Project overview and details
```

## Key Findings
- **Health Expenditure**: Positively correlated with life expectancy; a 1% increase raises life expectancy by ~1.21 years.
- **Sanitation**: Strong positive correlation; each unit increase raises life expectancy by ~0.18 years.
- **Education Expenditure**: Negligible direct impact on life expectancy.
- **CO2 Emissions**: Highlighted disparities, with countries like China and the USA as significant contributors.
- **Clusters Identified**: Five distinct groups based on life expectancy and socioeconomic profiles.

## How to Use This Repository

### Prerequisites:
- SAS software or SAS Studio for running scripts.
- Basic understanding of data analysis techniques.

### Steps:
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/LifeExpectancyAnalysis.git
   ```
2. Navigate to the `scripts/` directory and run SAS programs.
3. View results in the `results/` directory.
4. Refer to the `docs/` folder for detailed methodology.

## Contribution
Contributions are welcome! Please fork this repository and submit a pull request for improvements or feature additions.

## License
This project is licensed under the [MIT License](LICENSE).

---

For further information or queries, please contact [patelhetvij@gmail.com].
