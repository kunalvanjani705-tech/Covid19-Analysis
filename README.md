🦠 COVID-19 Time Series Analysis & Forecasting
📌 Project Overview

This project performs an end-to-end time series analysis of global COVID-19 data. The goal is to analyze trends, test for stationarity, transform the data appropriately, and build forecasting models to predict future case counts.

The analysis follows a structured data science pipeline — from data preprocessing to forecasting and visualization.

📊 Dataset
The dataset contains daily global COVID-19 statistics including:
Confirmed cases
Deaths
Recovered cases
Active cases
Date (time index)
Data was aggregated at the global level for time series modeling.

🔎 Exploratory Data Analysis (EDA)
Converted Date column to DatetimeIndex
Aggregated data by Date
Checked for duplicates and missing values
Converted cumulative cases to daily cases

Visualized:
Trend
Seasonality
Rolling mean & rolling standard deviation

📈 Stationarity Analysis
To prepare the data for modeling:
Log Transformation
Differencing
Rolling statistics visualization
Augmented Dickey-Fuller (ADF) Test
KPSS Test
Objective: Ensure the time series satisfies stationarity assumptions.

🛠 Modeling Techniques
The following models were applied:

SARIMAX (with seasonal component)

Model parameters were selected based on:
ACF & PACF plots
AIC values
Diagnostic plots

📊 Forecasting
Generated 30-day forecasts
Applied inverse log transformation 

Visualized predictions using
Matplotlib
Plotly (interactive)

📌 Key Insights

COVID cumulative data is non-stationary
Daily cases provide better modeling structure
Seasonality (weekly patterns) exists in reported data
Differencing removes trend component effectively
SARIMAX performs better when seasonality is present

📦 Technologies Used
Python
Pandas
NumPy
Matplotlib
Plotly
Statsmodels

