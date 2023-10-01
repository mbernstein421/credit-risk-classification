# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose the of the analysis was to use supervised machine learning to predict whether a borrower would default on their loan.
* Explain what financial information the data was on, and what you needed to predict.
The financial information used included loan size, interest rates, total debt, and other financial info. We needed to determine the f1 score to find out the percentage that someone might default on their loan.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The basic information about the variables for the value_counts were repaid and defaulted. 
* Describe the stages of the machine learning process you went through as part of this analysis.
First we had to collect and process the data. Then we analyzed the data in order to make a model. We then trained the data and then evaluated the results.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
We used LogisticRegression because of its interpretability and ability to provide probabilities which was needed to predict if someonf would default on their loan. 

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
Classification Report:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     22515
           1       0.85      0.91      0.88       746

    accuracy                           0.99     23261
   macro avg       0.93      0.95      0.94     23261
weighted avg       0.99      0.99      0.99     23261
 * the f1-score had an accuracy of .99, which indicates the model can nearly perfectly predict the risks of loan takers.

 * the precision score for the healthy loans is very high which means the positive predictions were correct, but for the high risk loans the model was only accurate

* for the recall scores, the health loan score of .99, which means it successfully identified 99% of all the instances where someone were they qualified for a healthy loan, but with a .91 score the model was only able to identify 95% of people who qualified for a high risk loan.

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  Classification Report:
              precision    recall  f1-score   support

           0       1.00      0.99      1.00     22515
           1       0.85      0.99      0.92       746

    accuracy                           0.99     23261
   macro avg       0.92      0.99      0.96     23261
weighted avg       0.99      0.99      0.99     23261

 * the f1-score had an accuracy of .99, which indicates the model can nearly perfectly predict the risks of loan takers.

 * the precision score for the healthy loans is very high which means the positive predictions were correct, but for the high risk loans the model was only accurate

 * the recall scores were both very high, which means the model successfully identified people who were qualified for these loans.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
the a Logistic Regression Model with Resampled Training Data was clearlly better because it has a more accurate recall score.
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
Yes it matters since one type of loan is riskier to assess then the other.

If you do not recommend any of the models, please justify your reasoning.
