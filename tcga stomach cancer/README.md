# TCGA Stomach Cancer Binary Classification

## Description of the Dataset
The TCGA stomach cancer dataset includes gene expression data from 20,531 features and 379 instances. The dataset is used to predict disease-specific survival (DSS) in patients, with the goal of classifying whether a patient will survive or die from stomach cancer.

## Comparison Performed
The comparison examines the performance of Lasso regression versus Fully Connected Neural Networks (FCNNs) in binary classification, focusing on metrics such as accuracy, False Negative Rate (FNR), and interpretability.

## Summary of Code
The code in this folder implements the Lasso regression and FCNN models for binary classification. It includes data preprocessing, model training, ROC curve analysis for threshold determination, and evaluation of classification metrics such as accuracy, FNR, and AUC.

## Summary of Results
The FCNN model outperformed Lasso in most metrics except for FNR and estimation time. Notably, the Lasso model achieved a perfect FNR, which is critical in predicting whether a patient will die from cancer. Despite FCNN’s higher overall accuracy, Lasso’s interpretability and zero false negatives make it a compelling choice in this healthcare scenario.
