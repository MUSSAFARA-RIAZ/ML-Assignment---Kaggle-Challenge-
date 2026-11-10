# 30-Day Hospital Readmission Prediction

This repository contains my submission progression for the **Machine Learning Fall 2026 Kaggle competition at IBA Karachi**.

The task was to predict whether a patient would be readmitted within 30 days. The evaluation metric was **ROC-AUC**.

The original dataset was provided in multiple CSV files. It included around **14 tables**, such as patient information, hospital encounters, diagnoses, procedures, lab results, vitals, medications, unit transfers, prior utilization, discharge planning, hospitals, and the train/test files.

I have **not uploaded the original CSV datasets to this repository** because they were provided specifically for the course competition.

## Submission Progress

I gradually improved the solution across multiple submissions instead of jumping directly to a complex model.

The overall flow was:

**Baseline models → model tuning → feature engineering → regularization → boosting → fold averaging → LightGBM tuning → blending → stacking → larger stacking ensembles**

Some of the main experiments included:

- Logistic Regression, KNN, Decision Tree, Naive Bayes, and Random Forest
- Missing-value indicators and hyperparameter tuning
- Diagnosis and lab-based feature engineering
- L1 regularization
- XGBoost, LightGBM, CatBoost, and other boosting models
- Cross-validation based prediction averaging
- LightGBM + Logistic Regression blending
- Three-model blending with CatBoost
- Stacking using out-of-fold predictions
- Larger stacking ensembles with multiple model families
- Diagnosis-pair features in the final experiment

My Kaggle score improved from **0.72619 in the first submission** to a best score of **0.74884**.

The notebooks are kept separately so the progression of experiments and improvements can be followed submission by submission.
