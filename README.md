# Machine Learning & Feature Selection in Biomedical Data

## Overview

This project presents a comparative analysis of machine learning models and feature selection techniques applied to a biomedical dataset. The primary objective is to evaluate whether a reduced set of predictors can maintain predictive performance while improving model interpretability.

The analysis includes Random Forest, XGBoost, and Logistic Regression models, each trained on both the full feature set and a reduced subset of top predictors identified through feature importance analysis. 

## Problem Definition

This study addresses a binary classification problem, where the goal is to predict a dichotomous outcome using a set of biomedical features. The binary outcome enables the evaluation of model performance using classification metrics such as accuracy.0

---

## Methods

### Machine Learning Models
- Random Forest
- XGBoost
- Logistic Regression

Each model was trained and evaluated using:
- Full feature set
- Top 10 selected features (based on importance)

---

### Feature Selection

Feature importance techniques were used to identify the most relevant predictors. The top 10 features were selected and used to train reduced models.

---

### Causal Analysis

Causal inference methods (DoWhy) were applied to estimate the potential effect of individual predictors on the outcome variable.

---

## Results

### Model Performance

| Model                | Full Features | Top Features |
|---------------------|-------------|-------------|
| Random Forest       | 0.96        | 0.96        |
| XGBoost             | 0.96        | 0.96        |
| Logistic Regression | 0.94        | 0.92        |

---

## Key Findings

- Random Forest and XGBoost maintained identical performance after feature reduction.
- Logistic Regression showed a slight decrease in performance, indicating higher sensitivity to feature selection.
- A small subset of predictors captures most of the predictive signal.
- Feature selection significantly improves interpretability without major loss of accuracy.

---

## Causal Insights

- Key features (e.g., concave-related variables) consistently showed stronger estimated effects.
- Results were stable across different feature subsets.
- Findings align with machine learning feature importance rankings.

⚠️ Note: Estimated effects represent associations under model assumptions and do not imply definitive causality.

---

## Conclusion

This project demonstrates that:

- Feature selection can significantly reduce model complexity without sacrificing performance.
- Tree-based models are robust to feature reduction.
- A compact set of predictors is sufficient for high predictive accuracy.
- Combining machine learning with causal analysis provides deeper insight into data structure.

---

## Repository Structure
ter when working with reduced or noisy feature sets.
