# Credit_Risk_Analysis
Module 17
## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. In this project, I employed different techniques to train and evaluate models with unbalanced classes. I used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. With this information, I can  evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
*Naive Random Oversampling
<img width="699" alt="image" src="https://user-images.githubusercontent.com/110864175/206274540-a983d59f-a77f-4354-b4fe-0f1c924da140.png">
The balanced accurage score is 62.9% for this model. The precision is 99% and the recall is 68%. 

*SMOTE Oversampling
<img width="707" alt="image" src="https://user-images.githubusercontent.com/110864175/206274916-4e6b3208-2f1f-4085-ac2d-ba8b361a8f40.png">
The balanced accuracy score is 62.7% for this model. The precision is 99% and the recall is 63%. 

*Undersampling
<img width="708" alt="image" src="https://user-images.githubusercontent.com/110864175/206275165-df9d1cca-af86-40fd-bfce-50252f0d5bc8.png">
The balanced accuracy score is 51% for this model. The precision is 99% and the recall is 44%. 

*Combination (Over and Under) Sampling
<img width="709" alt="image" src="https://user-images.githubusercontent.com/110864175/206275324-b1a6f9a2-1860-430e-a094-b65942920663.png">
The balanced accuracy score is 64.1% for this model. The precision is 99% and the recall is 58%.

*Balanced Random Forest Classifier
<img width="702" alt="image" src="https://user-images.githubusercontent.com/110864175/206275646-da3dacfa-3d5f-43a8-9d88-b8bb872d99dc.png">
The balanced accuracy score is 78.9%. The precision is 99% and the recall is 87%. 

*Easy Ensemble AdaBoost Classifier
<img width="672" alt="image" src="https://user-images.githubusercontent.com/110864175/206275747-2fbc8350-5b66-4e18-9dd9-b38aa9c540ec.png">
The balanced accuracy score is 93.2%. The precision is 99% and the recall is 94%. 



## Summary
