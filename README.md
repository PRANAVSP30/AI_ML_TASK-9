# AI & ML Internship — Task 9
## Random Forest: Credit Card Fraud Detection

### Submitted by : **Pranav S P**

---

##  Task Overview

This project implements a **Random Forest Classifier** to detect fraudulent credit card transactions.
Special emphasis is placed on handling extreme class imbalance and using correct evaluation metrics.

---

##  Key Concepts Covered

- Fraud Detection
- Class Imbalance
- Stratified Train–Test Split
- Ensemble Learning
- Random Forest
- Feature Importance
- Model Persistence

---

##  Project Structure
```
AI_ML_Task9/
│
├── data/
│ └── creditcard.csv
│
├── notebooks/
│ └── fraud_detection_random_forest.ipynb
│
├── outputs/
│ ├── artifacts/
│ │ ├── class_imbalance_summary.txt
│ │ ├── feature_target_info.txt
│ │ ├── train_test_split_summary.txt
│ │ ├── baseline_logistic_report.txt
│ │ ├── random_forest_report.txt
│ │ ├── feature_importance.txt
│ │ └── model_comparison.txt
│ │
│ └── visualizations/
│ ├── class_imbalance.png
│ └── feature_importance.png
│
├── models/
│ └── random_forest_fraud.pkl
│
├── reports/
│ └── task9_report.md
│
└── README.md

```
---

##  Workflow Summary

1. Loaded the Kaggle Credit Card Fraud dataset
2. Analyzed and visualized class imbalance
3. Separated features and target variable
4. Applied stratified train–test split
5. Trained a baseline Logistic Regression model
6. Trained a Random Forest model with 100 trees
7. Evaluated using precision, recall, and F1-score
8. Visualized feature importances
9. Compared baseline vs Random Forest
10. Saved the trained model using joblib

---

##  Why Accuracy Is Misleading

- Fraud cases are extremely rare
- A model predicting all transactions as non-fraud achieves high accuracy
- Precision and Recall are more meaningful for fraud detection

---

## Tools & Technologies Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Joblib
- Jupyter Notebook
- Git & GitHub

---

##  Final Outcome

This project demonstrates a complete fraud detection pipeline using ensemble learning.
It highlights the importance of proper evaluation and real-world ML practices.


