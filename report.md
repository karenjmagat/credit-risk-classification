# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The goal is to determine if Logistic Regression model can be accurate to predict healthy loans versus high risk loans. Using original data vs. resampled data to increase the size of minority class

* Explain what financial information the data was on, and what you needed to predict.
loan_status is what we needed for predictions

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
original:
value_counts 0- 75036, 1-2500

oversampled  0-56271, 1-56271

* Describe the stages of the machine learning process you went through as part of this analysis.
First stage - prepare data
second stage - separate data to features or columns which X and y is the outcome labels
third stage - train_test_split
fourth stage - Pick the ml model for classification
fifth stage - fit the model with training data 
sixth stage - use model to make predictions with the test data
seventh stage - evaluate the predictions comparing metrics, confusion matrix classifcation report

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
SkLearn Logistic Regression
train_test_split
confusion_matrix
classification_report

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
- Accuracy: 0.99 
- Precision Class 0: 1.00 Class 1: 0.85 
- Recall Class 0: 0.99 Class 1: 0.91



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
- Accuracy: 0.99 
- Precision Class 0: 1.00 Class 1: 0.84 
- Recall Class 0: 0.99 Class 1: 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
OVerall Logisitic Regression Model performed well especially prediction the outcome of 0 healthy loans for class 0. Both precision and recall were high



* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
For 1 class high risk loans the models precision is 0.84 and recall 0.91 not as good as 0 . This indicates the model more often gives false positives than false negatives

If you do not recommend any of the models, please justify your reasoning.
The logistic regression models does a great job at predicting both healthy and high risk loans given the features that used to training the set data.