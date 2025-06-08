---
title: "Customer Churn Prediction"
description: "Machine learning model to predict customer churn using behavioral data"
tech_stack: "Python, Scikit-learn, Pandas, Matplotlib"
duration: "3 weeks"
status: "Completed"
github_url: "https://github.com/yourusername/churn-prediction"
date: 2024-01-15
---

# Customer Churn Prediction

## Project Overview

Developed a machine learning model to predict customer churn for a telecommunications company, helping reduce customer attrition by 15%.

## Problem Statement

The company was experiencing high customer churn rates (25% annually) and needed to identify at-risk customers to implement targeted retention strategies.

## Dataset

- **Size**: 7,043 customers
- **Features**: 21 variables including demographics, services, and usage patterns
- **Target**: Binary churn indicator (Yes/No)

## Methodology

### 1. Exploratory Data Analysis
- Analyzed customer demographics and service usage patterns
- Identified key factors correlated with churn
- Visualized data distributions and relationships

### 2. Data Preprocessing
- Handled missing values and outliers
- Encoded categorical variables
- Scaled numerical features
- Split data into training/validation/test sets

### 3. Model Development
Tested multiple algorithms:
- Logistic Regression
- Random Forest
- Gradient Boosting (XGBoost)
- Support Vector Machine

### 4. Model Evaluation
- Cross-validation for model selection
- Performance metrics: Accuracy, Precision, Recall, F1-score
- ROC-AUC analysis

## Results

- **Best Model**: XGBoost Classifier
- **Accuracy**: 84.2%
- **Precision**: 81.7%
- **Recall**: 78.9%
- **F1-Score**: 80.3%

## Key Insights

1. **Contract Type**: Month-to-month contracts showed highest churn risk
2. **Payment Method**: Electronic check users more likely to churn
3. **Tenure**: Customers with <1 year tenure had 3x higher churn rate
4. **Support Calls**: Customers with >3 support calls in 30 days showed elevated risk

## Business Impact

- Enabled proactive customer retention campaigns
- Reduced churn rate from 25% to 21.25% (15% improvement)
- Estimated annual savings: $2.3M in retained revenue

## Technical Details

```python
# Key libraries used
import pandas as pd
import numpy as np
from sklearn.ensemble import XGBClassifier
from sklearn.model_selection import train_test_split
from sklearn.metrics import classification_report

# Model training snippet
model = XGBClassifier(
    max_depth=6,
    learning_rate=0.1,
    n_estimators=100
)
model.fit(X_train, y_train)
```

## Visualizations

*Note: Visualizations and charts would be displayed here in a real project. This includes:*
- Churn rate analysis by contract type
- Feature importance rankings from the XGBoost model
- ROC curves and confusion matrices
- Customer segmentation plots

## Future Improvements

- Implement real-time scoring pipeline
- A/B test retention campaigns
- Integrate with CRM system
- Add additional behavioral features

[View Code on GitHub]({{ page.github_url }}) | [Interactive Dashboard](link-to-dashboard) 