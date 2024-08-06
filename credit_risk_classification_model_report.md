# Module 12 Report

## Overview of the Analysis

The purpose of this analysis was to build and evaluate a logistic regression model to predict the eligibility of borrowers based on historical lending data. The dataset included financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable was `loan_status`, where `0` indicates a healthy loan and `1` indicates a high-risk loan.

The analysis followed these steps:
1. **Data Preparation:** Loaded the dataset and examined its structure and summary statistics.
2. **Data Scaling:** Scaled the features using `StandardScaler` to ensure all variables contribute equally to the model.
3. **Data Splitting:** Split the data into training and testing sets using `train_test_split`.
4. **Model Training:** Trained a logistic regression model on the training data.
5. **Model Evaluation:** Evaluated the model using confusion matrix and classification report on the testing data.

## Results

* **Machine Learning Model 1: Logistic Regression**
  * **Accuracy:** 99%
  * **Precision:**
    * Healthy Loans (0): 100%
    * High-Risk Loans (1): 86%
  * **Recall:**
    * Healthy Loans (0): 99%
    * High-Risk Loans (1): 98%
  * **F1-Score:**
    * Healthy Loans (0): 100%
    * High-Risk Loans (1): 92%

## Summary

The logistic regression model performed exceptionally well in predicting healthy loans with an accuracy of 99%. It showed near-perfect precision and recall for healthy loans, and high precision and recall for high-risk loans. The model is highly effective at identifying both healthy and high-risk loans, although it is slightly less precise for high-risk loans.

**Recommendation:** The logistic regression model is recommended for predicting loan statuses due to its high accuracy and reliability in identifying both healthy and high-risk loans. It is especially important in this context to accurately identify high-risk loans to mitigate potential defaults, and the model achieves this with a recall of 98% for high-risk loans.
