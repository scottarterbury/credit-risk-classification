# credit-risk-classification

## Overview of the Analysis

For this challenge, I used a logistic regression model to train and evaluate a model for loan risk. I used historical lending activity  data from a peer-to-peer lending services company to build a model and identify the creditworthiness of borrowers.

The data included the loan size, interest rate, borrower's income, debt-to-income ratio, derogatory marks, their total debt and current loan status. The loan status was either  healthy (0) or a risky (1).

Using the logistic regression model I was determined to predict whether the loan would be a good investment on behalf of the lender or a risky investment. I separated the data into training data--to train the model--and testing data--to test the model's results. 

Then I used a confusion matrix to and classification report to evaluate the model.


## Results

The confusion matrix generated a report that showed:

- 18679 true negatives with 80 false negatives (0.004% inaccuracy)
- 67 false positives with 558 true positives (12% inaccuracy)

The classification report showed a 99% overall accuracy and a breakdown of the following:
 - Healthy loans (0)
    - Precision: 100% (rounded up)
    - Recall: 100%
    - F1-Score: 88%

 - Risky loans (1)
    - Precision: 87%
    - Recall: 89%
    - F1-score: 88%

## Summary

Overall the logistic regression model proved to be an accurate assessment of credit worthiness to determine whether a loan would be healthy or risky. However, the ratio between healthy and risky loans was greatly unbalanced (625 to 18,759) and may lead to more weight being applied to healthy loans. Further testing may be needed to truly be an accurate predictor of credit worthiness. Overall I would recommend this model to test for credit worthiness with the caveat of continued testing with training and testing data.