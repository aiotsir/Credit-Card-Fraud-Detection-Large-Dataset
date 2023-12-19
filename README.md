# Credit-Card-Fraud-Detection-Large-Dataset
Predicting the probability that an online transaction is fraudulent on Large Dataset

## Dataset --> https://www.kaggle.com/competitions/ieee-fraud-detection
In the dataset, there are four files and total size is 1.35 GB. Cleaned and Merged to obtain the train and test datset of following size :

Train data set : (590540, 434) i.e., five lakh ninety thousand five hundred forty rows and 434 features

Test data set : (506691, 433) i.e., five lakh six thousand six hundred ninety-one rows and 433 features

# Models 

## 1. Isolation Forest      2. XGBoost    3. Neural Network  4. Ensemble of XGBoost and Isolation Forest  

My XGB model achieved high precision, recall, and F1-score for the majority class (0).
And it had good accuracy and AUC score (0.92) indicating overall good performance. But it gave lower performance on the minority class (1) with lower recall, precision, and F1-score.

While my Isolation Forest Model, achieved a higher recall and F1-score for the minority class (1).
Identified anomalies (class 1) more effectively (as seen in the confusion matrix and higher recall). 
But it had very low precision, resulting in a lower F1-score for the minority class and low overall accuracy and AUC score (0.73).

* Hence thought of ensembling XGB and Isolation Forest because ensembling models can be a good strategy, especially when individual models have complementary strengths and weaknesses.
