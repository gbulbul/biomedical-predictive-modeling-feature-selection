# Biomedical Predictive Modeling and Feature Selection

## Problem Description
This project focuses on a binary classification problem in a biomedical context, where the goal is to predict disease-related outcomes based on a set of clinical and biological features. The dataset includes multiple predictors that may vary in relevance, redundancy, and predictive power.

## Approach
We implemented and compared several machine learning models, including Random Forest, XGBoost, and Logistic Regression, to evaluate their performance in predicting the target outcome.

A key focus of this study is feature selection and model robustness. We constructed both full models (using all available features) and reduced models (using a subset of the most important predictors based on feature importance techniques). This allowed us to systematically assess how model performance changes with feature reduction.

## Results
- Random Forest: 0.94 (stable across full and reduced feature sets)
- XGBoost: 0.96 (full model), 0.92 (reduced model)
- Logistic Regression: 0.92 (both full and reduced models)

The full implementation is available in the notebook.

## Interpretation of Results
The results show that Random Forest and Logistic Regression provide stable performance regardless of feature reduction, indicating robustness to changes in the predictor set. In contrast, XGBoost achieves the highest accuracy when using the full feature set but shows a noticeable decrease in performance when features are reduced.

These findings highlight the importance of feature selection in balancing model performance and stability. While more complex models may achieve higher accuracy, simpler or more robust models may generalize better when working with reduced or noisy feature sets.
