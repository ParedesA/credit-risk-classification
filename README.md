# credit-risk-classification

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
To determine if a loan is healthy or high-risk.
* 
* Explain what financial information the data was on, and what you needed to predict.
Based on teh following information the model needs to predict if the loan is healthy or high-risk: loan_size,	interest_rate,	borrower_income,	debt_to_income,	num_of_accounts,	derogatory_marks	and total_debt.
* 
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The variable consites on 0 for health and 1 for high-risk loans with a total of 75036 healthy examples and 2500 high-risk examples.
* 
* Describe the stages of the machine learning process you went through as part of this analysis.
After spliting the data between training and testing portions, I created a instance, trained the model using the training data and predicted using the test data. Later I checked for accuracy score and generated a confusion matrix and a classification report to check how well the model was doing.
* 
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
I used a Logistic Regression model
* 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model:
  * Description of Model Accuracy: model accuracy score was 0.95
  * Description of Model Precision: precision for "0 health loan" was 1.00, "1 high-risk" was 0.85
  * Description of Model Recall: recall for "0 health loan" was 0.99, "1 high-risk" was 0.91

 Really good scores overall.

## Summary

Summarize the results of the machine learning model, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s?)

The model perfoms really well and I believe it could be deployed as a first layer to determine if the loan should be considered or not. But since the prediction for "1 high-risk" has a precision of 0.85 I would still have a second layer of avaluation before granting the loan.

If you do not recommend any of the models, please justify your reasoning.

