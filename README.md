# Health Insurance Charges Prediction and Analysis

This project aims to analyze the factors affecting health insurance charges and predict them using machine learning and deep learning models. The goal is to identify the key contributors to insurance costs, helping companies make more informed decisions regarding pricing and risk assessment.

---

## Project Objectives

- Explore the dataset (EDA)
- Check and preprocess missing or erroneous data
- Analyze and visualize relationships between factors
- Predict health insurance charges using machine learning models:
  - Linear Regression
  - Decision Tree / Random Forest
  - XGBoost or other advanced models
- Evaluate model performance (R², MAE, MSE, etc.)
- Interpret the models and identify important features
- Draw conclusions and recommendations
- (Optional) Share findings via report or presentation

---

## Dataset Features

| Column | Description |
|--------|-------------|
| Age | Age of the insurance holder |
| Sex | Gender |
| BMI | Body Mass Index |
| Children | Number of children covered |
| Smoker | Whether the person smokes |
| Region | Residential region |
| Charges | Health insurance charges (target variable) |

---

## Model Performance

| Model | R² | RMSE | MAE |
|-------|----|------|-----|
| XGBRegressor | 0.941776 | 2616.94 | 1034.31 |
| Decision Tree | 0.936599 | 2730.81 | 540.79 |
| Extra Tree | 0.934633 | 2772.82 | 573.24 |
| Gradient Boosting | 0.876721 | 3807.92 | 2102.69 |
| AdaBoost | 0.821251 | 4585.28 | 2661.31 |
| KNeighborsRegressor | 0.790895 | 4959.36 | 3962.34 |
| SGD | 0.745432 | 5472.00 | 3847.38 |
| Lasso | 0.744107 | 5486.22 | 3926.95 |
| Linear | 0.744093 | 5486.37 | 3928.45 |
| Ridge | 0.743949 | 5487.91 | 3926.91 |
| ElasticNet | 0.270318 | 9264.26 | 6920.40 |
| SVR | -0.064211 | 11188.14 | 7429.05 |
| MLP Regressor | -0.744711 | 14325.37 | 9680.15 |

**Insights:**

- **Best Performing Model:** XGBRegressor with R² ≈ 0.942
- **Decision Tree & Extra Tree:** High accuracy (R² ≈ 0.935)
- **Linear Models (Linear, Ridge, Lasso):** Moderate performance (R² ≈ 0.744)
- **Low Performance:** SVR and MLP Regressor unsuitable for this dataset (negative R²)

---

## Deep Learning Model Performance

- **Model Type:** Deep Learning (Multilayer Perceptron)  
- **R² Score:** 0.843

**Interpretation:**

- The model explains approximately 84% of variance in the dataset.  
- Deep learning predicts health charges well but still leaves some variation unexplained.  
- Accuracy can be further improved by:
  - Feature engineering
  - Hyperparameter tuning
  - Using more data or alternative architectures

---

## Data Preprocessing

- **Missing Values:** None  
- **Categorical Variables:** Converted to dummy variables  
- **Numerical Variables:** Scaled appropriately  
- **Outliers:** Filtered based on 97th percentile

---

## Feature Engineering

- No additional features created; all existing columns were used

---

## Summary & Recommendations

- Machine learning models can accurately predict health insurance charges.  
- **Recommended Models:** XGBRegressor, Decision Tree, Extra Tree  
- Deep learning models provide competitive predictions but slightly lower than XGBRegressor  
- To improve performance:
  - Perform additional feature engineering
  - Optimize model parameters
  - Incorporate more data sources

**Conclusion:**  
The models developed in this project can guide health insurance companies in pricing strategies and risk assessment processes.
