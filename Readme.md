# Customer Churn Prediction

## Project Overview

This project builds a complete machine learning pipeline to predict customer churn for a telecommunications company. The model identifies customers who are likely to cancel their service, enabling the business to proactively offer retention incentives.

## Dataset

The project uses the **Telco Customer Churn** dataset, which contains 7,043 customer records and 21 features detailing customer demographics, services, and account information. The target variable is `Churn`.

## Methodology \& Pipeline

The project follows a structured pipeline to ensure robust and reliable model performance.

```
[Data Loading & Exploration] --> [Data Cleaning & Preprocessing] --> [Feature Engineering] --> [Train-Test Split] --> [Feature Scaling] --> [SMOTE for Imbalance] --> [Model Training & Evaluation] --> [Hyperparameter Tuning] --> [Final Model Selection]
```


## Techniques Used

* **Feature Engineering**: Created new features like `tenure_group` to capture non-linear relationships and improve model accuracy.
* **StandardScaler**: Scaled numerical features to a common range. This is crucial for distance-based algorithms like SVM and helps Logistic Regression converge faster.
* **SMOTE (Synthetic Minority Oversampling Technique)**: Addressed class imbalance by generating synthetic samples of the minority class (churned customers). This helps the model learn to identify churners effectively.
* **Hyperparameter Tuning**: Systematically searched for the best model settings (hyperparameters) using `GridSearchCV`. This process optimizes the model to achieve the best possible performance on unseen data.


## Results

The final model, a **Logistic Regression** classifier, achieved an **AUC score of 84.5%**. This indicates a strong ability to distinguish between customers who will churn and those who will not.
