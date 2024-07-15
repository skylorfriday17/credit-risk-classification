# Module 12 Report Template

## Overview of the Analysis

In this analysis the intended insight was to teach a machine learning algorithm to identify what kind of borrowers for a lending service are high-risk or untrustworthy based on the given 'loan_status'. We want to be able to identify what people would be high-risk borrowers in the future. Data aspects of borrowers that were observed are things such as loan size, interest rate, income, debt to income ratio, total debt, etc. Based on this information we wanted the algorithm to predict whether a loan was a healthy or high risk loan based on the borrowers financial information. Loan status in this case is what we are trying to predict on future loans so that we can decrease the amount of defaulting. It is in our best interest to give loans to people with qualities that indicate healthy loan status rather than those that are high-risk and have less likelihood in paying the loan back on time or at all.

The stages in which we progressed to get to the prediction at the end included:
Preprocessing Data, identifying the outcome from the input data, train the machine learning model with 75% of the data, predict with the 25% test data, assess results and accuracy of the model. Within this process we used the LogisticRegression algorithm function which is a statistical method that is used to predict binary outcomes out of a multi-variable data input to classify future borrowers.


## Results

* Confusion Matrix Report:
    * With the confusion matrix report we could tell that the amount of True Positives and True Negatives in the results highly outweighed the False Negatives and Positives. With this information we can say that the model does a good jo of predicting loan status, but there is a small margin of error still.
    * TP: 18663
    * TN: 563
    * FP: 102
    * FN: 56

* Classification Report:
    * In this report we were able to see that our model did pretty well with predicting loan status based off of the scores. We had a very high precision, recall and f-1 score for both healthy and high-risk loan status. The scores are slightly higher with predicting healthy loans than high-risk loans telling us the model was more accurate with healthy loans. Both are still very high indicating that the model has performed very well.
    * Precision Scores: Measure of predicitng positive classes correctly.
        * 0: 1.00
        * 1: 0.85
    * Recall Scores: Measure of ratio of correctly predicted true positives against false negatives.
        * 0: 0.99
        * 1: 0.91
    * f-1 score: Composite score of the above two scores.
        * 0: 1.00
        * 1: 0.88


## Summary

I would recommend this model to predict the classification of loan status as this model scored very highly on both reports. It does predict the 0's (healthy loans) better than the 1's (high-risk loans) so I would highly trust it to classify healthy borrowers over high-risk borrowers. Although this model does have a small margin of error, the subject is not so serious that accidentally classifying someone as high-risk or healthy borrowers when they're not is going to severely impact them. This model very accurately predicts loan status with high results of correct classifications that I would recommend using it to help with this classification of borrowers.