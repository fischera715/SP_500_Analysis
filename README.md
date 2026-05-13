# S&P 500 Time Series Analysis (2020–2025)

## Overview
This project performs an exploratory time series analysis of the S&P 500 index using R. The goal is to understand price behavior, return dynamics, volatility patterns, and stationarity in financial time series data.

The S&P 500 represents 500 large-cap U.S. companies and is widely used as a benchmark for overall market performance.

Data was obtained from Yahoo Finance using the `quantmod` package in R.


## Methods
- Collected historical S&P 500 adjusted closing prices using `quantmod`
- Analyzed price trends and structural market changes
- Transformed price series into daily log returns:
  
  \[
  r_t = \log(P_t) - \log(P_{t-1})
  \]

- Computed descriptive statistics of returns (mean, variance, standard deviation)
- Applied Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF)
- Conducted Augmented Dickey-Fuller (ADF) test for stationarity
- Analyzed return distribution and rolling volatility (20-day window)


## Key Findings
- The S&P 500 price series is non-stationary and exhibits a strong upward trend with structural shocks (e.g., COVID-19 crash in 2020 and volatility in 2022)
- Daily log returns are stationary with a mean close to zero (≈ 0.0005)
- The ADF test confirms stationarity (p-value < 0.05)
- Returns show very low autocorrelation, indicating weak short-term predictability
- Volatility clustering is observed during major market events, with elevated uncertainty in 2020, 2022, and 2025
- The distribution of returns is centered around zero with occasional extreme values


## Descriptive Statistics (Log Returns)
- Mean: 0.0004979  
- Variance: 0.0001749  
- Standard Deviation: 0.0132 (~1.3% daily volatility)


## Key Visuals
- S&P 500 price trend (2020–2025)
- Daily log returns time series
- Histogram of returns
- ACF and PACF plots
- 20-day rolling volatility


## Conclusion
This analysis demonstrates that while S&P 500 prices are non-stationary, transforming them into log returns produces a stationary series suitable for time series analysis.

The results highlight key properties of financial data, including low autocorrelation, volatility clustering, and return distributions centered around zero. These characteristics are foundational for financial modeling and quantitative analysis.


## Tools Used
- R
- quantmod
- tseries
- ggplot2
