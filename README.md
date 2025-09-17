## Time Series Analysis – Gold Prices

Overview: This project applies time series analysis to gold price data (2013–2023) to identify patterns and build a forecasting model.

ARIMA Model -
ARIMA stands for **AutoRegressive Integrated Moving Average**.  
- **AR (p):** Relationship between current value and its past values  
- **I (d):** Differencing to make the series stationary  
- **MA (q):** Relationship between current value and past forecast errors  

It is commonly used for forecasting time series data once stationarity is achieved.

Steps -
1. Loaded and cleaned daily average gold prices (removed 2010–2012)  
2. Plotted and decomposed the series into trend, seasonality, and residuals  
3. Checked for stationarity with the Augmented Dickey-Fuller (ADF) test  
4. Applied differencing to achieve stationarity  
5. Selected ARIMA parameters using auto_arima  
6. Built and fitted the ARIMA(1,0,2) model  
7. Validated with a train/test split (last 18 days)  
8. Evaluated results – RMSE ≈ 12.79, forecasts closely followed actual prices

