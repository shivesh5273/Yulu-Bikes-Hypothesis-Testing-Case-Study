# 🚴 Yulu Bikes — Hypothesis Testing Case Study

## Overview
Statistical analysis to identify factors affecting demand 
for shared electric cycles in the Indian market.

## Business Problem
Yulu, India's leading micro-mobility provider, has suffered 
considerable revenue dips. This project uses hypothesis 
testing to determine which variables significantly affect 
cycle rental demand.

## Dataset
- 10,886 rows × 12 columns
- Hourly bike rental data
- Target variable: count (total rentals)

## Tools & Libraries
- Python, Pandas, NumPy
- Matplotlib, Seaborn
- SciPy (Stats)

## Steps Covered
1. Data Preprocessing & Type Conversion
2. Missing Values & Duplicate Check
3. Skewness & Kurtosis Analysis
4. Univariate Analysis (Histograms, Countplots, Boxplots)
5. Bivariate Analysis (Correlation Heatmap)
6. Hypothesis Testing

## Hypothesis Testing Results

| Test | Question | p-value | Decision |
|------|----------|---------|----------|
| 2-Sample T-Test | Working Day → Count? | 0.2264 | Fail to Reject H0 |
| One-Way ANOVA | Weather → Count? | 0.0000 | Reject H0 ✅ |
| One-Way ANOVA | Season → Count? | 0.0000 | Reject H0 ✅ |
| Chi-Square | Weather ~ Season? | 0.0000 | Reject H0 ✅ |

## Key Findings
- Working day does NOT significantly affect demand
- Weather DOES significantly affect demand
- Season is the STRONGEST predictor (F=236.94)
- Weather and Season are significantly associated

## Business Recommendations
- Deploy maximum bikes during Fall season
- Reduce fleet during Spring to cut idle costs
- Monitor weather forecasts for daily fleet planning
- Deprioritise working day as a demand predictor
