# Credit_Risk_Analysis
Predicting levels of credit risk using various resampling algorithms and machine learning models

## Predict Credit Risk with Resampling Models
Using resampling to determine which of three machine learning models is the best at predicting credit risk. The three models in question are the oversampling RandomOverSampler and SMOTE algorithms, and the undersampling ClusterCentroids algorithm.

### Split the Data into Training and Testing Sets
<img width="1172" alt="Screen Shot 2023-02-08 at 8 24 10 PM" src="https://user-images.githubusercontent.com/95303422/217690896-95ddaff4-879d-4348-bee2-9b0ed963b314.png">

### Resample the Training Data with Each Algorithm and Assess Performance
Given the accuracy scores after making predictions with logistic regression, it appears that the oversampling algorithms outperformed the undersampling algorithm, with RandomOverSampler yielding the largest percentage of accurate classifications (63.8%).
* RandomOverSampler - 0.638
* SMOTE - 0.605
* ClusterCentroids - 0.507

### Predict Credit Risk with SMOTEENN Algorithm
The SMOTEENN algorithm is a combinational approach of over- and undersampling. After making predictions with logistic regression, it appears that this combinational algorithm was almost as accurate as the RandomOverSampler, correctly classifying 62.5% of cases as either high-risk or low-risk.

## Predict Credit Risk with Ensemble Classifiers
