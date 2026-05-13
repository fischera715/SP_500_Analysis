# S&P 500 Time Series Analysis (2020–2025)

## Overview
This project analyzes the S&P 500 index using R to study return behavior, volatility, and statistical properties of financial time series data. The goal is to understand trends, distributional characteristics, and stationarity in equity market returns.


## Methods
- Collected historical S&P 500 data using the `quantmod` package from Yahoo Finance  
- Computed daily log returns to transform non-stationary price data into a stationary series  
- Applied the Augmented Dickey-Fuller (ADF) test to assess stationarity  
- Analyzed autocorrelation (ACF) and partial autocorrelation (PACF) to evaluate dependency structure  
- Examined return distribution and volatility patterns over time  
- Investigated volatility clustering during major market events  


## Key Findings
- The S&P 500 price series is non-stationary, while log returns are stationary (ADF test p < 0.05)  
- Daily returns exhibit very low autocorrelation, indicating limited short-term predictability  
- Volatility clusters during major economic events such as the COVID-19 crash and 2022 market downturn  
- Log returns provide a stable framework for modeling financial time series behavior  


## Tools Used
- R  
- quantmod  
- tseries  
- ggplot2  


## Summary
This project demonstrates foundational time series analysis techniques applied to financial data, including transformation, stationarity testing, and volatility analysis. It highlights key properties of equity returns that are important for financial modeling and quantitative analysis.
