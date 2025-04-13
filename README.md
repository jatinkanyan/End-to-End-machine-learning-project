# 🚲 Bike Sharing Demand Prediction

This project aims to analyze and predict bike-sharing demand based on historical usage data and environmental conditions. It involves exploratory data analysis (EDA) and regression modeling to understand patterns in bike rentals and build a predictive model.

## 📊 Overview

- **Project Type**: Individual
- **Objective**: Predict daily bike rental counts using regression models
- **Dataset**: 8,760 records × 14 attributes (1 year of hourly data)
- **Tech Stack**: Python, Pandas, Matplotlib, Seaborn, Scikit-learn, NumPy

## 📁 Dataset

The dataset contains hourly data related to bike rental demand across a year, along with various weather and time features. Key variables include:

- `datetime`: Timestamp of record
- `season`: Categorical - Spring, Summer, Fall, Winter
- `holiday`: Whether the day is a holiday
- `workingday`: Whether the day is a working day
- `weather`: Weather situation (1-4)
- `temp`, `atemp`, `humidity`, `windspeed`: Weather indicators
- `casual`, `registered`, `count`: Rental counts by user type and total

## 🔍 Exploratory Data Analysis

Key insights from the EDA:

- **Seasonality**: Usage varies with months and seasons — highest in summer and fall.
- **Hourly Trends**: Registered users peak during commute hours (8 AM, 5-6 PM); casual users peak in afternoons and weekends.
- **User Behavior**: Registered users dominate usage, especially on working days.
- **Weather Influence**: Rainy and stormy conditions lead to significantly lower demand.
- **Correlations**: Temperature has a positive correlation with demand; humidity and windspeed have negative or weak influence.

## 🧠 Modeling Approach

- **Target Variable**: `count`
- **Model Type**: Supervised Regression
- **Steps**:
  - Feature Engineering: Hour, day of week, season, lag features
  - Data Transformation: Log-transform target if needed
  - Train/test split and cross-validation
  - Model training using algorithms like Linear Regression, Random Forest, and XGBoost
  - Evaluation using RMSE and R²

## 📈 Models Implemented

Multiple regression models were implemented and evaluated:

- **Linear Regression**: A baseline model for regression tasks.
- **Random Forest**: An ensemble method used for capturing non-linear patterns in data.
- **XGBoost**: A gradient boosting model for improved prediction performance.

The models were evaluated using:
- **RMSE (Root Mean Squared Error)**
- **R² (Coefficient of Determination)**
- **Adjusted R²**

## 📌 Next Steps

- Complete feature engineering and preprocessing
- Train and compare multiple regression models
- Optimize hyperparameters and evaluate on test data
- Visualize model performance and residuals
- Deploy the model to a real-time system for bike-sharing demand prediction

## 📷 Sample Visuals

![Hourly demand by user type](images/hourly_usage_user_type.png)
*Peak hours differ greatly between registered and casual users.*

![Correlation heatmap](images/correlation_heatmap.png)
*Key features like temperature and working day show correlation with demand.*

## 🧰 Tools & Libraries

- Python (Pandas, NumPy)
- Visualization: Matplotlib, Seaborn
- Modeling: Scikit-learn
- Jupyter Notebook

## 📚 Learnings

Through this project, I deepened my understanding of:
- Time series feature engineering
- User behavior segmentation
- Building interpretable regression models
- Evaluating and tuning predictive performance

## 📎 References

- Dataset Source: [UCI Machine Learning Repository – Bike Sharing Dataset](https://archive.ics.uci.edu/ml/datasets/bike+sharing+dataset)
- Inspired by real-world applications in urban planning and smart transportation systems

---

> 👤 Project by [Jatin Kanyan] 

