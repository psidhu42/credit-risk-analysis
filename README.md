# Credit Risk Analysis

## Overview of Project

Use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

### Purpose

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, oversample the data using the RandomOverSampler and SMOTE. Then undersample the data using the ClusterCentroids. Then use a combination of the two with SMOTEENN. Use BalancedRandomForestClassifier and EasyEnsembleClassifier to predict credit risk.

## Results

Results of Analysis for data from "LoanStats_2019Q1.csv"

### Random Oversampling

![Random Oversampling](https://github.com/psidhu42/credit-risk-analysis/blob/main/resources/images/Random_Oversampling.png)
* Balanced Accuracy: 0.6485852762367502
* Precision: High Risk is 1%, and Low Risk is 100%.
* Recall: High Risk is 62%, and Low Risk is 68%.

### SMOTE

![SMOTE](https://github.com/psidhu42/credit-risk-analysis/blob/main/resources/images/SMOTE_Oversampling.png)
* Balanced Accuracy: 0.656385091716322
* Precision: High Risk is 1%, and Low Risk is 100%.
* Recall: High Risk is 67%, and Low Risk is 65%.

### ClusterCentroids

![ClusterCentroids](https://github.com/psidhu42/credit-risk-analysis/blob/main/resources/images/ClusterCentroids.png)
* Balanced Accuracy: 0.656385091716322
* Precision: High Risk is 1%, and Low Risk is 100%.
* Recall: High Risk is 60%, and Low Risk is 43%.

### SMOTEENN

![SMOTEENN](https://github.com/psidhu42/credit-risk-analysis/blob/main/resources/images/SMOTEENN.png)
* Balanced Accuracy: 0.5160196365189295
* Precision: High Risk is 1%, and Low Risk is 100%.
* Recall: High Risk is 70%, and Low Risk is 58%.

### BalancedRandomForestClassifier

![BalancedRandomForestClassifier](https://github.com/psidhu42/credit-risk-analysis/blob/main/resources/images/BalancedRandomForestClassifier.png)
* Balanced Accuracy: 0.7921638045953004
* Precision: High Risk is 3%, and Low Risk is 100%.
* Recall: High Risk is 70%, and Low Risk is 87%.

### EasyEnsembleClassifier

![EasyEnsembleClassifier](https://github.com/psidhu42/credit-risk-analysis/blob/main/resources/images/EasyEnsembleClassifier.png)
* Balanced Accuracy: 0.9316600714093861
* Precision: High Risk is 9%, and Low Risk is 100%.
* Recall: High Risk is 92%, and Low Risk is 94%.

## Summary

The first four models produced a weaker precision, and there for are unfit to use for determining credit risk. The BalancedRandomForestClassifier and EasyEnsembleClassifier had the higher precisions. The EasyEnsembleClassifier model had a balanced accuracy of roughly 93%. The Easy Ensemble model also had the highest recalls at 92% and 94%, making it the best out of the six machine learning models to use for determining credit risk.