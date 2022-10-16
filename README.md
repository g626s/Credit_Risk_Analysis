# Credit_Risk_Analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, for this project we employed different techniques to train and evaluate models with unbalanced classes. 

## Overview of the loan prediction risk analysis
The _imbalanced-learn_ and _scikit-learn_ libraries were implemented to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the _RandomOverSampler_ and _SMOTE algorithms_, and undersampled the data using the _ClusterCentroids algorithm_. We then used a combinatorial approach of over- and undersampling using the _SMOTEENN algorithm_. In the next phase of our project, we compared two new machine learning models that reduce bias, _BalancedRandomForestClassifier_ and _EasyEnsembleClassifier_, to predict credit risk. Lastly, we evaluated the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results

## Summary 

