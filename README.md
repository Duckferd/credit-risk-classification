# credit-risk-classification
Module 20 Challenge- Credit Risk Classification

Project Description: This is the assignment submission for challenge #20- Credit Risk classification. This assignment involves usage of Supervised Learning Model (Logistic Regression Model) with original data and oversampled data to create a model that evaluates credit risk.  

## Credit Risk Analysis Report

### Analysis Overview
The purpose of creating a supervised training model, specifically a Logistic Regression Model is to evaluate the riskiness of loans based on a couple of factors. These include the size and interest rate of the loan, the borrower's income, total number of accounts, debt to income ratio, total debt, and whether the account has any derogatory marks. 

The model should take in a potential applicant's information and then evaluate whether that application will result in a healthy or high risk loan.

### Results
The model was evaluated using the original dataset, as well as an oversampled dataset.

With the original dataset:
- the overall accuracy score was very high (0.992). The confusion matrix shows a relatively low number of false negatives and positives. 
- Looking at the classification report, the precision/recall/FI score for 0 (healthy loans) shows very good performance for predictions. High risk labels however show slightly lower performance, at 0.88. 
- In the context of credit risk assessement, this performance should be improved as this grouping is more important than 0 (healthy loans)

The oversampled dataset shows improvements in all areas. 
- Accuracy score increased slightly to 0.994, but the confusion matrix showed that the number of false negatives and positives have dropped and are very similar now. This is corroborated by the classification report. 
-  With oversampling, the F1 and accuracy scores for 0 (healthy loans) decreases minimally (0.01 in all instances), but the F1 and accuracy scores of high risk loan labels increased significantly to 0.99. 
- The model does a much better job predicting high risk loans while still doing a very good job predicting healthy loans. This is overall a very good model now. 

### Summary
The results from the original dataset is good, but the oversampled dataset is better. Recommendation is to use the Logistic Regression Model that has been trained on oversampled data. This model provides good performance for both healthy and unhealthy loans, with F1 and accuracy scores for both categories at 0.99.


### Other Info
Getting Started and Installation: Open credit_risk_classification.ipynb and run the script. Ensure that the raw data is in the resources folder.

The following are uploaded to Github: All original folders including resources

Contributors: Christopher Yang

Acknowledgements: I would like to thank the University of Toronto for putting together a robust program for Data Analytics, my fellow classmates as well as the wonderful Instructors and LAs at the University of Toronto for their support.

License: This is licensed under the MIT licensing scheme. Please see separate License File for information.