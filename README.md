# credit-risk-classification

## Overview
* This analysis aims to predict credit risk for peer-to-peer lending using machine learning techniques.
* The dataset includes various loan attributes such as loan size, interest rate, borrower income, and loan status, with the goal of distinguishing between healthy and high-risk loans.
* The dataset comprises 75,036 healthy loans and 2,500 high-risk loans. Initially, the data was split into training and testing sets, and a logistic regression model was applied.
* Due to class imbalance, a resampled training dataset was generated using RandomOverSampler from imbalanced-learn, and a new logistic regression model was trained on this resampled data.

## Results
* Model 1:

* Balanced Accuracy: 94.4%
* Precision:
* Healthy Loans: 1%
* High-Risk Loans: 87%
* Recall:
* Healthy Loans: 1%
* High-Risk Loans: 89%

* Model 2:
* Balanced Accuracy: 99.6%
* Precision:
* Healthy Loans: 1%
* High-Risk Loans: 87%
* Recall:
* Healthy Loans: 1%
* High-Risk Loans: 1%

## Summary
Both models exhibit strong performance in predicting healthy loans. However, Model 2, which utilized resampled data, demonstrated significant improvements in accuracy and recall, achieving nearly perfect scores. Precision remains consistent at 87% for both models. Given the importance of correctly identifying high-risk loans, Model 2 is recommended due to its enhanced performance in this regard. Misclassifying a healthy loan as high-risk poses lower risks compared to failing to identify a high-risk loan accurately. Therefore, prioritizing high recall for high-risk loans is crucial for effective risk management.





