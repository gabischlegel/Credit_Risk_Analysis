# Credit_Risk_Analysis
Module 17
## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. In this project, I employed different techniques to train and evaluate models with unbalanced classes. I used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. With this information, I can  evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
* Naive Random Oversampling
<img width="699" alt="image" src="https://user-images.githubusercontent.com/110864175/206274540-a983d59f-a77f-4354-b4fe-0f1c924da140.png">

The balanced accurage score is 62.9% for this model. For the average, the precision is 99% and the recall is 68%. The high risk precision is 1% and the recall is 57%.

* SMOTE Oversampling
<img width="707" alt="image" src="https://user-images.githubusercontent.com/110864175/206274916-4e6b3208-2f1f-4085-ac2d-ba8b361a8f40.png">

The balanced accuracy score is 62.7% for this model. For the average, the precision is 99% and the recall is 63%. The high risk precision is 1% and the recall is 62%. 

* Undersampling
<img width="708" alt="image" src="https://user-images.githubusercontent.com/110864175/206275165-df9d1cca-af86-40fd-bfce-50252f0d5bc8.png">

The balanced accuracy score is 51% for this model. For the average, the precision is 99% and the recall is 44%. The high risk precision is 1% and the recall is 59%.

* Combination (Over and Under) Sampling
<img width="709" alt="image" src="https://user-images.githubusercontent.com/110864175/206275324-b1a6f9a2-1860-430e-a094-b65942920663.png">

The balanced accuracy score is 64.1% for this model. For the average, the precision is 99% and the recall is 58%. The high risk precision is 1% and the recall is 70%.

* Balanced Random Forest Classifier
<img width="702" alt="image" src="https://user-images.githubusercontent.com/110864175/206275646-da3dacfa-3d5f-43a8-9d88-b8bb872d99dc.png">

The balanced accuracy score is 78.9%. For the average, precision is 99% and the recall is 87%. The high risk precision is 3% and the recall is 70%.

* Easy Ensemble AdaBoost Classifier
<img width="672" alt="image" src="https://user-images.githubusercontent.com/110864175/206275747-2fbc8350-5b66-4e18-9dd9-b38aa9c540ec.png">

The balanced accuracy score is 93.2%. For the average, precision is 99% and the recall is 94%. The high risk precision is 9% and the recall is 92%.



## Summary
We used 6 different models in this analysis to see which model is best at prediciting high risk loans. All of the above models have very low high risk precision rates indicating many false positives. The Easy Ensemble AdaBoost Classifier has the highest high risk precision and highest recall. The balance accuracy is also much higher than the other models. The most effective model is the Easy Ensemble AdaBoost Classifier, however I would not recommend using any of the models due to the amount of false postives even the Easy Ensemble AdaBoost Classifier model will generate. 
