# Credit-Risk-Analysis

## Problem Statement
Banks lend money to customers in the form of personal loans, home loans etc. and credit cards. Not all of them pay it back on time. Your goal is to - 
- identify which customers are likely to default.
- understand why defaults happen
- help reduce risk and losses

## Tools used
  -  Python (data cleaning, EDA, modelling)
  -  Statistics (Correlation, distributions)
  -  Business thinking
  -  Data Story-telling

## Dataset used

Lending club dataset (kaggle)

## Key Questions to be asked
  - Who is the customer?
  - What is default?
  - What happens if we approve risky loans.

## Exploratory Data Analysis

![Graphs Preview](https://github.com/sidhmen09/Credit-Risk-Analysis/blob/main/eda_analysis.png)

## Feature Engineering

Created new features:
  - Income Bucket
  - Credit Grade
  - Loan to Income Ratio
  - Credit Utilization

## Risk Prediction Model
Feature Importance (Top Risk Factors):
- credit_score : -0.204981
- employment_length : -0.135958
- Interest_rate : 0.078437
- loan_term : -0.077110
- dti : 0.02724
- credit_utilization : -0.018891
- loan_amount : 0.014986
- annual_income : -0.009988
- open_credit_lines : -0.003429
- loan_to_income : -0.001277

## Model Evaluation

![Graphs Preview](https://github.com/sidhmen09/Credit-Risk-Analysis/blob/main/model_evaluation.png)

## Key Findings
- ### Interest Rate impact
    - Customers with interest rate > 15%: 6.4% default rate
    - Customers with interest rate ≤ 15%: 3.4% default rate
    - High rates are 1.86x more likely to default.
- ### Income Level impact
    - Low income (<$50K): 3.5% default rate
    - Higher income (≥$50K): 3.4% default rate
    - Low income customers are 1.02x more risky.
- ### Employment Stability
    - Correlation with default: -0.021
    - Longer employment history reduces risk
- ### Credit Utilization
    - Low utilization (0-30%): 3.5% default
    - High utilization (50-100%): 3.2% default

## Business recomendations
- ### Implement risk-based pricing adjustments for high-risk segments
- ### Require additional documentation for customers with DTI > 35%

## Portfolio Risk Summary
- ### Total Loan Portfolio : $499,380,032
- ### At-Risk Exposure : $17,439,109 (3.5%)
