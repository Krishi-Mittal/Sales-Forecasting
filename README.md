The following Anlaysis is on "Sales Forecasting".

OBJECTVE: This project aims to analyze and forecast monthly sales of the comanpany using the SARIMA MODEL, with objective to capture seasonality and trend efficiently. The Analysis involved:

(1) Data Processing & Transformation
- Check the dimesnions of the dataset
- Check missing/null values
- Drop the null values
- Check the dimensions of the dataset
- Convert the Order Date into Date Time
- Aggregates raw sales data first on daily basis and then on a monthly basis
- Applies log transformation to stabilize variance
- Splits data into train (80%) and test (20%) sets

(2) Model Selection & Forecasting
- Use seasonal decompose to check trend, seasonality and distribution of residuals
- Check stationarity using Augmented Dickey Fuller (ADF) Test
- Plot ACF and PACF to find the order of p and q
- Uses auto_arima to find the best SARIMA order
- Implements a rolling forecast approach
- Forecasts 12 months into the future

(3) Model Evaluation & Diagnostics
- Computes MAE (Mean Absolute Error) & RMSE (Root Mean Squared Error)
- Performs residual diagnostics using plot_diagnostics()
- Plots actual vs. predicted sales trends

(4) Conclusion
The SARIMA MODEL successfully forecasted for sales for next 12 months. By applying log transformation, the model stability improved and reduced forecasting errors. The rolling forecast approach provided more accurate and adaptive predictions over time. The model can be improved further by incorporating other factors like - Holidays, Inflation, Shipping Cost, Competition from Competitors, Advertisement, etc. Since, these variables were not available in the given dataset, ceteris paribus, the model performed well achieving it's objective of capturing seasonality and trend while forecasting the sales.
