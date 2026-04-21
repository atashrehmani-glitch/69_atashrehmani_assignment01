# 69_atashrehmani_assignment01
Project Overview

This project focuses on analyzing and forecasting stock prices using the ARIMA (AutoRegressive Integrated Moving Average) model. Daily closing prices of a selected NSE-listed stock were collected for the past one year and used for time series analysis and prediction.

Objective
Analyze historical stock price data
Check stationarity of the time series
Build an ARIMA model
Forecast future stock prices for the next 30 days
 Dataset
Source: NSE Historical Data
Data: Daily closing prices for the past 1 year
File: stock_data.csv
Data Preprocessing
(i) Data Cleaning
Converted Date column to datetime format
Sorted data by date
Handled missing values using forward fill / removal
(ii) Visualization
Plotted closing price vs date to observe trends

 Graph: Closing Price Trend
(Insert screenshot here)
 ARIMA Model Implementation
(i) Stationarity Check
Performed ADF (Augmented Dickey-Fuller) Test
Result:
p-value > 0.05 → Data is non-stationary
Applied differencing to make it stationary
(ii) Parameter Selection (p, d, q)
Used:
ACF plot → to determine q
PACF plot → to determine p
Selected ARIMA parameters:
p = 1, d = 1, q = 1 (example values)

Graphs: ACF & PACF Plots
(Insert screenshots here)

(iii) Model Training
Fitted ARIMA model on training data
Evaluated model using error metrics (e.g., RMSE)
Future Price Prediction
(i) Forecasting
Predicted stock prices for the next 30 days
(ii) Visualization
Plotted:
Historical data
Forecasted values

Graph: Forecast vs Actual
(Insert screenshot here)

Results & Observations
The stock shows (increasing/decreasing/volatile) trend over time
ARIMA model captured the trend reasonably well
Forecasted values follow the historical pattern with slight variations
Model performance depends on proper parameter tuning
Technologies Used
Python
Pandas
NumPy
Matplotlib
Statsmodels
