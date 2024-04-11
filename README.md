# Credit-Fraud

## Intro-data
The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

## Analysis in Python
I do XGBoost algorithm in Python. 

Follow the outline: 

1. Explore data analysis

2. Check the missing value

3. Split the training and testing

4. Compute the AUC and plot ROC

5. Perform the 5-folds-CV

6. Perform GridSearchCV

## Analysis in R
I do Random Forest in R.

Follow the outline:

1. Read data  Convert class to factor See variables detail 
2. Missing value  Correlation plot 
3. Split train and test 
4. Do 5-folds-CV on the train set 
5. Train the Random forest on the train set
6. Evaluate it on the test set and work out AUC/ROC curve.

## Data
https://drive.google.com/file/d/1zNTbNN-Nvt_0Zsj3XhIF1G_x6v2Ik0Cp/view?usp=drive_link
