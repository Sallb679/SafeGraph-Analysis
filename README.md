# SafeGraph-Analysis
# Restaurant Chain Data Analysis Project

## Project Overview

This project analyzes weekly customer visit patterns for a restaurant chain and compares its performance against a benchmark competitor. The goal is to understand visitation trends, compare weekday vs weekend traffic, and explore factors influencing relative performance using basic data analysis and regression techniques.

---

## Repository Contents

### File 1: Data Summary and Concatenation  
- Counts total observations across five yearly datasets (2018-2022) without concatenating full datasets initially.  
- Identifies the unit of observation as weekly visits per restaurant.  
- Filters data to only include observations for the focal restaurant chain and concatenates these filtered yearly subsets into a combined dataset.  

### File 2: Histogram Visualization of Daily Visits  
- Plots a histogram of daily customer visits with custom bin ranges to address skewness in the data.  
- Provides clear axis labels and explanations for bin choices.  
- Includes a grouped histogram comparing daily visits distribution on weekdays vs weekends, with commentary on observed differences.  

### File 3: Benchmark Chain Selection and Data Preparation  
- Selects “Cracker Barrel” as the benchmark restaurant chain for comparison.  
- Explains the rationale for this choice (largest competitor in the casual dining sector).  
- Filters and concatenates relevant data for the benchmark chain for analysis alongside the focal chain.  

### File 4: Dependent Variable Definition and Regression Summary  
- Defines the dependent variable as the log-difference in total weekly visits between the focal chain and benchmark chain.  
- Summarizes relevant independent variables including day-of-week, demographics, and state political leanings.  
- Reports model results from Ridge and LASSO regressions, including penalty parameters, coefficients, R-squared values, and feature importance.  
- Concludes Ridge regression (α = 1.0) performs best, balancing prediction accuracy and feature retention.  

---

## How to Use

1. Load the zipped datasets for each year (2018-2022) and filter by your chosen restaurant chain.  
2. Explore visit patterns via histogram visualizations.  
3. Define the performance measure relative to the benchmark chain using log differences in weekly visits.  
4. Conduct regression analysis to identify key predictors of relative performance.  

---

## Dependencies

- Python 3.x  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- tabulate  

