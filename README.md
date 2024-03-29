# Credit Risk Classification Report

## Overview of the Analysis

The purpose of this analysis was to test if our training model was predicting credit risk well by using the Logistic Regression model. The data consisted of loan sizes, interest rates, borrower income, debt to income ratio, number of accounts, derrogatory marks, total debt and loan status of customers. The data was split into labels and features. Labels being the loan status and features were everything else. This was to predict if the loan was healthy or if it was a high risk loan. 

These following steps were taken to create machine learning for this dataset. To start, the data must be split into labels and features, which are y and X respectively. Then the data is futher split into X training, X testing, y training, and y testing categories using train_test_split from sklearn. The train_test_split categories were then fitted to the Logistic Regression model from sklearn. Predictions were then made on the X test category using the predict function. 

A confusion matrix was generated using the y test category and the predictions. This matrix predicts the true negatives, false positives, false negatives and true positives. A classification report was then printed to show the precision, recall, f1 score, support, accuracy etc.

## Results

Linear Regression Model(binary outcomes)
-precision score: false positives (high precision score = low false positives)
-recall score: false negatives (high recall score = lower false negatives)
-accuracy score: ratio of correctly predicted observations to total number of observations

Healthy loans
-precision score: 1
-recall score: 1
-support: 18759

High risk loans
-precision score: 0.87
-recal score: 0.89
support: 625

accuracy score: 0.99

## Summary

The Linear Regression model used did a fairly decent job at predicting if the loan was healthy or high risk overall, with an accuracy score of 99%. But when you break it down and look at the precision and recall scores, the model is predecting healthy loans better than high risk loans. I would not recommend to use this model quite yet, as it can be improved. One way of improvement would be to balance the high risk loan data vs healthy loan data, either by including more high risk loan data or decreasing healthy loan data.Yes, performance does depend on the problem we are trying to solve. I think that it is more important to predict the 1's(high risk loans) for this model because those loans may default and the lender may end up losing money.