# Sampling Techniques For Imbalanced Dataset

## Introduction
This assignment shows the various oversampling and undersampling techniques to apply on imbalanced dataset in Machine Learning. The dataset used here is Credit Card Dataset. The dataset contains 772 observations and 31 features. It is a binary classification dataset with 763 observations belonging to class 0 and only 9 observations belong to class 1. Because of such a high imbalance, the following sampling techniques are used.

## Sampling Techniques
A total of 5 sampling techniques are used on the dataset which are as follows:

1. Random Under sampling
2. Random Over sampling
3. Tomek Links sampling
4. SMOTE(Synthetic Minority Oversampling Technique)
5. NearMiss sampling

After applying the above techniques, n samples are randomly chosen from the generated balanced dataset (except for Tomek link sampling). n is calculated as follows:

![n = (z**2 * p * (1-p) )//(e**2)](./sample_images/n.png)

## Model training
After appling the sampling techniques, the following 5 Machine Learning models are training on the dataset:
1. K Nearest Neighbours
2. Random Forest Classifier
3. Xgboost Classifier
4. Support Vector Classifier
5. Naive Bayes Classifier
The accuracy scores of all the models are recorded in a Dataframe which is as follows:

![Result Dataframe](./sample_images/result.png)

## Conclusion
From the above table, it is clearly visible the all models perform significantly better on Tomek Link sampling technique. The maximum accuracy is 0.9806 which is achieved on Tomek Link sampling by 4 out of 5 Models.