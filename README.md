# Loan Repayment Risk Assessment (MoneyLion) (Technical Assessment)

## Overview
This project aims to assess the risk of MoneyLion loan applicants by predicting the likelihood of loan default. The analysis is performed on the provided dataset, and a machine learning model is developed to aid MoneyLion in making more informed lending decisions. The final model chosen is a Random Forest classifier.

## Table of Contents
- Chapter 1: Introduction
- Chapter 2: Setup
- Chapter 3: Exploratory Data Analysis (EDA)
- Chapter 4 Feature Engineering
- Chapter 5: Data Visualization
- Chapter 6: Model Development
- Chapter 7: Conclusion

## Data Preprocessing
- Data cleaning and transformation were performed on the `loan.csv` and `clarity_underwriting_variables.csv` datasets.
- Several irrelevant columns were dropped to prevent target leakage.
- Missing values were handled using appropriate techniques like median and mode imputation.

## Feature Engineering
- New features were engineered, including `time_apply_to_originate` which measures the time between application and loan origination.
- Categorical variables were encoded using ordinal and one-hot encoding.

## Model Development
- Four models were evaluated: Logistic Regression, Support Vector Machine (SVM), Decision Tree, and Random Forest.
- The Random Forest model was selected based on its superior ROC-AUC score.
- Class imbalance was addressed using oversampling techniques.

## Results
- The top factors influencing loan default risk include:
  1. Time taken from application to origination.
  2. Originally Scheduled Payment Amount.
  3. Clear Fraud Score.
  4. APR.
  5. Loan Amount.

## Future Work
- Further feature engineering could be conducted to enhance the model.
- Explore the `payment.csv` dataset for additional insights, while carefully avoiding target leakage.
- Include more data on applicants' financial backgrounds, such as income and credit score, to improve model accuracy.
