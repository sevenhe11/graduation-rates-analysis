# Factors Associated with Six-Year College Graduation Rates in the U.S.

Course project for PSTAT 100 (Data Science Principles), UC Santa Barbara, Spring 2026.

**Team:** Ke Chen, Huiyue Deng, An (Sean) Xie, Yuxiang He, Zeyu Huang

**My role:** I led the modeling and results section, including regression modeling, model comparison, multicollinearity checks, diagnostics, and final model selection.

## Overview

This project examines which institutional characteristics are associated with six-year bachelor's graduation rates at U.S. four-year public and private nonprofit institutions, using IPEDS 2023 data from the National Center for Education Statistics.

## Data

- Source: Integrated Postsecondary Education Data System (IPEDS), 2023 collection year
- Raw extract: 2,392 institutions, 92 variables
- Final analysis sample: 1,423 institutions after sample restriction and complete-case deletion

The raw CSV is not included in this repository. It can be downloaded from the [IPEDS Data Explorer](https://nces.ed.gov/ipeds/).

## Methods

- Data cleaning, variable selection, and exploratory data analysis
- Three nested multiple linear regression models (3, 5, and 11 predictors)
- Model comparison using adjusted R² and residual standard error
- Multicollinearity check with variance inflation factors (VIF)
- Diagnostics: residuals vs. fitted, normal Q-Q plot, leverage, and Cook's distance

## Key Findings

- The selected five-predictor model explains about 60% of the variation in graduation rates (adjusted R² = 0.599).
- Higher total price is associated with higher graduation rates; higher admission rates and higher Pell Grant percentages are associated with lower graduation rates.
- Each one-point increase in the share of Pell Grant recipients is associated with a 0.42-point decrease in graduation rate, holding other variables constant.
- Results are associational, not causal.

## Tools

Python (pandas, NumPy, matplotlib, seaborn, SciPy), Jupyter Notebook
