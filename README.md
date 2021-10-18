# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis:
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, I have used different techniques to train and evaluate models with unbalanced classes.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I had oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 
Then,I used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
Next, I compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 
## Results:
oversample the data using the RandomOverSampler and SMOTE algorithms and observed balanced accuracy score and precision scores and then undersample the data using the ClusterCentroids algorithm.
![randomoversample.png](https://github.com/deepayogesh/Credit_Risk_Analysis/blob/4d636c4361953bc7e8f9c4d89709c4d9d66592ec/img/randomoversample.png)

Observing the classification report shows the our SMOTEEN undersampling classification gives less value of precision and the random sampling logistic regression shows closer higher precision to our model. 
BalancedRandomForestClassifier
![balrandomforest.png](https://github.com/deepayogesh/Credit_Risk_Analysis/blob/4d636c4361953bc7e8f9c4d89709c4d9d66592ec/img/balrandomforest.png)

Classification report after using dabooster to our randomforest classification. Adding boost to our classification we can see the less number of recall value.
EasyEnsembleClassifier
![ adaboost-arcy.png](https://github.com/deepayogesh/Credit_Risk_Analysis/blob/4d636c4361953bc7e8f9c4d89709c4d9d66592ec/img/adaboost-arcy.png)

## Summary:
We should use the randomboost classifier with a booster which shows less number of recall values and colser to prediction.  And we can get get higher values of actual and predicted true. 