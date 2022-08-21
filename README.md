# Credit Risk Analysis
## Overview
##### We were tasked with applying different machine learning models to determine which would be the best in predicting a customer's credit risk for loan approvals. Because good loans tend to outnumber risky loans, we implemented oversampling, undersampling, and a combinatorial approach to better help our models when they train on the data. If the accepted loans severely outnumber the rejected loans, it will be hard for the model to predict true negatives. We then compared Balanced Random Forest Classifier and EasyEnsembleClassifer models to reduce bias and predict the customer's loan risk. The results of our tests are below.
## Results
### Naive Random Oversampling algorithm
![random_oversampling.png](https://github.com/carinaediaz/credit_risk_analysis/blob/main/Images/random_oversampling.PNG)
- Balanced accuracy score: 0.66
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
- Balanced accuracy score: 0.65
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
- Balanced accuracy score: 0.65
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
- Balanced accuracy score: 0.54
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
- Balanced accuracy score: 0.78
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
- Balanced accuracy score: 0.93
- Precision scores:
  - High Risk: 0.09
  - Low Risk: 1.00
  - Average: 0.99
- Recall scores:
  - High Risk: 0.92
  - Low Risk: 0.94
  - Average: 0.94
## Summary
##### Most of the resampling techniques (Naive Random, SMOTE, Cluster Centroids) produced very similar balanced accuracy and precision scores. The combinatorial SMOTEEN technique produced a lower balanced accuracy score compared to the other resampling techniques. While there is a high low risk precision score for all these techniques, the low high risk precision scores tell us that high-risk applications are poorly predicted by these models, allowing customers who should be denied credit to fall through the cracks. 
##### The balanced accuracy and high risk precision scores for the ensemble learner techniques were higher than those for the resampling techniques. Of the two, the Easy Ensemble technique produced the highest high risk precision, re-call, and f1 scores. Of the 17,205 customers, only 991 were incorrectly predicted. Because of this, I would recommend implementing the Easy Ensemble model to predict the loan approval status of customers. While it had the highest accuracy scores, it still incorrectly identified a large number of customers. It may be best to implement a system where the machine learning model first reviews and predicts approval, then the predictions are manually reviewed to determine if a customer's status should be changed.
