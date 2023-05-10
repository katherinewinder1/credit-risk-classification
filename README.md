# credit-risk-classification

## Overview of the Analysis


The purpose of this analysis is to identify the creditworthiness of borrowers. I used various techniques to train and evaluate two models.
The data contains financial information from a peer-to-peer lending service company and I used it to predict whether the loan given had a high risk of defaulting or the loan was healthy. The data included loan size, interest rate, borrower income, a debt to income ratio, number of accounts, derogatory marks, total debt, and loan status for each potential borrower.
The variables I tried to predict were the balance of target values using value_counts on the loan status column from the dataset. This gave me a count of healthy and high-risk loans which I used to train the model and make predictions.
To make my analysis, I went through several stages of the machine learning process. I first split the data into training and test data to avoid overfitting, then I created a logistic regression model using the original data and resampled training data. I fit the data to make predictions, and calculated the accuracy score for the original data and the resampled data. I then created a confusion matrix and a classification report to show the accuracy of each model.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * balanced_accuracy = 0.9918489475856377
  * precision: 0 = 1.00, 1 = 0.85
  * recall: 0 = 0.99, 1 = 0.91

* Machine Learning Model 2:
  * balanced_accuracy = 0.9947308560359688
  * precision: 0 = 0.99, 1 = 0.99
  * recall: 0 = 0.99, 1 = 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* The resampled training model does a better job of predicting the high risk loans.
* In this case it is more important to predict the 1's classification representing high-risk loans since we do not want to increase the number of bad loans given, therefore I would recommend the RandomOverSampler model since it detects more of the potential people who are likely to default on loans based on their credit risk.
