# Credit_Risk_Analysis
---

## Overview

The aim of the paper is to look at credit risk and employ different techniques to train and evaluate models with unbalanced classes. It will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

### Aim

The aim of this paper is to used six machine learning models to analyise and predict credit risk, using the credit card dataset from LendingClub. The models are: 
- RandomOverSampler
- SMOTE
- ClusterCentroids
- SMOTEENN
- BalancedRandomForestClassifier
- EasyEnsembleClassifier

---
## Analysis and Results 

### RandomOverSampler

<p align="center">
<img src="Images/randomovsam_BAS.png" width="900">
<img src="Images/random_oversampling.png" width="900">
</p>

- Balanced Accuracy:64%
- High Risk Precision:1%
- High Risk Sensitivity:63%
- High Risk F1 Score:2%
- Low Risk Precision:100%
- Low Risk Sensitivity:64%
- Low Risk F1 Score:78%

<br>

### SMOTE

<p align="center">
<img src="Images/smote_oversampling.png" width="900">
</p>

- Balanced Accuracy:64%
- High Risk Precision:1%
- High Risk Sensitivity:62%
- High Risk F1 Score:2%
- Low Risk Precision:100%
- Low Risk Sensitivity:66%
- Low Risk F1 Score:79%

<br>

### ClusterCentroids

<p align="center">
<img src="Images/cluster_centroids.png" width="900">
</p>

- Balanced Accuracy:51%
- High Risk Precision:1%
- High Risk Sensitivity:59%
- High Risk F1 Score:1%
- Low Risk Precision:100%
- Low Risk Sensitivity:44%
- Low Risk F1 Score:61%

<br>

### SMOTEENN

<p align="center">
<img src="Images/smoteenn_BAS.png" width="900">
<img src="Images/smoteenn.png" width="900">
</p>

- Balanced Accuracy:62%
- High Risk Precision:1%
- High Risk Sensitivity:70%
- High Risk F1 Score:2%
- Low Risk Precision:100%
- Low Risk Sensitivity:54%
- Low Risk F1 Score:70%

<br>

### BalancedRandomForestClassifier

<p align="center">
<img src="Images/random_forest.png" width="900">
</p>

- Balanced Accuracy:79%
- High Risk Precision:3%
- High Risk Sensitivity:70%
- High Risk F1 Score:6%
- Low Risk Precision:100%
- Low Risk Sensitivity:87%
- Low Risk F1 Score:93%

<br>

### EasyEnsembleClassifier

<p align="center">
<img src="Images/emsemble.png" width="900">
</p>

- Balanced Accuracy:93%
- High Risk Precision:9%
- High Risk Sensitivity:92%
- High Risk F1 Score:16%
- Low Risk Precision:100%
- Low Risk Sensitivity:94%
- Low Risk F1 Score:97%

---
## Summary

In summary, all the models used to perform the credit risk analysis show weak precision in determining if a credit risk is high. The Easy Ensemble Classifier model had the highest overall accuracy, due largely to the fact that the dataset was so radically unbalanced. Even when it's balanced accuracy and average F-score were above 90%, it's F-score for high-risk prediction was no better than 0.16.

For the reasons stated above, it would be recommended to not use any of the algorithms, as it would put creditors as too great of risk being unable to accurately predict who the high-risk clients/debtors would be. Though all the models were strong in predicting low risk credit, they are sill weak when predicting hight reisk credit, including Ensemble model, it would still be advised to not use any of the models above. 
