The following Anlaysis is on "Sales Forecasting".

This project aims to analyze and forecast sales of the comanpany using the SARIMA MODEL. The primary objective of the analysis is to:

Model the volatility of financial returns.
Evaluate residuals to ensure the model captures volatility clustering effectively.
Perform a multi-step volatility forecast to estimate future volatility.
Implement a rolling forecast approach to capture dynamic volatility patterns over time.
The analysis begins with importing relevant such as Pandas, Matplot, Seaborn, Statsmodel, arch, numpy followed by impoting the data.

Model Selection: GARCH The analysis begain with ARIMA medl but due to the presence of hetroscedasticity, moved to GARCH Model. Chose the GARCH(1,1) model for its efficiency in capturing volatility clustering. GARCH models the conditional variance as a function of past squared observations and past variances, making it ideal for financial data. The model was fitted using the arch library in Python.

The Anlysis:

Conducted Residual Analysis
Performed the Ljung-Box test to ensure there’s no remaining autocorrelation, validating the model’s robustness.
Variance Forecasting
Forecasted volatility for 30 days ahead using the fitted GARCH model.
Plotted the variance forecast to visualize expected volatility trends.
Rolling Forecast
Implemented a rolling forecast approach to enhance prediction accuracy. This method effectively adapts to changing market conditions.

Conclusion:
The model predicted decreasing volaility over the next 30 days, which means the market is gaining confidence and becoming more stable over time. This would attract investors, thereby leading to a rise in price, thus it is advisable to invest currently.
