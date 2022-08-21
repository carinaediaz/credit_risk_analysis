# Credit Risk Analysis
## Overview
##### We were tasked with applying different machine learning models to determine which would be the best in predicting a customer's credit risk for loan approvals. Because good loans tend to outnumber risky loans, we implemented oversampling, undersampling, and a combinatorial approach to better help our models when they train on the data. If the accepted loans severly outnumber the rejected loans, it will be hard for the model to predict true negatives. We then compared Balanced Random Forest Classifier and EasyEnsembleClassifer models to reduce bias and predict the customer's loan risk. The results of our tests are below.
## Results
### Naive Random Oversampling algorithm
![random_oversampling.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/random_oversampling.PNG)
- Balanced accuracy score:
- Precision scores:
  - High Risk: 0.01
  - Low Risk: 1.00
  - Average: 0.99
- Recall scores:
  - High Risk: 0.72
  - Low Risk: 0.60
  - Average: 0.60
### SMOTE Oversampling algorithm
![SMOTE_oversampling.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/SMOTE_oversampling.PNG)
- Balanced accuracy score:
- Precision scores:
  - High Risk: 0.01
  - Low Risk: 1.00
  - Average: 0.99
- Recall scores:
  - High Risk: 0.62
  - Low Risk: 0.69
  - Average: 0.69
### Cluster Centroids algorithm
![cluster_centriods_undersampling.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/cluster_centriods_undersampling.PNG)
- Balanced accuracy score:
- Precision scores:
  - High Risk: 0.01
  - Low Risk: 1.00
  - Average: 0.99
- Recall scores:
  - High Risk: 0.69
  - Low Risk: 0.40
  - Average: 0.40
### SMOTEEN algorithm
![SMOTEEN.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/SMOTEEN.PNG)
- Balanced accuracy score:
- Precision scores:
  - High Risk: 0.01
  - Low Risk: 1.00
  - Average: 0.99
- Recall scores:
  - High Risk: 0.77
  - Low Risk: 0.57
  - Average: 0.57
### Balanced Random Forest Classifier algorithm
![balanced_random_forest.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/balanced_random_forest.PNG)
- Balanced accuracy score:
- Precision scores:
  - High Risk: 0.03
  - Low Risk: 1.00
  - Average: 0.99
- Recall scores:
  - High Risk: 0.70
  - Low Risk: 0.87
  - Average: 0.87
### Easy Ensemble AdaBooster Classifier algorithm
![easy_ensemble.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/easy_ensemble.PNG)
- Balanced accuracy score:
- Precision scores:
  - High Risk: 0.09
  - Low Risk: 1.00
  - Average: 0.99
- Recall scores:
  - High Risk: 0.92
  - Low Risk: 0.94
  - Average: 0.94
## Summary
