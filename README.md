# MNIST Digit Classification using K-Nearest Neighbors (KNN)

## Problem Statement
The MNIST dataset consists of grayscale images of handwritten digits (0-9), each represented as a 28x28 pixel grid. The goal is to build a K-Nearest Neighbors (KNN) classifier to identify the digit in each image based on pixel intensity values. This involves preprocessing the high-dimensional dataset, tuning hyperparameters, and evaluating the model's accuracy on a test set.

## Objective
This project demonstrates the application of the KNN algorithm for digit classification with a focus on preprocessing, feature selection, and cross-validation to achieve robust performance.

## Workflow
1. **Preprocess the MNIST dataset:**
   - Normalize pixel intensity values using Min-Max Scaling.
   - Remove low-variance features (<300 variance threshold) to reduce dimensionality and computational cost.
2. **Perform hyperparameter tuning:**
   - Use GridSearchCV with 5-fold cross-validation to optimize hyperparameters (`n_neighbors`, `weights`, and `metric`).
3. **Evaluate the final model:**
   - Test accuracy: 97.31%
   - Precision, recall, and F1-scores exceed 0.97 for all classes.

## Results
- **Test Accuracy:** 97.31%
- The model shows robust performance with high precision, recall, and F1-scores for all digit classes.
