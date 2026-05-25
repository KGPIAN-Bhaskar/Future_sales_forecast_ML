# 📈 Sales Forecasting Using Machine Learning

## Project Overview

This project develops a machine learning-based sales forecasting system that predicts future sales trends using historical sales data. The objective is to improve business decision-making through accurate demand forecasting and provide useful business insights.

The project follows a complete machine learning workflow including:

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Model Development
* Hyperparameter Tuning
* Future Forecasting
* Business Recommendations

---

## Problem Statement

Businesses often struggle to estimate future sales accurately because customer demand changes due to multiple factors such as product categories, discounts, seasonal trends, and market conditions.

Incorrect sales prediction may result in:

* Inventory shortages
* Overstocking
* Increased operational costs
* Reduced business efficiency

This project aims to solve this problem using machine learning techniques.

---

## Objectives

* Analyze historical sales data
* Perform data preprocessing and feature engineering
* Build baseline and advanced machine learning models
* Compare model performance
* Predict future sales trends
* Generate business recommendations

---

## Dataset Features

Dataset columns used:

* Order Date
* Ship Date
* Product Category
* Quantity
* Discount
* Profit
* Shipping Cost
* Region
* Market
* Order Priority
* Sales

---

## Data Preprocessing

Data preprocessing steps performed:

### Missing Value Handling

* Missing values detected using:

```python
df.isnull().sum()
```

* Product names filled using mode imputation.

### Duplicate Removal

* Duplicate records checked and removed.

### Outlier Detection

Methods used:

* Boxplot
* Interquartile Range (IQR)

### Log Transformation

Applied log transformation to reduce skewness and handle extreme sales values.

---

## Exploratory Data Analysis (EDA)

EDA findings:

* Sales distribution was positively skewed
* Product categories significantly influenced sales
* Discounts affected purchasing behavior
* Quantity strongly impacted sales
* Sales values showed fluctuations

---

## Feature Engineering

Features created:

* Month
* Day
* Weekday
* Quarter
* Year

Categorical variables were transformed using:

* One-Hot Encoding

Feature selection was applied to reduce unnecessary variables.

---

## Models Implemented

### 1. Multiple Linear Regression

Used as baseline model.

Performance:

* R² Score: 0.76
* RMSE: 230.88

---

### 2. Random Forest Regression

Used as advanced model.

Base Model Performance:

* R² Score: 0.8734

Tuned Model Performance:

* R² Score: 0.8736

Hyperparameter tuning performed using:

```python
GridSearchCV
```

---

## Evaluation Metrics

Performance evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

---

## Business Insights

* Product categories significantly influence sales.
* Quantity affects demand patterns.
* Discounts influence customer behavior.
* Random Forest captured complex sales patterns better than Linear Regression.

---

## Future Forecasting

Future sales trends were generated using historical behavior and recent patterns.

Forecasting includes:

* Future sales predictions
* Confidence intervals
* Trend visualization

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

---

## Project Structure

```bash
Sales-Forecasting/
│
├── data/
├── notebooks/
├── models/
├── images/
├── sales_forecasting.ipynb
├── README.md
└── requirements.txt
```

---

## Future Improvements

* Implement ARIMA
* Implement LSTM
* Include holiday effects
* Add external economic indicators
* Deploy as web application

---

## Author

Bhaskar Mandal

GitHub:
https://github.com/KGPIAN-Bhaskar

LinkedIn:
https://www.linkedin.com/in/bhaskar-mandal/

---

⭐ If you found this project useful, please consider giving a star.
