# Seasonal Agriculture Performance Analysis

## IBM SkillsBuild – Data Analytics with AI | Academic Project

**Author:** Siddhi Chavan

## Project Overview

This project analyzes agricultural activities across seasons, geographical areas, crops, irrigation methods, environmental conditions, resource usage, and economic outcomes. The objective is to identify seasonal patterns, relationships, variations, and evidence-based insights that can support better agricultural planning.

## Problem Statement

Agricultural performance can vary with seasonal environmental conditions, farming practices, resource availability, and market conditions. This project investigates how agricultural performance changes across **Kharif, Rabi, and Zaid** seasons and identifies meaningful patterns, relationships, and variations in the supplied dataset.

## Objectives

- Explore and understand the dataset.
- Clean and prepare the data for analysis.
- Compare agricultural performance across seasons.
- Investigate environmental and resource relationships with outcomes.
- Compare crops, irrigation methods, and regions.
- Identify significant differences and unusual patterns.
- Apply appropriate statistical and visualization techniques.
- Interpret findings and develop data-driven recommendations.

## Dataset

**Dataset file:** [seasonal_agriculture_performance_dataset.csv](./seasonal_agriculture_performance_dataset.csv)

The supplied dataset contains **4,000 records and 28 columns**, covering:
- 3 seasons: Kharif, Rabi, Zaid
- 8 states
- 8 crops
- 4 irrigation methods
- Environmental, agricultural, resource, production, and economic variables

The dataset is included separately with the project submission/repository.

## Technologies Used

- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- SciPy

## Analysis Performed

1. Dataset inspection and structure analysis
2. Missing-value and duplicate checks
3. Data cleaning and preparation
4. Seasonal performance comparison
5. Crop × season analysis
6. Irrigation-method analysis
7. Regional/state comparison
8. Spearman correlation analysis
9. Kruskal–Wallis statistical tests
10. Chi-square test of independence
11. Visualization and interpretation
12. Conclusions and recommendations

## Data Cleaning

- Missing **Rainfall** values are imputed using season-level medians.
- Missing **Soil Moisture** values are imputed using season-level medians.
- Missing **Yield** values are imputed using crop-season medians.
- Duplicate rows are checked.
- Core numeric fields are checked for negative/impossible values.
- `Profit_Margin_pct` is derived from profit and revenue.

## Key Findings

- Kharif has the highest average yield at approximately **5.64 t/ha** and the highest average profit at approximately **₹178,915**.
- Rabi has an average yield of approximately **5.08 t/ha** and average profit of approximately **₹87,689**.
- Zaid has the lowest average yield at approximately **4.67 t/ha** and negative average profit of approximately **₹24,805**.
- Seasonal differences in yield, profit, water efficiency, and disease/pest risk are statistically significant in the analysis (**Kruskal–Wallis, p < 0.001**).
- Profitability status is associated with season in the analyzed data (**chi-square, p < 0.001**).
- Drip has the highest average yield among irrigation methods in Kharif and Rabi, while Sprinkler has the highest average yield in Zaid.
- Regional performance varies across states, indicating that seasonal planning should account for location-specific conditions.
- Correlation results show associations among environmental/resource variables, yield, water efficiency, and profit. These associations should not be interpreted as causal effects.

## Setup and Run Instructions

1. Keep the notebook and dataset in the same folder.
2. Install Python 3.x.
3. Install the required dependencies:

```bash
pip install -r requirements.txt
```

4. Start Jupyter Notebook:

```bash
jupyter notebook
```

5. Open:

`Siddhi_Chavan_Seasonal_Agriculture_Performance_Analysis.ipynb`

6. Run the notebook cells from top to bottom.

The notebook loads the dataset using:

```python
pd.read_csv("seasonal_agriculture_performance_dataset.csv")
```

## Project Files

```text
.
├── Siddhi_Chavan_Seasonal_Agriculture_Performance_Analysis.ipynb
├── seasonal_agriculture_performance_dataset.csv
├── requirements.txt
├── Siddhi_Chavan_ProjectReport.docx
└── README.md
```

## Statistical Methods

### Spearman Correlation
Used to examine monotonic relationships between selected environmental, resource, yield, profit, and risk variables.

### Kruskal–Wallis Test
Used to test whether distributions differ across the three seasons without assuming normality.

### Chi-square Test of Independence
Used to examine the association between season and profitability status (profitable vs. non-profitable).

**Important:** Statistical significance and correlation describe patterns in the supplied data. They do not by themselves establish causation.

## Future Scope

- Add multi-year historical agricultural data.
- Include market-price and weather forecasts.
- Develop predictive models for yield and profitability.
- Add interactive dashboards using Power BI or Tableau.
- Incorporate district-level and farm-level time-series analysis.
- Validate analytical findings with domain experts and additional datasets.

## Dataset Link

The dataset used for this project is included as a project file:

[Open the dataset](./seasonal_agriculture_performance_dataset.csv)

## Author

**Siddhi Chavan**

## Project Context

Prepared for **IBM SkillsBuild – Data Analytics with AI** academic project submission.
