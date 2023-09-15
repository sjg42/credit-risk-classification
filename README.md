## Overview of the Analysis

The purpose of this analysis was to use a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.
The dataset included Loan Size, Interest Rate, Borrower Income, Debt to Income Ratio, Number of Accounts, Derogatory Marks, Total Debt, and their Creditworthiness. The goal of the analysis was to predict a borrower's Creditworthiness using the other provided variables.  The dataset included 75,036 borrowers that were considered creditworthy, and 2500 borrowers that were identified as risky borrowers.

In order to prepare for the machine learning process, we split the dataset into training data and test data, and then created Logistic Regression Models (one with the original dataset, one that was resampled in order to balance the training data between creditworthy and risky borrowers).


## Results

* Machine Learning Model 1 (Logistic Regression, Unbalanced training data):
		* Balanced Accuracy Score: 94.31%
  * Creditworthy Borrowers: Precision - 100%,  Recall - 100%
  * Risky Borrowers: Precision - 86%,  Recall - 89%


* Machine Learning Model 2 (Logistic Regression, Resampled training data so the model is trained on an equal number of creditworthy and risky borrowers):
  * Balanced Accuracy Score (resampled): 99.49%
  * Creditworthy Borrowers: Precision - 100%,  Recall - 99%
  * Risky Borrowers: Precision - 86%,  Recall - 100%
  

## Summary

Ultimately, ML Model 2 is the better model in this case because it is the more cautious model. In this case, we wanted to correctly identify the risky borrowers, and since ML Model 2 was trained on resampled data (equal parts creditworthy and risky borrowers), it was able to do a much better job at identifying risky borrowers and reduced the number of falsely identified creditworthy borrowers!
