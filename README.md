# Credit Card Fraud Detection

## Introduction

This project focuses on identifying fraudulent transactions with credit cards using machine learning techniques. Our goal is to construct a fraud detection system that labels transactions as either fraudulent or legitimate. Notably, the dataset exhibits a low prevalence of fraud, which we address by balancing it through resampling techniques.

## Data Understanding

The dataset comprises 555,719 transactions, each described by 23 attributes (22 predictive and 1 target variable). We perform data preprocessing in R, utilizing libraries such as `caret`, `tidyverse`, `randomForest`, and `pROC`, among others. After loading and initial inspection, the dataset undergoes several preprocessing steps to prepare it for analysis, including handling missing values, converting features to appropriate data types, and creating new features for model training.

## Exploratory Data Analysis (EDA)

Before model training, we explore the dataset to identify any patterns or trends indicative of fraudulent transactions. This involves analyzing the distribution of transaction amounts, examining the prevalence of fraud across different categories, and investigating the relationship between fraud and variables such as transaction hour, cardholder age, and transaction category.

## Balancing the Dataset and Feature Selection

Given the imbalanced nature of the dataset, we generate a new dataset with a 60:40 balance between non-fraudulent and fraudulent transactions. This step is crucial for training our machine learning models on a dataset that better represents real-world conditions. We also select relevant features for the models, excluding unnecessary variables to improve model performance and interpretability.

## Machine Learning Modeling

We train and evaluate four different models: Logistic Regression, Decision Trees, K-Nearest Neighbors (KNN), and Random Forests. Each model is assessed on both the balanced and unbalanced datasets. Model performance is compared using metrics such as accuracy, sensitivity, specificity, and the area under the ROC curve (AUC). The best-performing model is selected based on these metrics.

## Model Evaluation

After training and testing, we compare the models to identify which provides the most accurate and reliable fraud detection. We discuss the performance of each model, highlighting their strengths and limitations in the context of fraud detection.

## Conclusion

The project concludes with a discussion of the findings, including the effectiveness of the selected model, potential improvements, and recommendations for deploying the fraud detection system in a real-world scenario.

## Dependencies

- R version 4.3.2 or later
- R packages: `caret`, `tidyverse`, `randomForest`, `corrplot`, `rpart`, `kernlab`, `pROC`, `ROSE`, `lubridate`, `class`
