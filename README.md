## From-Rejection-to-Prediction##
A three-part applied statistics project using R: rejection sampling, time series modeling (ARIMA &amp; VAR), and volatility forecasting with GARCH.

# 📁 Sample Data#

This repository includes sample datasets (`usd_gbp_sample.csv` and `indices_sample.xlsx`)  
to allow others to run and explore the code without access to the original coursework files.

These files contain simulated values and do not represent real market data.

# 🧩 Task 1 – Rejection Sampling & Distribution Fitting#

Goal:
To implement rejection sampling for generating random variables from a specified target distribution, evaluate the sampling efficiency, and test the goodness-of-fit of the simulated data.

What’s done:
	•	Simulated values from a custom distribution using rejection sampling
	•	Compared empirical distribution with theoretical one
	•	Applied Kolmogorov–Smirnov (KS) test for goodness-of-fit evaluation
	•	Visualized histograms and overlayed theoretical density

Skills & Tools:
R, simulation, distribution theory, ks.test, plotting

Takeaway:
This section demonstrates simulation-based data generation and evaluation — a foundational method for probabilistic modeling, Monte Carlo methods, and statistical computing.

# ⏳ Task 2 – Time Series Modeling with ARIMA and VAR#

Goal:
To model and forecast time series data using both univariate (ARIMA) and multivariate (VAR) approaches. The analysis is based on financial index returns.

What’s done:
	•	Processed stock index data and converted it to log-returns
	•	Conducted ARIMA modeling (with ACF/PACF diagnostics and forecasting)
	•	Built a Vector Autoregression (VAR) model to capture relationships between multiple indices
	•	Performed Granger causality testing and impulse response analysis

Skills & Tools:
R, forecast, vars, tseries, time series diagnostics, multivariate modeling

Takeaway:
This task showcases time series forecasting techniques used in economics and finance, demonstrating how asset relationships can be captured through VAR models.

# 📉 Task 3 – Exchange Rate Volatility Modeling with GARCH#

Goal:
To model the volatility of USD/GBP exchange rate returns using ARCH and GARCH models, identifying patterns in conditional variance over time.

What’s done:
	•	Preprocessed daily exchange rate data and computed log returns
	•	Diagnosed volatility clustering with ACF of squared returns
	•	Fitted and evaluated ARCH(1) and GARCH(1,1) models
	•	Forecasted future volatility and visualized conditional variances

Skills & Tools:
R, rugarch, tseries, volatility modeling, financial time series analysis

Takeaway:
Volatility modeling is essential for risk management and derivative pricing. This section demonstrates how GARCH captures the non-constant variance structure in financial returns.
