# Letter Recognition ML Capstone

## Overview
This repository contains a capstone project focused on classifying handwritten letters using multiple machine learning models. The project evaluates and compares the performance of SVM, Random Forest, and KNN models, and includes a feature importance analysis to provide insights into key predictive features.

## Objective
- **Evaluate and compare** multiple machine learning models for handwritten letter classification on a 26-class dataset.
- **Conduct feature importance analysis** to identify key predictors and enhance model interpretability.

## Data Description
The dataset, taken from the UCI repository, consists of handwritten alphabet images (A–Z), where each image is converted into an m×n pixel grid. Pixel values indicate the density of the ink (with 0 for blank areas). From these processed images, 16 numerical features are extracted (e.g., box width, mean variance ratio), which serve as inputs for the classification models.

## Approach
1. **Data Preparation:**  
   - Loaded and explored the dataset.
   - Scaled the 16 numeric features using `StandardScaler`.

2. **Model Comparison:**  
   - Evaluated baseline models (SVM, Random Forest, KNN, Logistic Regression) using 5-fold cross-validation.

3. **Hyperparameter Tuning:**  
   - Optimized SVM, Random Forest, and KNN using GridSearchCV to find the best parameters.

4. **Evaluation:**  
   - Compared final test accuracies, confusion matrices, and classification reports to identify the best-performing model.

5. **Feature Importance Analysis:**  
   - Used Random Forest’s `feature_importances_` attribute to identify the most influential features, aiding in model interpretability.

## Final Results
- **Tuned SVM Test Accuracy:** ~97.25%
- **Tuned Random Forest Test Accuracy:** ~96.27%
- **Tuned KNN Test Accuracy:** ~95.10%

The SVM model achieved the highest accuracy and demonstrated balanced performance across all 26 classes.


