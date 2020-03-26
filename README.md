# SageMaker Supervised Learning

## Project: Payment Fraud Detection

### Source 

Project 3 from Udacity's [Machine Learning Engineer Nanodegree](https://www.udacity.com/course/machine-learning-engineer-nanodegree--nd009t)

### Description

Built a binary classification model using Amazon SageMaker to identify transactions as either fraudulent or valid. 

- Acquired SageMaker session, role, and default bucket 
- Loaded and explored data (calculated that 0.0017% of the data was fraudulent) 
- Created a Linear Learner Estimator, converted data into RecrodSet format, trained it using a ml.c4.xlarge instance, and deployed it using a ml.t2.medium instance
- Evaluated model and found metrics: Recall of 0.773, Precision of 0.768, and Accuracy of 0.999
- Created, trained, and deployed a Linear Learner tuned for highest maximum possible precision with a recall of 0.9 
- Created, trained, and deployed a Linear Learner tuned for highest maximum possible recall with a precision of 0.9 
- Addressed class imbalance issue 

### Data 

The payment fraud data set (Dal Pozzolo et al. 2015) was downloaded from [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud/data). This has features and labels for thousands of credit card transactions, each of which is labeled as fraudulent or valid. In this notebook, we'd like to train a model based on the features of these transactions so that we can predict risky or fraudulent transactions in the future. 
