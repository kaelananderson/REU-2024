# Wave Energy Farm Regression

## Description of the Dataset
The Large-scale Wave Energy Farm dataset, sourced from UC Irvine’s Machine Learning Repository, contains 63,600 instances and 149 features. The dataset represents wave farms’ wave energy converters (WECs) coordination, individual power output, q-factor, and total farm power output. The objective is to predict the total energy power output of each farm.

## Comparison Performed
The comparison involves evaluating the performance of Lasso regression and Convolutional Neural Networks (CNNs) on this regression task. The goal is to determine which model provides better predictive accuracy, efficiency, and interpretability when applied to this high-dimensional dataset.

## Summary of Code
The code in this folder implements the Lasso regression model and a 1-dimensional CNN model for the regression task. It includes data preprocessing steps, model training, and evaluation using metrics such as RMSE and estimation time.

## Summary of Results
Lasso regression outperformed the CNN model in all metrics except the False Positive Rate (FPR). The Lasso model demonstrated higher efficiency and interpretability, making it a more suitable choice for this regression task.
