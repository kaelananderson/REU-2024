# Simulation Dataset

## Description of the Dataset
The simulation dataset was generated using a custom Python function designed to create a synthetic dataset with a defined number of true effective predictors and non-effective (noisy) predictors. The dataset is used to simulate high-dimensional data scenarios and evaluate the performance of feature selection methods.

## Comparison Performed
The comparison focuses on evaluating the feature selection capabilities and overall performance of Lasso regression and Fully Connected Neural Networks (FCNNs). The goal is to determine how well each model identifies true effective predictors while minimizing the impact of noisy predictors.

## Summary of Code
The code in this folder generates the synthetic dataset, implements both Lasso regression and FCNN models, and evaluates their performance using metrics such as R-squared, Root Mean Squared Error (RMSE), and feature selection accuracy. The code also includes the use of the SHAP library to explain the decisions of the FCNN model.

## Summary of Results
Both Lasso and FCNN models produced nearly identical results in terms of accuracy and feature selection capabilities. However, Lasso demonstrated superior interpretability with almost instantaneous feature selection insights, while FCNN required significantly more computational time to generate SHAP values for explainability.
