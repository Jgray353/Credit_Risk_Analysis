# Credit_Risk_Analysis

## Overview/Purpose 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. WIth that, the purpose is to employ different techniques to train and evaluate models with unbalanced classes. This project will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, this project will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Next, what will be done is a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. The purpose will be to figure out the best model to use to detect high risk loans. 

Finally, this written analysis will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results

# Naive Random Oversampling

<img width="708" alt="NaiveRandomSampling" src="https://user-images.githubusercontent.com/90881705/153731297-c0299226-e831-4dce-9417-0931dd1ef14c.png">

1. The balanced accuracy is 0.6556397581090282
2. The precision is high for low risk loans at 1, and low for high risk loans at .01. 
3. The recall is .64 for high risk loans, and .67 for low risk. 

# SMOTE Oversampling

<img width="695" alt="SMOTEOversamping" src="https://user-images.githubusercontent.com/90881705/153731298-61089279-7655-4759-b014-0bd1ac3445b1.png">

1. The balanced accuracy is 0.6642131090080616.
2. The precision is high for low risk loans at 1, and low for high risk loans at .01. 
3. The recall is .67 for high risk loans, and .66 for low risk. 

# Undersampling

<img width="699" alt="Undersampling" src="https://user-images.githubusercontent.com/90881705/153731301-6aa4b6cd-1ac8-42b2-a675-4b69c027b15f.png">

1. The balanced accuracy is 0.5293318990697431.
2. The precision is high for low risk loans at 1, and low for high risk loans at .01. 
3. The recall is .61 for high risk loans, and .45 for low risk. 

# Combination (Over and Under) Sampling

<img width="699" alt="Combination(OverandUnder)Sampling" src="https://user-images.githubusercontent.com/90881705/153731309-7aacc824-4474-49f1-a66a-47af5f511132.png">

1. The balanced accuracy is 0.6188152418708276.
2. The precision is high for low risk loans at 1, and low for high risk loans at .01. 
3. The recall is .68 for high risk loans, and .56 for low risk. 

# Balanced Random Forest Classifier

<img width="696" alt="BalancedRandomForestClassifier" src="https://user-images.githubusercontent.com/90881705/153731317-eeda20de-6ca2-49fc-a52e-4ac35d4a6a56.png">

1. The balanced accuracy is 0.7877672625306695. 
2. The precision is high for low risk loans at 1, and low for high risk loans at .04. 
3. The recall is .67 for high risk loans, and .91 for low risk. 

# Easy Ensemble AdaBoost Classifier

<img width="703" alt="EasyEnsembleAdaBoostClassifier" src="https://user-images.githubusercontent.com/90881705/153731319-f1ee45c1-c374-400c-9212-2220e2ee4893.png">

1. The balanced accuracy is 0.925427358175101.
2. The precision is high for low risk loans at 1, and low for high risk loans at .07. 
3. The recall is .91 for high risk loans, and .94 for low risk. 

## Conclusion

The results show us that the Easy Ensemble Classifier is the best model to use for detecting high risk loans, as well as ensuring low risk loans are not incorrectly flagged. Easy Ensemble Classifier had the accuracy score of over 90%. Of these models, it's...easy to recommend the Easy Ensemble Classifier. 
