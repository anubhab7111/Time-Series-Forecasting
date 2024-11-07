# American Electric Power (AEP) Energy Consumption Forecasting

This repository contains a time series forecasting model for estimating the energy consumption of the American Electric Power (AEP) company using historical data. The data is sourced from the Kaggle dataset **AEP - Estimated Energy Consumption**.

The model leverages the **XGBoost** algorithm to predict the energy consumption in **Megawatts (MW)**, based on historical time series data.

## Overview

Energy consumption forecasting is crucial for power grid management, energy trading, and efficient resource allocation. In this project, we aim to predict the energy consumption of AEP using machine learning techniques, particularly **XGBoost** (Extreme Gradient Boosting).

The dataset contains historical energy consumption data, with various features including date, day of the week, and time of day, which are used to build the predictive model.

## Dataset

The dataset used in this project is the **AEP - Estimated Energy Consumption** dataset from Kaggle. It includes historical data about energy consumption in MW for a period of time.

- **Source**: [AEP - Estimated Energy Consumption on Kaggle](https://www.kaggle.com/datasets/uciml/electric-power-consumption)
- **Features**:
  - `Date`: Date of the measurement
  - `Time`: Hour of the measurement
  - `Consumption`: Energy consumption in Megawatts (MW)
  - Other time-related features such as day of the week, month, and holidays.

## Model

The main approach used in this project for forecasting is **XGBoost**, a powerful machine learning algorithm known for its performance in regression and classification tasks. It is particularly suited for time series forecasting due to its ability to handle non-linear relationships and interactions between variables.

### Steps Taken:
1. **Data Preprocessing**:
   - Data cleaning (handling missing values, outliers)
   - Feature engineering (extracting date/time features)
   - Scaling and normalization of data
2. **Model Training**:
   - Split data into training and testing sets
   - Train XGBoost model using training data
3. **Model Evaluation**:
   - Evaluate the model using metrics like RMSE (Root Mean Squared Error)
   - Fine-tune model parameters using grid search or random search
