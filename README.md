Portfolio Optimization Capstone Project

🎯 Project Goal: The Optimal Risk-Adjusted Allocation

This project implements Modern Portfolio Theory (MPT), pioneered by Harry Markowitz, to determine the optimal asset allocation for a diversified portfolio of major technology stocks. The primary objective was to find the Maximum Sharpe Ratio Portfolio, which represents the highest expected return for a given level of risk.

📈 Methodology

1. Data Acquisition & Preparation (10 Years History)

Assets: Apple (AAPL), Microsoft (MSFT), Alphabet (GOOGL), and Amazon (AMZN).

Time Horizon: 10 years of historical Adjusted Closing Price data, spanning from January 1, 2016, to the present.

Preprocessing: Daily returns were calculated and annualized (multiplied by 252 trading days) to determine the annualized average returns and the annualized covariance matrix.

2. Monte Carlo Simulation

A Monte Carlo simulation was executed to explore the entire universe of possible portfolio combinations:

Iterations: 50,000 random asset allocations were generated.

Metrics Calculated for Each Portfolio:

Annual Return: The expected yearly gain.

Annual Volatility (Risk): The standard deviation of returns.

Sharpe Ratio: (Portfolio Return - Risk-Free Rate) / Volatility. This is the measure of risk-adjusted performance used for optimization.

3. Visualization: The Efficient Frontier

The results of the 50,000 simulations were plotted on a scatter graph where the X-axis is Volatility (Risk) and the Y-axis is Return. The upper boundary of this data cloud forms the Efficient Frontier .

✅ Key Results (The Optimal Portfolio)

The analysis identified the single best asset allocation that maximizes the Sharpe Ratio based on the 10-year lookback period.

Metric

Value

Maximum Sharpe Ratio

1.109160

Annual Expected Return

27.57%

Annual Volatility (Risk)

24.85%

Optimal Asset Weights

To achieve the maximum risk-adjusted return, the assets should be weighted as follows:

AAPL: 25.53%

MSFT: 21.06%

GOOGL: 23.08%

AMZN: 30.33%

💻 Technologies Used

Language: Python

Libraries: pandas, numpy, yfinance, matplotlib, plotly
