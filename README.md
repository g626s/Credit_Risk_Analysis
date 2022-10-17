# Credit_Risk_Analysis
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, for this project we employed different techniques to train and evaluate models with unbalanced classes. 

## Resources
<details>
<summary>Dataset:</summary>

- LoanStats_2019Q1.csv
</details>

<details>
<summary>Software and IDE:</summary>

- Python
- Jupyter Notebook
- Libraries:
  - Numpy
  - Scikit-learn
  - Imbalanced-learn 
- Techniques:
  - Ensemble
  - Resampling
</details>

## Overview of the loan prediction risk analysis
The _imbalanced-learn_ and _scikit-learn_ libraries were implemented to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the _RandomOverSampler_ and _SMOTE algorithms_, and undersampled the data using the _ClusterCentroids algorithm_. We then used a combinatorial approach of over- and undersampling using the _SMOTEENN algorithm_. In the next phase of our project, we compared two new machine learning models that reduce bias, _BalancedRandomForestClassifier_ and _EasyEnsembleClassifier_, to predict credit risk. Lastly, we evaluated the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
Using our knowledge of the _imbalanced-learn_ and _scikit-learn_ libraries, we evaluated three machine learning models by using _resampling_ to determine which is better at predicting credit risk. First, we used the _oversampling_ `RandomOverSampler` and `SMOTE algorithms`, and then we used the _undersampling_ `ClusterCentroids algorithm`. Using these algorithms, we _resampled the dataset_, _view the count of the target classes_, _train a logistic regression classifier_, _calculate the balanced accuracy score_, generate a _confusion matrix_, and generate a _classification report_.

- Native Random Oversampling:
![Screen Shot 2022-10-16 at 8 08 24 PM](https://user-images.githubusercontent.com/107281474/196081189-227320da-ff2e-4499-88f3-330d237af4c0.png)

- SMOTE Oversampling:
![Screen Shot 2022-10-16 at 8 08 36 PM](https://user-images.githubusercontent.com/107281474/196081342-a6ac8681-26ae-4287-9448-6c59f7fa13ec.png)

- Cluster Centroid Undersampling:
![Screen Shot 2022-10-16 at 8 09 12 PM](https://user-images.githubusercontent.com/107281474/196081363-8457e490-414d-4e44-9481-487a784fad18.png)

The next phase of the project was to implement a combinatorial approach of _over- and undersampling_ with the `SMOTEENN algorithm` to determine if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from the previous step. Using the `SMOTEENN algorithm`, we _resampled the dataset_, _view the count of the target classes_, _train a logistic regression classifier_, _calculate the balanced accuracy score_, generate a _confusion matrix_, and generate a _classification report_.

- SMOTEENN Combination Sampling:
![Screen Shot 2022-10-16 at 8 14 10 PM](https://user-images.githubusercontent.com/107281474/196081569-01ad8755-6ada-4924-9824-75238a101f54.png)

## Summary 

