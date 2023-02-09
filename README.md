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
Training and comparing two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk and evaluating the accuracy of each model. 

Accuracy Scores:
* BalancedRandomForestClassifier - 0.802
* EasyEnsembleClassifier - 0.938

The ensemble classifiers were far more accurate than the resampling algorithms, with the EasyEnsembleClassifier producing a correct classification for an amazing 93.8% of cases. While the BalancedRandomForestClassifier clocked in at a lesser 80.2%, it has the added benefit of providing a list of the most influential features in its model.

Top Ten Most Important Features in BalancedRandomForestClassifier:
<img width="686" alt="Screen Shot 2023-02-08 at 9 12 49 PM" src="https://user-images.githubusercontent.com/95303422/217699311-f64b0a16-7e8a-4380-9579-aa571afe9d8a.png">
