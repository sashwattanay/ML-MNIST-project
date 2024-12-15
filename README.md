# MNIST Digit Classification using K-Nearest Neighbors (KNN)

## Problem Statement
The goal of this project is to classify handwritten digits from the MNIST dataset using the K-Nearest Neighbors (KNN) algorithm. The dataset consists of grayscale images of digits (0-9), each represented as a 28x28 pixel grid. The challenge is to preprocess this high-dimensional dataset, optimize the model for accuracy, and evaluate its performance on a test set.

## Objective
This project demonstrates the use of KNN for digit classification, focusing on preprocessing, hyperparameter tuning, and model evaluation to achieve robust performance. The target accuracy is 97% or higher on the test set.

## Workflow
1. **Data Preprocessing:**
   - Loaded the MNIST dataset with 70,000 samples and 784 features per sample (28x28 pixels).
   - Applied Min-Max Scaling to normalize feature values between 0 and 1.
   - Removed low-variance features (<300 variance threshold) to reduce dimensionality.
   
2. **Feature Engineering:**
   - Visualized feature variance to identify and drop low-information features.

3. **Model Selection and Hyperparameter Tuning:**
   - Used GridSearchCV with 5-fold cross-validation to tune hyperparameters:
     - `n_neighbors`: Number of neighbors to consider.
     - `weights`: Uniform or distance-based weighting.
     - `metric`: Euclidean or Manhattan distance.
   - Selected the best hyperparameters based on cross-validation accuracy.

4. **Evaluation:**
   - Achieved a test accuracy of 97.31%.
   - Generated confusion matrix and classification report for detailed performance analysis.

## Results
- **Final Test Accuracy:** 97.31%
- Precision, recall, and F1-scores exceeded 0.97 for all digit classes.

## File Outputs
- **`best_knn_model.pkl`:** The trained KNN model with the best hyperparameters, saved for reuse.
