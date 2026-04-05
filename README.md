# Credit-Risk-Model-Probability-of-Default
Credit Risk Model – Probability of Default
## Project Overview
This project focuses on building a machine learning model to predict the probability of default (PD) for unsecured personal loans. The goal is to support better risk assessment and decision-making in consumer finance.

## Objective
- Build a classification model to predict default risk  
- Evaluate model performance using appropriate metrics  
- Generate probability predictions for unseen data  

## Dataset
The dataset consists of loan applications with features related to:
- customer financial behavior  
- credit history  
- loan characteristics  

Target variable:
- TARGET (1 = default, 0 = non-default)

## Approach

### Data Preprocessing
- Handling missing values  
- Converting data types  
- Feature engineering  
- Log transformation for skewed variables  

### Exploratory Data Analysis (EDA)
- Distribution analysis  
- Missing values analysis  
- Correlation analysis  

### Feature Selection
- Based on ROC-AUC of individual features  
- Removal of highly correlated variables  
- Business logic consideration  

## Models

### Logistic Regression
- Baseline model  
- Interpretable  

### LightGBM
- Main model  
- Handles non-linear relationships  
- Better performance  

## Evaluation Metrics
- ROC-AUC ≈ 0.81  
- KS Statistic ≈ 0.48  
- Cross-validation used for stability  

## Calibration
- Calibration curve used to evaluate probability quality  
- Model shows good overall calibration with minor deviations  

## Output
Final predictions generated for test dataset:

pd_predictions.csv

Contains:
- probability of default for each observation  

## Key Insights
- Credit behavior variables are strong predictors  
- Feature engineering significantly improves performance  
- Tree-based models outperform linear models  

## Tech Stack
- Python (pandas, numpy, sklearn, lightgbm)  
- Jupyter Notebook  
- Matplotlib / Seaborn  
