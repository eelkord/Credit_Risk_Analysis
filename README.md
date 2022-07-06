# Credit_Risk_Analysis


## Overview of the Project

The purpose of this analysis is to understand how to utilize Machine Learning statistical algorithms to make predictions based on data patterns provided. In this challenge, we focus on Supervised Learning using a free dataset from LendingClub, a P2P lending service company to evaluate and predict credit risk. This reason why this is called "Supervised Learning" is because the data includes a labeled outcome.

To complete this analysis, we use different Machine Learning techniques to train and evaluate the data with unbalanced classes. The dataset from the LendingClub has an unbalanced classification problem due to the number of good loans outweighing the amount of risky loans. In order balance out the classifications to allow for more meaningful predictions and improve the accuracy score, we needed to employ various Machine Learning algorithms to resample the data. These algorithms include RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.


Naive Random Oversampling results: Our balanced accuracy test it 67%, the precision for the high_risk has a very low positivity at 1% and the recall is 74%

<img width="1382" alt="1" src="https://user-images.githubusercontent.com/100106554/177469097-bc8da43d-11f6-4529-aed9-037f6992c8f9.png">

SMOTE oversampling results: the accuracy score is 66.2%, the precision for the high_risk loans has a low positvity again at 1% and recall is 69% overall


<img width="1286" alt="2" src="https://user-images.githubusercontent.com/100106554/177469110-e16f13fc-2bed-4d33-add5-b1d6908504e2.png">


Undersampling results: balanced accuracy score is 66.2% overall, the precision is at 99% and the recall is 41%
<img width="1315" alt="3" src="https://user-images.githubusercontent.com/100106554/177469125-f83954d4-ebbd-41ad-a533-0b4643dd5d68.png">

Combination(over and undersampling) results: balanced accuracy score is 54.7% the precision is 99% and the recall is 57% overall

<img width="1355" alt="4" src="https://user-images.githubusercontent.com/100106554/177469679-9ec24c38-645f-4719-b7cc-0e501cfa5bea.png">

Balanced Random Forest Classifier results: the accuracy score is 77.2% the precision is 99% and the recall is 88%

<img width="1293" alt="5" src="https://user-images.githubusercontent.com/100106554/177469685-88ed099b-68bb-4025-af84-9e59b5316f9c.png">


Easy Ensemble AdaBoost Classifier results: the accuracy score is 91.7% the precision is 99% and the recall is 94%

<img width="1353" alt="6" src="https://user-images.githubusercontent.com/100106554/177469695-6a47c4f8-4b8b-4b00-bf4b-bdcc8f92f975.png">


## Summary

In the first four models we undersampled, oversampled and did a combination of both to try and determine which model is best at predicting which loans are the highest risk. The next two models we resampled the data using ensemble classifiers to try and predict which which loans are high or low risk. In our first four models our accuracy score is not as high as the ensemble classifiers and the recall in the oversampling/undersampling/mixed models is low as well. Typically in your models you want a good balance of recall and precision which is why I recommend the ensemble classifiers over the first four models. It appears that the Easy Ensemble had the best balance of all the models because of it's high accuracy score and good balance of precision and recall scores.
