# credit-risk-classification
## Overview of the Analysis
The purpose of this analysis is to train and evaluate a model based on loan risk. I used a dataset of historical lending activity from a lending services company to build a model which can determine the creditworthiness of loan borrowers. The model is supposed to predict the loan_status of borrowers to determine if they giving them a loan would be a healthy loan, `0`, or a high-risk loan, `1`. 

`y.value_counts() : `
`0    75036`
`1     2500`
`Name: loan_status, dtype: int64`

### Stages of Machine Learning Process
1. Split the Data:
   * First, I split the dataset into training and testing sets to evaluate the performance of the model.
2. Train the Model:
   * I initialized the Logistic Regression Model with the dataset to predict the classification as high risk or low risk.
   * Then, I used the training data in order to fit the model to the data
3. Confusion Matrix and Clasification report
   * In order to evaluate the performance of the model, I generated a confusion matrix
   * Then, I made a classification report in order to show how well the model performed.

The main method used was the Logistic Regression Model which was trained with the dataset to assess and classify loan risk status. 

## Results
* Machine Learning Model 1:
  * For Healthy Loans, `0`, the Logistic Regression Model has a precision of 100%. This indicates that all of the predictions for healthy loans were correct. For High-risk loans, `1`, the precision is 87% which shows that less predictions for high-risk loans were correct.
  * The recall for Healthy loans was also 100% while the recall for High-risk loans was 89%. Recall indicates when this label was correctly identified; so this model predicts recall better for Healthy loans than High-risk loans.
  * The model accuracy was 0.99, showing that the model was correctly loaning loan risk 99% of the time. 

## Summary
The Logistic Regression model performed well with an overall accuracy of 99%. Additionally, the model was perfectly predicting the healthy loans. The model is predicting the healthy loans as healthy loans every time, but is sometimes predicting high-risk loans as healthy loans. It is important to identify the healthy loans so lenders know when a borrower is safe to lend to. It would be helpful to improve the model in order to increase the precision and recall for high-risk loans in order to ensure that lenders aren't giving loans to borrowers with high-risk. 
