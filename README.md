# Forecasting Divorce Rates in the UK: A Time Series Analysis

## Project Overview
This project focuses on forecasting divorce rates in the United Kingdom using historical data and time series models. By analyzing trends from the past decades, the goal is to project future divorce rates and evaluate the performance of different forecasting methods, including Holt-Winters exponential smoothing and ARIMA models. Accurate forecasting of divorce rates is critical for policymakers, allowing them to anticipate societal trends and make informed decisions about family support services and resource allocation.

## Technologies Used
R Programming Language: Primary language for data analysis and visualization.
R Libraries:
- forecast: For building and evaluating time series models (ARIMA, Holt-Winters).
- tidyverse: For data import, tidying, manipulation, and data visualization.
- tseries: For statistical tests (ADF).
- TTR.

## How to Run
1. Clone the Repository:
```bash
git clone https://github.com/B-Taiwo/timeseries-uk-divorces.git
```
2. Install the Required R Libraries: Open your R console or RStudio and install the necessary libraries by running:
```R
install.packages(c("forecast", "tidyverse", "tseries", "TTR"))
```
3. Run the Analysis: Open the provided R notebook (divorces timeseries.Rmd) and run it in your R environment. The script includes:
- Data loading and preprocessing
- Time series decomposition
- Model fitting for Holt-Winters and ARIMA
- Model evaluation and comparison

## Project Results
- Forecasting Models: Among the tested models, ARIMA (1,2,1) was the best. It captured the structure of the time series 
most effectively by accounting for correlations in the irregular components, as it had lower error 
metrics such as AIC, MAPE, and RMSE. While Holt-Winters is suitable for data with clear trends, its 
inability to handle autocorrelations limited its forecasting precision.
- Model Comparison: The ARIMA model showed a better fit compared to Holt-Winters based on AIC, residual diagnostics, and RMSE values.
- Key Insights: The forecast suggests that divorce rates in the UK followed a steady upward trend from the 1970s 
until the mid-1990s, after which they began to decline. These trends likely follow societal changes 
influencing marriage stability This information can be valuable for long-term planning and policy formulation related to family and societal well-being.
