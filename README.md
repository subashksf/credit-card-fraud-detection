# credit-card-fraud-detection
Classification model to detect fraud in an anonymized credit card dataset

## Dataset
The dataset was acquired from [kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud/data).

The dataset contains the below attributes:-

+ Time: Number of seconds elapsed between this transaction and the first transaction in the dataset
+ Anonymized columns V1 to V28
+ Amount: Transaction amount
+ Class: label that marks the transaction as fraudulent
  + 1: fraudulent
  + 0: not fraudulent

## Data Preprocessing
I used the below data preprocessing techniques:-
+ determined the covariance matrix, and dropped the columns with covariance less than 0.01 with the label.
+ scaled the independent numerical columns to normalize them.

## Models
I built two models to compare the performance and efficiency - Decision Tree (a very simple one, without any hyperparameter tuning) and XGBoost. The confusion matrix and accuracy can be found in the notebook.
