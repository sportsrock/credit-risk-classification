# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

In this analysis, the purpose was to develop machine learning models for credit risk analysis. The goal was to predict whether a loan is a healthy loan (0) or a high-risk loan (1) based on financial data. The dataset provided information on various financial attributes, and the task was to build and evaluate machine learning models that could classify loans into these two categories. The primary focus was on addressing class imbalance and evaluating model performance.

Key Information about the Analysis:

Purpose: Credit risk analysis to predict loan status.
Data: Financial information, including attributes like loan amount, interest rate, annual income, and more.
Target Variable: loan_status, where 0 represents healthy loans and 1 represents high-risk loans.
Stages of the Machine Learning Process: Data preprocessing, data splitting, model training and evaluation, resampling using the RandomOverSampler, and assessing model performance.
Methods: Logistic Regression models and RandomOverSampler for class imbalance correction.




## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

Machine Learning Model 1 (Original Data):
Balanced Accuracy Score: 0.9521352751368186
Precision for Healthy Loan (0): 1.00
Recall for Healthy Loan (0): 1.00
Precision for High-Risk Loan (1): 0.86
Recall for High-Risk Loan (1): 0.91
Machine Learning Model 2 (Resampled Data):
Balanced Accuracy Score: 0.9941749445500477
Precision for Healthy Loan (0): 1.00
Recall for Healthy Loan (0): 0.99
Precision for High-Risk Loan (1): 0.85
Recall for High-Risk Loan (1): 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )


In summary, both machine learning models demonstrated strong performance, but Model 2, which used resampled data, outperformed Model 1. Model 2 achieved a significantly higher balanced accuracy score and better overall precision and recall for both healthy and high-risk loans. This improved performance can be attributed to addressing class imbalance through oversampling.

Recommendation:

Model 2 (Logistic Regression with Resampled Data) is recommended for credit risk analysis. It performs exceptionally well in accurately predicting both healthy and high-risk loans, with a balanced accuracy score of approximately 0.994.
Performance Dependence:

The performance of the model does depend on the problem we are trying to solve. For credit risk analysis, it is crucial to predict both healthy and high-risk loans accurately. Model 2 excels in this regard, making it the preferred choice for this specific problem.
In this case, Model 2 should be used for credit risk analysis due to its superior performance and its ability to provide better protection against misclassifying high-risk loans, which is critical in financial risk assessment.