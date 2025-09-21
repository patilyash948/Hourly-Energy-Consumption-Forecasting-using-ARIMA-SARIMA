Description

This repository contains a Python project for forecasting hourly energy consumption using time series models. It demonstrates the difference between ARIMA and SARIMA models, showing how seasonality affects predictions.

The project is designed to:

Load and preprocess hourly energy consumption data.

Visualize historical consumption trends.

Fit ARIMA and SARIMA models for forecasting.

Generate hourly and daily forecasts.

Compare ARIMA vs SARIMA forecasts to highlight seasonality impact.

Allow users to query forecasted energy consumption for a specific datetime.

Key Features

Automatic handling of missing data with forward filling.

Uses statsmodels and pmdarima for time series modeling.

Supports hourly, daily, and multi-day forecasts.

Visual plots for easy comparison between models.

Demonstrates why ARIMA alone fails on seasonal data.

Technologies

Python 3.x

Pandas, Numpy

Matplotlib & Seaborn

Statsmodels (ARIMA & SARIMA)

Pmdarima (Auto ARIMA)

Usage

Clone the repository:

git clone https://github.com/your-username/energy-forecasting.git
cd energy-forecasting


Install dependencies:

pip install -r requirements.txt


Run the notebook or script:

jupyter notebook Energy_Forecasting.ipynb


Enter your future datetime to get forecasted energy consumption.

Dataset

The dataset should contain hourly timestamps and energy consumption values.

Example CSV format:

Timestamp,EnergyConsumption
01-01-2022 00:00,75.36
01-01-2022 01:00,83.40
01-01-2022 02:00,78.27

Why ARIMA vs SARIMA

ARIMA: Works for trend and short-term correlations, but fails for seasonal patterns → flat forecasts.

SARIMA: Captures trend + seasonality, giving realistic hourly forecasts.

