# Credit_Risk_Analysis

## Overview of the Analysis 
- Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once we were done, we evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.

## Results
- Cluster Centeroids:
  - <img width="703" alt="cc" src="https://user-images.githubusercontent.com/89552059/195715202-0410c85c-d130-4ea1-94ad-0daedd90c37e.png">
  - The cluster centroid machine learning method was the least accurate in predicting credit risk, with an accuracy score of 54 %. High-risk precision was recorded at 0.01 and sensitivity at 0.69, and the combined f-1 score resulted in 0.1. The low-risk score for precision was a perfect 1, and recall was 0.40 that resulted in an f-1 score of 0.57
  
- SMOTEENN:
    - <img width="718" alt="smoteeen" src="https://user-images.githubusercontent.com/89552059/195716401-f5d6d06e-eba4-4df6-984f-169a5ac2c926.png">
    - SMOTEENN combined method of over and undersampling proved to show a slight increase in accuracy score of about 64%.
    - High-risk precision and sensitivity scores showed 0.01 and 0.72, respectively, which combined to 0.02 f-1 score.
    - Low-risk precision and sensitivity scores resulted in 1 and 0.57, and an f-1 score 0f 0.72.
- Random Over Sampler:
  - <img width="710" alt="ros" src="https://user-images.githubusercontent.com/89552059/195717290-8fbb582e-4445-4eee-a5ca-d252cdb3da17.png">
  - Random Over Sampler method showed an accuracy rate of 66.38 percent.
  - High-risk scores for precision and recall were 0.01 and 0.70, and the f-1 score recorded only 0.02.
  - Low-risk scores were 1 and 0.62 for precision and recall, respectively, and the f-1 score at 0.77.
- SMOTE:
  - <img width="707" alt="smote" src="https://user-images.githubusercontent.com/89552059/195717932-0f51d8d4-1dfe-4c1c-ab48-2a0c629de112.png">
  - SMOTE Oversampling method showed an almost identical accuracy score as the Random Over Sampling method with 66.41 percent.
  - High-risk score resulted in 0.01 for precision and 0.63 for sensitivity, with the final score of 0.02 for f-1.
  - Low-risk precision score was 1, sensitivity score was 0.69, and an f-1 score of 0.82.
  
- Balanced Random Forest Classifier:
  - <img width="703" alt="brfc" src="https://user-images.githubusercontent.com/89552059/195718667-977e581b-0e81-423c-92a6-a94a4500cb4e.png">
  - Balanced Random Forest Classifier method resulted in a slight increase in accuracy score of about 79%.
  - High-risk scores for precision, sensitivity, and f-1 were 0.03, 0.70, and 0.06, respectively.
  - Low-risk scores for the same measures were 1, 0.87, and 0.93.
  
- Easy Ensemble AdaBoost Classifier:
  - <img width="712" alt="eec" src="https://user-images.githubusercontent.com/89552059/195719163-6924e8c7-67dc-41ae-8efd-7ed3645db637.png">
  - Easy Ensemble AdaBoost Classifier proved to be the most accurate method with an accuracy rate of about 93 %.
  - High-risk scores were 0.09, 0.92, and 0.16 for precision, recall, and the f-1.
  - Low-risk scores were 1, 0.94, and 0.97 for precision, recall, and the f-1.
  
## Summary:
- We should consider a high imbalance in low-risk and high-risk measures. Due to this, we can notice that there are good prediction results for almost all methods for predicting low-risk applicants. However, all the methods failed to be accurate in predicting high-risk applicants. I would not recommend any of the above methods as they fail to predict a measure of high-risk applicants.
