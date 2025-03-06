# Superstore Sales Forecasting using Time Series Analysis

## 1. Introduction

Sales forecasting is crucial for inventory management, budgeting, and strategic planning. This project applies time series forecasting techniques to predict future sales for a superstore based on historical sales data.

## 2. Data Description and Preprocessing

The dataset consists of transaction records, including order date and sales amount. The steps involved in preprocessing were:

Converting "Order Date" to a DateTime format.

Aggregating sales data on a monthly basis.

Handling missing values and outliers if necessary.

## 3. Exploratory Data Analysis (EDA)

A line plot of monthly sales trends revealed a seasonal pattern.

A seasonal decomposition of time series confirmed seasonality.

ADF test was applied to check stationarity:

If non-stationary, differencing was applied to stabilize the mean.

## 4. Forecasting Models

### 4.1 ARIMA Model

Auto ARIMA was used to select the best parameters (p, d, q) automatically.

The model was trained and used for forecasting.

### 4.2 Holt-Winters Exponential Smoothing

Three variations were tested: Additive, Multiplicative, and Fixed.

The best variation was selected based on performance metrics.

## 5. Model Evaluation

Models were compared using:

Mean Squared Error (MSE)

Root Mean Squared Error (RMSE)

Mean Absolute Error (MAE)

## 6. Results and Conclusion

The Holt-Winters Multiplicative Model performed best with the lowest error metrics.

Forecasts were generated with 70%, 80%, and 95% confidence intervals.

The final model can be used for inventory planning and decision-making.
