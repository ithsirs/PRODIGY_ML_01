# PRODIGY_ML_01
This repository contains the source code of the task-01 (Implement a linear regression model to predict the prices of houses based on their square footage and the number of bedrooms and bathrooms.)
Dataset:https://www.google.com/url?q=https%3A%2F%2Fwww.kaggle.com%2Fdatasets%2Fcamnugent%2Fcalifornia-housing-prices

# 🏡 California Housing Price Prediction

This project implements regression models to predict housing prices in California using the **California Housing Prices** dataset from Kaggle. The models are trained on numerical and categorical features derived from the dataset.

## 📁 Dataset

- **Source**: [California Housing Prices (Kaggle)](https://www.kaggle.com/datasets/camnugent/california-housing-prices)
- Features include:
  - Median income
  - House age
  - Average rooms and bedrooms
  - Population
  - Latitude & longitude
  - Ocean proximity (categorical)

## 🧹 Data Preprocessing

- Null values are dropped.
- The categorical column `ocean_proximity` is converted to binary/numerical encoding:
  - "NEAR OCEAN" or "NEAR BAY" → 1
  - Others → 2
- Features are selected and transformed for training.

## 🔍 Exploratory Data Analysis

- Correlation matrix is generated using Seaborn heatmap to identify influential features.
- Visualization helps guide feature selection and engineering.

## 🛠️ Feature Engineering

- Created new binary features from categorical values.
- Selected important predictors for model training.

## 🤖 Models Used

Two models are implemented and compared:

### 1. **Linear Regression**
- Simple baseline model to capture linear relationships between features and house prices.

### 2. **Random Forest Regressor**
- An ensemble model that builds multiple decision trees and averages their predictions.
- Better captures non-linear patterns and interactions between features.

## 🧪 Evaluation

- The dataset is split into training and testing sets using `train_test_split`.
- Evaluation metrics:
  - **R² Score**
  - **Mean Absolute Error (MAE)**
  - **Mean Squared Error (MSE)**

## 🛠️ Libraries Used

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- kagglehub (for dataset retrieval)


This project is open-sourced under the [MIT License](LICENSE).

