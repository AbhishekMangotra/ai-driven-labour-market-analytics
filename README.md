# AI-Driven Labour Market Analytics

## Predicting Daily Wages and Identifying Drivers of Wage Inequality in India

An AI for Business project using India's Periodic Labour Force Survey (PLFS) data to analyse wage patterns, working hours, education, occupation and industry differences, and to develop a machine-learning model for daily wage prediction.

## Business Problem

Large labour-market datasets contain valuable information, but converting this information into actionable workforce insights can be challenging.

This project uses Business Analytics and Artificial Intelligence to answer:

- How does education relate to wages?
- How do occupations and industries differ in wages?
- What is the relationship between working hours and wages?
- Can worker characteristics be used to predict daily wages?

## Dataset

- Source: Periodic Labour Force Survey (PLFS), India
- Reference period: January–December 2024
- Original dataset: 415,549 observations × 140 variables
- Main analytical sample: 164,046 observations
- Machine-learning sample: 27,523 observations

## Methodology

1. Data cleaning
2. Feature engineering
3. Exploratory Data Analysis
4. Statistical analysis
5. ANOVA and Tukey HSD
6. Correlation analysis
7. Random Forest regression
8. Business interpretation

## Key Findings

### Industry and Wage

| Industry | Average Daily Wage |
|---|---:|
| Services | ₹509.76 |
| Industry | ₹504.55 |
| Agriculture | ₹348.11 |

Agriculture showed a statistically significant wage difference compared with both Industry and Services.

### Occupation and Wage

- Technicians & Associate Professionals: ₹617.89/day
- Craft & Related Trades Workers: ₹607.38/day
- Plant & Machine Operators: ₹584.08/day
- Skilled Agricultural, Forestry & Fishery Workers: ₹363.12/day

### Working Hours and Wage

Pearson correlation:

**r = 0.102**

This indicates a weak positive relationship between working hours and reported daily wages.

## Statistical Results

- Education → Wage: F = 171.891, p < 0.001
- Industry → Wage: F = 2780.626, p < 0.001
- Education → Working Hours: F = 506.458, p < 0.001

## Machine Learning

Three approaches were compared:

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Mean Baseline | ₹136.10 | ₹185.41 | ~0.000 |
| Basic Random Forest | ₹115.35 | ₹163.05 | 0.227 |
| Expanded Random Forest | ₹108.22 | ₹154.08 | **0.309** |

The expanded Random Forest outperformed the baseline and basic model.

### Most Important Features

1. Average Daily Hours — 23.99%
2. Sex = 2 — 14.26%
3. Agriculture — 10.12%
4. Sex = 1 — 7.78%

Feature importance represents predictive contribution and should not be interpreted as causation.

## Business Recommendations

- Targeted vocational and technical skills development
- Workforce reskilling and occupational mobility
- Data-driven workforce planning
- AI-supported labour-market intelligence
- Focus on productivity and employment quality rather than working hours alone

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- SciPy
- Statsmodels
- Jupyter / Google Colab

## Future Scope

- XGBoost and Gradient Boosting
- SHAP Explainable AI
- Additional PLFS years
- Geographic and employment characteristics
- Power BI / Tableau dashboard

## Disclaimer

This project identifies statistical associations and predictive relationships. It does not establish causal relationships between education, occupation, industry, working hours and wages.
