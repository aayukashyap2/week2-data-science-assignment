# week2-data-science-assignment
# Tesla Deliveries ML Pipeline (2015–2025)

## Project Overview

This project demonstrates an end-to-end Machine Learning pipeline built using Tesla Deliveries and Production Data (2015–2025).

The objective of this project is to analyze Tesla's delivery and production trends, perform feature engineering, build predictive machine learning models, evaluate model performance, and generate delivery forecasts using historical data.

The project covers the complete data science workflow, including data preprocessing, exploratory data analysis (EDA), feature engineering, model training, validation, hyperparameter tuning, forecasting, and time series analysis.

---

## Dataset

**Dataset Used:** Tesla EA Deliveries and Production Data (2015–2025)

The dataset contains information related to:

* Year and Month
* Region
* Tesla Vehicle Models
* Estimated Deliveries
* Production Units
* Average Vehicle Price
* Battery Capacity
* Vehicle Range
* CO₂ Saved
* Charging Stations
* Source Type

---

## Project Workflow

### 1. Data Loading

* Imported dataset from Kaggle
* Verified dataset structure and dimensions
* Inspected columns and data types

### 2. Data Cleaning

* Checked for missing values
* Checked for duplicate records
* Verified data consistency

### 3. Exploratory Data Analysis (EDA)

Performed visual analysis to understand:

* Deliveries by Vehicle Model
* Deliveries by Region
* Correlation between numerical features
* Production vs Deliveries relationship
* Tesla Delivery Trends over Time

### 4. Feature Engineering

Created additional features to improve model performance:

* Label Encoding for categorical variables
* Lag Features
* Rolling Mean Features

### 5. Machine Learning Modeling

#### Linear Regression

* Chronological Train-Test Split
* Model Training
* Performance Evaluation

#### Cross Validation

* 5-Fold Cross Validation
* Model Stability Assessment

#### Random Forest Regression

* Ensemble Learning Approach
* Performance Comparison

### 6. Hyperparameter Tuning

* GridSearchCV
* Optimal Parameter Selection

### 7. Time Series Analysis

* Augmented Dickey-Fuller (ADF) Stationarity Test
* Verification of time series behavior

### 8. Forecasting

* Future delivery prediction
* Actual vs Predicted comparison

---

## Results

### Linear Regression Performance

| Metric   | Value  |
| -------- | ------ |
| R² Score | 0.9889 |
| MAE      | ~318   |
| RMSE     | ~387   |

### Cross Validation

| Metric           | Value   |
| ---------------- | ------- |
| Average R² Score | ~0.9903 |

### Random Forest Performance

| Metric   | Value  |
| -------- | ------ |
| R² Score | 0.9872 |

### Stationarity Test

* ADF Statistic: -53.83
* P-Value: 0.0
* Result: Stationary Time Series

---

## Key Insights

* Production Units show a strong positive relationship with Estimated Deliveries.
* Historical delivery data is highly useful for forecasting future deliveries.
* Tesla delivery trends remain relatively stable across regions.
* Machine learning models achieved excellent predictive performance with R² scores above 0.98.
* Time-series analysis confirmed stationarity of delivery data.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Statsmodels
* Kaggle Notebook

---

## Repository Structure

```text
Tesla-Deliveries-ML-Pipeline/
│
├── Tesla_Deliveries_ML_Pipeline.ipynb
├── README.md
└── Dataset Reference
```

---
Kaggle Notebook:- 
https://www.kaggle.com/code/aayushkumar681/week2-aayush-ml-pipeline

## Conclusion

This project successfully demonstrates the implementation of a complete Machine Learning pipeline for Tesla delivery forecasting. Through data preprocessing, exploratory analysis, feature engineering, regression modeling, hyperparameter tuning, and time-series analysis, the project achieved high prediction accuracy and generated meaningful business insights.

---

### Author

**Aayush Kumar**

Data Science Assignment – End-to-End ML Pipeline on Tesla Deliveries & Production Data
