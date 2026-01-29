# AI & ML Internship — Task 9
## Random Forest: Credit Card Fraud Detection
### Submitted By: Pranav S P

---

## 1. Objective

The objective of this task is to detect fraudulent credit card transactions using an ensemble learning approach.
This task focuses on handling extreme class imbalance, selecting appropriate evaluation metrics, and building a robust fraud detection model using Random Forest.

---

## 2. Dataset Description

Dataset Used: Kaggle Credit Card Fraud Detection Dataset  

- Total transactions: ~284,000
- Fraud cases: ~492
- Target column: `Class`
  - 0 → Legitimate transaction
  - 1 → Fraudulent transaction

The dataset is highly imbalanced, which makes accuracy an unreliable metric.

---

## 3. Class Imbalance Analysis

- Fraud transactions represent approximately 0.17% of the data.
- A bar chart was used to visualize the imbalance.
- This confirms the need for:
  - Stratified sampling
  - Precision, Recall, and F1-score–based evaluation

Accuracy alone would fail to detect fraud cases effectively.

---

## 4. Feature Preparation

- The target variable `Class` was separated from input features.
- No manual feature removal was done since most features are anonymized PCA components.
- Feature and target separation was documented as an artifact.

---

## 5. Train–Test Split Strategy

- The dataset was split using stratified sampling (80% train, 20% test).
- Stratification ensured that fraud ratios remained consistent in both training and testing sets.

This is critical for reliable fraud evaluation.

---

## 6. Baseline Model

A Logistic Regression model was trained as a baseline.

- Purpose: Establish a performance reference point
- Observation: High accuracy but poor recall for fraud cases

This demonstrated why baseline models are insufficient for fraud detection.

---

## 7. Random Forest Model

- Model: Random Forest Classifier
- Number of trees (`n_estimators`): 100
- Parallel processing enabled

Random Forest improved fraud detection by:
- Capturing non-linear patterns
- Reducing overfitting through ensemble learning

---

## 8. Model Evaluation

Evaluation focused on:
- Precision
- Recall
- F1-score

Random Forest outperformed the baseline model, especially in recall for fraud cases.

---

## 9. Feature Importance Analysis

- Top contributing features were identified using feature importance scores.
- A bar chart was generated to visualize the most influential fraud indicators.

This improves interpretability of the ensemble model.

---

## 10. Model Persistence

- The trained Random Forest model was saved using `joblib`.
- This enables future reuse without retraining.

---

## 11. Conclusion

This task demonstrated the importance of:
- Handling imbalanced data correctly
- Using ensemble models for complex detection tasks
- Evaluating models with appropriate metrics

The Random Forest model provides a strong foundation for real-world fraud detection systems.
