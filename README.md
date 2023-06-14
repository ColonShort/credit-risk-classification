# credit-risk-classification
# Module 20 Report


## Overview of the Analysis

In this analysis, we explored the performance of machine learning models for predicting loan status using financial data. The purpose of this analysis was to develop a model that can effectively classify loans as either healthy or high-risk.

The dataset used in this analysis contained various financial information related to loans. The target variable was the "loan_status," which indicated whether a loan was healthy (0) or high-risk (1).

Here is some basic information about the loan status variable:

Value counts of the loan status variable:
Healthy loans (0): 15,001 instances
High-risk loans (1): 507 instances
To address the class imbalance issue, we employed resampling techniques, specifically the RandomOverSampler from the imbalanced-learn library. This technique increased the representation of the minority class (high-risk loans) by generating artificial samples.

We then applied the logistic regression algorithm to the original and resampled data and evaluated the model's performance using various metrics.

## Results


Machine Learning Model 1: Logistic Regression with Original Data

Balanced Accuracy Score: 0.9521
Precision (0): 1.00
Precision (1): 0.86
Recall (0): 1.00
Recall (1): 0.91


Machine Learning Model 2: Logistic Regression with Resampled Data

Balanced Accuracy Score: 0.9942
Precision (0): 1.00
Precision (1): 0.85
Recall (0): 0.99
Recall (1): 0.99

## Summary

Based on the results, both machine learning models demonstrated strong performance in predicting loan status. However, Model 2, which uses logistic regression with resampled data, outperformed Model 1 in terms of balanced accuracy, precision, and recall for both classes.

In Model 2, the balanced accuracy score was significantly higher (0.9942) compared to Model 1 (0.9521). This shows that Model 2 has a better overall ability to classify both healthy loans and high-risk loans accurately.

Correctly identifying high-risk loans is crucial, I would recommend Model 2. It shows a high precision (0.85) and recall (0.99) for high-risk loans, suggesting its effectiveness in correctly identifying and classifying these loans. The model also maintains high precision (1.00) and recall (0.99) for healthy loans.