# Module 12 Report Template Butler

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
-The purpose of the analysis was to determine/identify creditworthiness of borrowers.
* Explain what financial information the data was on, and what you needed to predict.
-The financial information the data was on was the loan size, income of the borrower, interest rate, debt to income, and total debt. I needed to predict in the model how credit worthy was the borrower based on the information in the dataset.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
-The variable used when trying to predict was loan_status.value_counts to get a better idea of the amount of loans the company would consider.
* Describe the stages of the machine learning process you went through as part of this analysis.
-The stages of machine learning process I went through was spliting the data into training and testing sets, then, creating a logistic regression model.  
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
-I used the LogisticRegression model as it was an algorithm that accomplishes binary classification tasks by predicting the probability and the analysis of creditworthiness is more of a probability based decision.
## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.
        -Accuracy score was .99 - which is almost perfect,indicating that the model performs very well overall in predicting both positive and negative cases.
        -Precision score was 1 or 100% for healthy loans(0); which shows the model has 100% positive instances of healthy loans.  It is .84 or 84% for high-risk loans (1), which shows that it .16 false positives instances for high-risk loans.
        - Recall score for healthy loans was .99 or 99%, which is shows that the model is almost perfect at identifying healthy loans. It is .94 when predicting high-risk loans, indicating the model correctly identified 94%.
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
-I only did the logistic regression.  I do believe it it the best choice as it had the accuracy score of .99, precision score for healthy loans of 100%, and a recall score of 99%.  All of which proved the model does well in predicting healthy loans.  It could be better in predicting high-risk loans as the precision score was .84 but it is still relatively reliable in predicting positives.

* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
-I think to a certain extent that the performance depends on the problem because the company is trying to avoid high-risk while predicting healthy loans.  In the model healthy loans had more positive instances than high-risk. However, the overall model's accuracy is 99% which is pretty good in terms of predicting healthy loans. 

-I do recommend the logistic regression model because it had an accuracy score of .99 and in predicting healthy loans the recall score was .99 and precision score 100%.  I would warn the decision makers that the model could be improved for high-risk loans but it's still reliable.