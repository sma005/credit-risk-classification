# Credit Risk Report

## Overview of the Analysis
This analysis compared two different models to see which one would have a better predictor of good accounts vs high risk accounts.
The data had various data points that showed various banking data, and if it was labeled good or bad. Loan status was split from the 
rest of the data to use that as the indicator whether the account was good or bad.

We used a Logistic Training Model to get info on both the training data, and the testing data. The testing data did better than the training data
so
In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

The classification report has every healthy loan being detected, but not every high-risk loan is being detected. If it is high risk, 
there is more than a 10% chance to miss the fact that it is a high risk loan. This model should not be used.



## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Training model:
 [[55980   297]
 [  198  1677]]
* Testing model:
[[18679    80]
 [   67   558]]
* Classification report:
   precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      0.89      0.88       625

    accuracy                           0.99     19384
   macro avg       0.94      0.94      0.94     19384
weighted avg       0.99      0.99      0.99     19384
  

## Summary

From the testing matrix, we can see that the number of false positives went considerably down from the training matrix. It showed improvement. 
There was about a 0.12% chance that a high risk would get flagged as a healthy loan, which would be the worst case scenario for the bank. 
There is also about a 0.14% healthy account would get flagged as high risk. This is a loss in buisness.

It looks like this model is getting better as it receives more data. I wouldn't scrap this project, but I would see if it improves with more customers.
