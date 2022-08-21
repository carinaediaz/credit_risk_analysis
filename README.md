# Credit Risk Analysis
## Overview
##### We were tasked with applying different machine learning models to determine which would be the best in predicting a customer's credit risk for loan approvals. Because good loans tend to outnumber risky loans, we implemented oversampling, undersampling, and a combinatorial approach to better help our models when they train on the data. If the accepted loans severly outnumber the rejected loans, it will be hard for the model to predict true negatives. We then compared Balanced Random Forest Classifier and EasyEnsembleClassifer models to reduce bias and predict the customer's loan risk. The results of our tests are below.
## Results
### Naive Random Oversampling algorithm
![random_oversampling.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/random_oversampling.PNG)
- Balanced accuracy score:
- Precision scores:
  - High Risk:
  - Low Risk:
- Recall scores:
  - High Risk:
  - Low Risk: 
### SMOTE Oversampling algorithm
![SMOTE_oversampling.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/SMOTE_oversampling.PNG)
### Cluster Centroids algorithm
![cluster_centriods_undersampling.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/cluster_centriods_undersampling.PNG)
### SMOTEEN algorithm
![SMOTEEN.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/SMOTEEN.PNG)
### Balanced Random Forest Classifier algorithm
![balanced_random_forest.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/balanced_random_forest.PNG)
### Easy Ensemble AdaBooster Classifier algorithm
![easy_ensemble.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/easy_ensemble.PNG)
## Summary
