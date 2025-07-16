# USD/CAD Exchange Rate Forecasting

Time Seires Course project. This project investigates macroeconomic drivers affecting the USD/CAD exchange rate and proposes a hybrid forecasting framework that combines traditional time series modeling (SARIMA) with machine learning (XGBoost and Random Forest).

## Project Overview
- Goal: Forecast the USD/CAD exchange rate one year ahead.
- Approach: Build and compare SARIMA, standalone ML models, and hybrid models.
- Data: Monthly data from 2005 to 2023 for key macroeconomic indicators.

## Key Features
- Exploratory data analysis of macroeconomic indicators
- Time series decomposition and seasonality checks
- SARIMA model selection via AIC and RMSE
- Feature importance analysis using XGBoost and Random Forest
- Hybrid model (SARIMA + ML residual correction)
- Robust comparison across modeling strategies

## Dataset
Dependent variable: USD/CAD exchange rate
Independent variables:
- Interest rate differential
- Inflation (CPI) differential
- GDP differential
- Oil price spread

Sources:
[Bank of Canada](https://www.bankofcanada.ca/)
[FRED Economic Data](https://fred.stlouisfed.org/)
[Statistics Canada](https://www.statcan.gc.ca/en/start)

## Modeling Framework
The hybrid modeling pipline includes:
1. SARIMA for capturing seasonality and linear trends.
2. Residual Modeling using:
   - Random Forest
   - XGBoost
3. Forecast Fusion: Combine SARIMA output with predicted residuals.
