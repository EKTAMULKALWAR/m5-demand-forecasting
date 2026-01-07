# M5 Demand Forecasting (Walmart)

This project demonstrates an end-to-end retail demand forecasting pipeline using the M5 dataset.

## Problem
Forecast daily unit sales for the next 28 days for a Walmart item-store series.

## Approach
- Exploratory Data Analysis to understand intermittent demand
- Strong baseline forecasting (naive, 7-day mean, 28-day mean)
- Leakage-safe lag and rolling feature engineering
- LightGBM regression with time-based validation
- Hybrid approach blending ML predictions with rolling mean baselines
- Recursive 28-day demand forecasting

## Example Forecast
![Forecast](forecast_example.png)

## Key Insight
For intermittent retail demand, predicting expected demand levels is more reliable than chasing rare spikes. Blending statistical baselines with ML improves forecast stability and realism.

## Tools
Python, Pandas, NumPy, LightGBM, Matplotlib
