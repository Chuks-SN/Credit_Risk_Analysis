# Overview of the Analysis 

In this analysis, we're applying machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we’ll need to employ different techniques to train and evaluate models with unbalanced classes. We'll use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We’ll also compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once we’re done, we’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results 
### Balance Accuracy, Precison and Recall Scores of the ML Models 

#### Accuracy Score
Naive Random Oversampling Accuracy = 0.6614 (66%)

Oversampling Accuracy Score for SMOTE = 0.6581 (66%)

Undersampling Accuracy = 0.6581 (66%)

Combination (Over and Under) = 0.5442 (54%)

Balanced Random Forest Classifier = 0.7959 (80%)

Ensemble AdaBoost Classifier = 0.9197 (92%)

#### Precison Score 
Precison score for all was 99%

#### Recall Score 
Nave Random Oversampling = 0.60 (60%)

SMOTE Oversampling = 0.69 (69%)

Undersampling = 0.40 (40%)

Combination (Over and Under) Sampling = 0.57 (57%)

Balanced Random Forest Classifier = 0.91 (91%)

Ensemble AdaBoost Classifier = 0.94 (94%)

## Summary 

Precision score for all was 99%, accuracy and sensitivity scores varied accross board. The Ensemble AdaBoost Classifier had the highest accuracy and Recall scores, at 92 and 84 percent respectively. 

For the above reasons, I'd recommend the Ensemble AdaBoost Classifier machine learning model as a preferred option. 
