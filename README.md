# Credit_Risk_Analysis
## Overview 
Using the credit card dataset from LendingCLub, data preparation, statistical and machine learning were used to evaluate credit risk.  Imbalanced-learn and scikit-learn libraries will assist in to build and evaluate models using resampling.  These include RandomOverSampler and SMOTE algorithms and under sample the data with ClusterCentroids.  Next, a combinational approach of over- and under sampling was implemented with SMOTEENN algorithm.  After the use of SMOTEEN algorithm, a comparison of BalancedRandomForestClassifier and EasyEnsembleClassifier were used to compared to determine best model to reduce bias and predict credit risk. Balanced accuracy test will be used measured for each model.  It will determine the performance of each model with dealing with imbalanced two classes (high risk or low risk).  These are the true positive and true negatives.  The next test is the precison and recall.  This will quantify number of positive class predictions that belong to positive class(precision) and quantifying the number of positive class predictions for all the positive examples in the data(recall).  
## Results

## Oversampling

### Naive Random Oversampling
! [alt txt]()
* Balanced Accuracy Score: 64.5%

! [alt txt]()
* Precision and Recall scores: 
    * High Risk: Precision of .01, Recall of .70
    * Low Risk: Precision of 1.0, Recall of .59
    * Avg/Total: Precision of .99, Recall of .59

### SMOTE Over sampling
! [alt txt]()
* Balanced Accuracy Score: 68.4%

! [alt txt]()
* Precision and Recall scores: 
    * High Risk: Precision of .01, Recall of .81
    * Low Risk: Precision of 1.0, Recall of .56
    * Avg/Total: Precision of .99, Recall of .56

## Under Sampling

### Cluster Centroids
! [alt txt]()
* Balanced Accuracy Score: 54.4%

! [alt txt]()
* Precision and Recall scores: 
    * High Risk: Precision of .01, Recall of .69
    * Low Risk: Precision of 1.0, Recall of .39
    * Avg/Total: Precision of .99, Recall of .40

## Combination (Over and Under) Sampling

### SMOTEENN
! [alt txt]()
* Balanced Accuracy Score: 68.4%

! [alt txt]()
* Precision and Recall scores: 
    * High Risk: Precision of .01, Recall of .81
    * Low Risk: Precision of 1.0, Recall of .56
    * Avg/Total: Precision of .99, Recall of .56


## Ensemble Learners

### Balanced Random Forest Classifier
! [alt txt]()
* Balanced Accuracy Score: near 77.0%

! [alt txt]()
* Precision and Recall scores: 
    * High Risk: Precision of .03, Recall of .66
    * Low Risk: Precision of 1.0, Recall of .88
    * Avg/Total: Precision of .99, Recall of .87

### Easy Ensemble AdaBoost Classifier
! [alt txt]()
* Balanced Accuracy Score: near 93.2%

! [alt txt]()
* Precision and Recall scores: 
    * High Risk: Precision of .09, Recall of .92
    * Low Risk: Precision of 1.0, Recall of .94
    * Avg/Total: Precision of .99, Recall of .94


## Summary
The six models performed at varying levels.  The machine learning models within oversampling, under sampling and combination (under- oversampling) truly performed at weaker side especially with high risk.  The under sampling of Cluster Centroids was weakest performer (avg recall of .40).  Overall testing showed that these models had a difficult time with classifying high risk.  I would not recommend the models for prediction of credit risk.  The one model which showed possible implementation would be Easy Ensemble AdaBoost Classifier.  It had recall of .92 for high risk, recall of .94 for low risk, and avg/total precision of .99 and recall of .94.  The Balanced Accuracy Score was near 93.2%.  Depending on the usage of these credit risk assessments, Easy Ensemble AdaBoost could be used.  I would although not recommend application for extremely important such as mortgage.  This could negatively affect potential buyers who are misclassified.  
   

