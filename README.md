# Interpretable Modeling for High-Dimensional Data: Comparing Lasso Regression and Neural Networks

## Overview

This repository contains the code and results from a research study comparing the performance of Lasso regression and neural network models—specifically Convolutional Neural Networks (CNNs) and Fully Connected Neural Networks (FCNNs)—on various high-dimensional datasets. The study focuses on evaluating these models based on accuracy, efficiency, feature selection capabilities, and, importantly, their interpretability versus explainability.

## Research Summary

High-dimensional data, characterized by a large number of features relative to the number of observations, presents significant challenges in machine learning, including overfitting, increased computational complexity, and difficulties in model interpretation. While deep learning models like CNNs and FCNNs are powerful for capturing complex patterns, their lack of interpretability often limits their practical application, especially in fields where understanding the decision-making process is critical.

### Objectives
The primary goal of this research is to identify scenarios where a simpler, more interpretable model like Lasso regression can outperform or match the predictive power of deep learning models, while also being more efficient and easier to interpret. This comparison is crucial for determining the most suitable modeling approach for different types of high-dimensional data.

### Methodology
The study involved analyzing four distinct datasets:
1. **Simulation Data**: A synthetic dataset generated to evaluate feature selection capabilities in a controlled environment.
2. **Wave Energy Farm Regression Data**: A real-world dataset used to predict energy output based on various features.
3. **TCGA Stomach Cancer Data**: A high-dimensional genetic dataset used for binary classification, predicting disease-specific survival.
4. **Taiwanese Bankruptcy Data**: A financial dataset used for binary classification, predicting company bankruptcy.

For each dataset, both Lasso regression and a neural network model (CNN or FCNN) were implemented, and their performances were compared using various metrics, including accuracy, root mean squared error (RMSE), false positive/negative rates, R-squared, and computation time for both training and feature selection interpretability.

### Key Findings
- **Lasso regression** consistently demonstrated superior interpretability and efficiency, with competitive accuracy across both regression and classification tasks.
- **CNNs** and **FCNNs** offered slight advantages in predictive power in some scenarios but required significantly more computational resources for explainability using tools like SHAP.
- The study highlights the trade-offs between accuracy and interpretability, emphasizing the importance of model selection based on the specific needs of the application, particularly in high-stakes environments where transparency is critical.

## Repository Structure

The repository is organized into the following folders, each containing code and results related to a specific dataset:

- **/simulation**: Contains the code for generating synthetic datasets and comparing Lasso regression with FCNNs on feature selection and accuracy.
- **/large-scale+wave+energy+farmn**: Includes the code for analyzing the Wave Energy Farm dataset using Lasso regression and CNN models, focusing on regression performance metrics.
- **/tcga stomach cancer**: Contains the code for the binary classification of the TCGA stomach cancer dataset, comparing Lasso regression and FCNNs.
- **/bankrupt data**: Includes the code for the binary classification of the Taiwanese Bankruptcy dataset, focusing on the comparison between Lasso regression and FCNNs.

Each folder contains a README file with detailed information about the dataset, the methods used, the code implementation, and a summary of the results.

## Conclusion

This repository provides a comprehensive exploration of the trade-offs between simple, interpretable models and complex, explainable deep learning models when applied to high-dimensional data. The findings contribute to the ongoing discussion about model selection, offering insights that can guide practitioners in choosing the most appropriate model based on their specific requirements for accuracy, efficiency, and interpretability.

## Acknowledgments

This research was supported by the National Science Foundation under Research Experience for Undergraduates (REU) Grant No. 2244480.
