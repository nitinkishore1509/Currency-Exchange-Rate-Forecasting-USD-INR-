
# 📈 INR–USD Exchange Rate Forecasting using SARIMAX

This project forecasts the Indian Rupee (INR) to US Dollar (USD) exchange rate using the **SARIMAX** (Seasonal AutoRegressive Integrated Moving Average with eXogenous regressors) model.  
It uses historical daily closing prices to build a seasonal time series forecasting model and visualize trends.

---

## 📌 Project Overview

- **Objective**: Predict future INR–USD exchange rates based on historical data.
- **Model**: SARIMAX — ideal for time series with both trend and seasonality.
- **Dataset**: Historical INR–USD rates from `INR-USD.csv` (daily closing prices).
- **Visualization**: All plots are generated using **Matplotlib** for clarity.

---

## 🛠 Steps in the Project

1. **Data Loading**
   - Reads INR–USD historical data from CSV.
   - Parses the `Date` column into datetime format and sets it as the index.

2. **Exploratory Data Analysis (EDA)**
   - Line plot of historical closing prices.
   - Seasonal patterns and trends are visually inspected.

3. **Stationarity Check**
   - Augmented Dickey-Fuller (ADF) test to check if differencing is required.

4. **Model Building**
   - SARIMAX model with parameters `(p, d, q)` for ARIMA and seasonal `(P, D, Q, s)` for seasonality.
   - Seasonal period set to 52 weeks to capture yearly seasonality.

5. **Model Training & Forecasting**
   - Fits the SARIMAX model to the training data.
   - Generates in-sample predictions and out-of-sample forecasts.

6. **Visualization**
   - Actual vs Predicted values (Matplotlib).
   - Forecast plot showing predicted future exchange rates.

---



