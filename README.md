# Credit Risk Analysis

Using Supervised Machine Learning, Python, and Jupyter Notebook to predict credit risk

## Overview of Project

An analysis of borrower data to predict credit risk. Various Machine Learning alogrithms are utilized to determine the best fit for predicting credit risk.

### Purpose

FastLending, a peer to peer lending services company, wants to use machine learning to predict credit risk. This process is believed to be a quicker and more reliable loan experience. Machine learning will lead to identifying good candidates for loans and lead to a lower default rate. Several machine learning algorithms were utilized for this analysis including:
- Naive Random Oversampling
- SMOTE Oversampling
- ClusterCentroids Undersampling
- SMOTEENN
- Balanced Random Forest Classifier
- Easy Ensemble Classifier

## Results

#### *Naive Random Oversampling*

![naive-random-oversampling](https://user-images.githubusercontent.com/108373151/198747282-fb51f3e3-8f1e-439a-9b80-a8aafceaac3c.jpg)

Some data points to consider are:
- Accuracy Score: 66.20%
- True Positives: 73
- False Negatives: 28
- False Positives: 6,820
- True Negatives: 10,284
- High Risk Precision: 1%
- High Risk Recall: 72%

#### *SMOTE Oversampling*

![smote-oversampling](https://user-images.githubusercontent.com/108373151/198747440-0fdbb614-b8b9-4928-bad1-e6abff32a932.jpg)

Some data points to consider are:
- Accuracy Score: 65.68%
- High Risk Precision: 1%
- High Risk Recall: 61%

#### *ClusterCentroids Undersampling*

![undersampling](https://user-images.githubusercontent.com/108373151/198748634-1d8139be-f7c3-43db-a6e4-b270b7f225d2.jpg)

Some data points to consider are:
- Accuracy Score: 54.43%
- High Risk Precision: 1%
- High Risk Recall: 69%


#### *SMOTEENN*

![smoteenn](https://user-images.githubusercontent.com/108373151/198748433-7b6ad967-3b63-4497-9f68-1bed4b7727bf.jpg)

Some data points to consider are:
- Accuracy Score: 64.61%
- High Risk Precision: 1%
- High Risk Recall: 72%

#### *Balanced Random Forest Classifier*

![balanced-random-forest](https://user-images.githubusercontent.com/108373151/198747156-eb1fabf7-25ce-418e-a7be-22157d0efa96.jpg)

Some data points to consider are:
- Accuracy Score: 78.85%
- High Risk Precision: 3%
- High Risk Recall: 70%

Please note that in the random forest classifier, a lot of importance was placed on data that might not be a good indicator for credit risk. The file has a lot of columns and it would likely be more effective if the columns were trimmed to only reflect those factors that are associated with credit risk.

#### *Easy Ensemble Classifier*

![easy-ensemble](https://user-images.githubusercontent.com/108373151/198747215-ef862149-02d1-451b-99f0-dc3e06cab6c8.jpg)

Some data points to consider are:
- Accuracy Score: 93.17%
- High Risk Precision: 9%
- High Risk Recall: 92%

## Summary

The most accurate model in predicting credit risk is the Easy Ensemble Classifier. It successfully predicted 93 high risk customers. Additionally, the 983 false positives that may require extra review is the best result of all the models. Additionally, there were only 8 customers that are truly high risk that was predicted to be low risk. So for a 93.17% accuracy score, 9% precision score, and 92% recall score, the Easy Ensemble Classifier would be the recommended machine learning algorithm. This model has the best trade-off between sensitivity and precision.

