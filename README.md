# Credit_Risk_Analysis
Supervised Machine Learning 

## Purpose/Objective:

The objective was to compare different resampling and ensemble techniques and determine which ones perform the best when predicting credit risk. Balanced accuracy scores, confusion matrices and imbalanced classification reports were generated for comparison purposes.

## Results: 

### Resampling 

Logistic Regression was used for the resampling methods.

#### Naive Random Oversampling 

<img width="707" alt="Screen Shot 2022-05-11 at 6 17 12 PM" src="https://user-images.githubusercontent.com/92544151/167956591-fc99de12-ff87-4ce9-9ff1-7d67b5297068.png">

Balanced accuracy score : 0.67

Recall (high_risk) : 0.74

Precision (high_risk) : 0.01 

#### SMOTE Oversampling 

<img width="718" alt="Screen Shot 2022-05-11 at 6 18 30 PM" src="https://user-images.githubusercontent.com/92544151/167956737-8deba785-ab1f-48fd-9014-ba9977cb1187.png">

Balanced accuracy score : 0.66

Recall (high_risk) : 0.63

Precision (high_risk) : 0.01

#### Undersampling - Cluster Centroids 

<img width="723" alt="Screen Shot 2022-05-11 at 6 19 04 PM" src="https://user-images.githubusercontent.com/92544151/167956802-a5adbb13-226d-489f-9d54-02471f1e7e74.png">

Balanced accuracy score : 0.54

Recall (high_risk) : 0.69

Precision (high_risk) : 0.01

#### Combination (Over and Under) Sampling - SMOTEENN

<img width="718" alt="Screen Shot 2022-05-11 at 6 22 35 PM" src="https://user-images.githubusercontent.com/92544151/167957178-629a8112-19db-459c-94d3-cce7895651e5.png">

Balanced accuracy score : 0.64

Recall (high_risk) : 0.71

Precision (high_risk) : 0.01

### Ensemble Learning 

#### Balanced Random Forest Classifier

<img width="715" alt="Screen Shot 2022-05-11 at 6 23 28 PM" src="https://user-images.githubusercontent.com/92544151/167957280-291154ac-55f7-4431-b647-826840c23cf9.png">

Balanced accuracy score : 0.79

Recall (high_risk) : 0.70

Precision (high_risk) : 0.03

#### Easy Ensemble AdaBoost Classifier

<img width="727" alt="Screen Shot 2022-05-11 at 6 25 07 PM" src="https://user-images.githubusercontent.com/92544151/167957472-52bb3647-988a-4467-bc00-aaf48a4ea797.png">

Balanced accuracy score : 0.93

Recall (high_risk) : 0.92

Precision (high_risk) : 0.09

## Summary

The dataset is imbalanced intrinsically. The ratio of high-risk to low-risk is very low. As a result, the precision values are less important than the recall (sensitivity) values. Looking at the recall values for the 6 methods tested, "Easy Ensemble AdaBoost classifier" scores the highest (0.92 for high_risk). Even though the precision values are of lesser importance with regards to this specific dataset, this ensemble method also has the highest precision out of the tested methods.  
