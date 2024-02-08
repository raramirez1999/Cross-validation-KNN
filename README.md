# Cross-Validation KNN Model with R

## Introduction

This project focuses on the implementation and evaluation of a K-Nearest Neighbors (KNN) model to classify credit card dataset transactions. Utilizing the R programming language, we explore two main approaches for model validation: K-Fold Cross-Validation and Train-Validation-Test Split, to ensure our model's reliability and accuracy in predicting outcomes based on unseen data.

## Project Goals

The primary goal of this project is to demonstrate the effectiveness of the KNN algorithm in classifying data with high accuracy. We aim to:
- Implement K-Fold Cross-Validation to optimize model parameters and mitigate overfitting.
- Utilize a Train-Validation-Test Split approach to separately evaluate the model's performance on unseen data.
- Compare the results of both validation techniques to identify the most effective approach for this specific dataset.

## Methodology

We used the `kknn` library in R to build our KNN models. The dataset, `credit_card_data.txt`, was divided using two different validation techniques:

1. **K-Fold Cross-Validation:** The dataset was split into 10 folds, with each fold serving as the test set once in a rotation manner to ensure every data point was used for testing exactly once. This approach helped in assessing the model's performance across different subsets of the data.

2. **Train-Validation-Test Split:** The dataset was divided into training (60%), validation (20%), and test (20%) sets. This split allowed us to train the model, fine-tune its parameters on the validation set, and finally evaluate its performance on the test set, which mimics real-world unseen data.

## Results

- **K-Fold Cross-Validation:** Achieved an accuracy of 82.263%, demonstrating the model's robustness in handling different subsets of the data for training and testing.

- **Train-Validation-Test Split:** The validation set accuracy was 83.96947%, while the test set accuracy dropped to 51.9084%. This variance highlighted the challenges in model generalization and the importance of careful data splitting and parameter tuning.

In conclusion, the project underscores the strengths and limitations of the KNN algorithm within the context of credit card transaction classification. Through detailed experimentation with K-Fold Cross-Validation and Train-Validation-Test Split, we gained insights into model validation techniques and their impact on predictive accuracy.

