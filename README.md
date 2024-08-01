# Stock_Market_Portfolio_Optimization
Financial Analysis Project: Stock_Market_Portfolio_Optimization_using_Python

## Problem Statement
The goal is to develop a portfolio optimization strategy using the given stock market data. This involves analyzing historical price trends, calculating key financial metrics, and applying Modern Portfolio Theory (MPT) to construct an efficient portfolio. The primary objectives are:
- Identify trends in stock prices using moving averages and other technical indicators.
- Calculate the volatility and risk associated with each stock.
- Determine the correlation between different stocks to understand their relationships and potential diversification benefits.
- Generate and evaluate a series of random portfolios to identify the optimal portfolio that maximizes the Sharpe ratio, balancing risk and return effectively.
  
Expected results include:
- Identification of the portfolio with the maximum Sharpe ratio, including the weights of each stock and the associated risk-return profile.
- Recommendations for constructing a diversified investment portfolio that maximizes returns while minimizing risk, based on the historical performance and statistical analysis of the provided stock data.

## Stock market portfolio optimization using Python
- Stock market portfolio optimization is the process of selecting the best combination of stocks to maximize returns while minimizing the risk, based on historical performance data and financial metrics. We will go through the task of stock market portfolio optimization with Python.
- Stock market portfolio optimization involves analyzing price trends, calculating expected returns and volatilities, and determining the correlations between different stocks to achieve diversification. Using techniques such as Modern Portfolio Theory (MPT), we can construct an efficient portfolio that relies on the efficient frontier to represent the optimal trade-off between risk and return.
- The expected results from stock market portfolio optimization include identifying the portfolio with the highest Sharpe ratio, which indicates the best risk-adjusted return and provides a clear allocation strategy for the selected stocks to achieve long-term investment goals.
- To get started with stock market portfolio optimization, we need to collect data about the stock market performance over time. I will collect real-time stock market data using the yfinance API.
Importing the necessary Python libraries and collecting the stock market data using the yfinance API. We can install it on your Python environment by executing the command below on your terminal or command prompt:
- pip install yfinance

we will collect the stock market data of some popular Indian companies

### Stock market performance of these companies in the stock market over time

- We can see that:
TCS has the highest adjusted close prices, followed by RELIANCE, INFY (Infosys), and HDFCBANK. The prices for RELIANCE and TCS show noticeable upward trends, which indicates strong performance, while HDFCBANK and INFY exhibit more stability with relatively lower price fluctuations.


### we compute the 50-day and 200-day moving averages and plot these along with the Adjusted Close price for each stock

- For HDFCBANK and INFY, the prices initially decline but later show signs of recovery, as indicated by the moving averages. RELIANCE and TCS display a more consistent upward trend in their adjusted close prices.
- The volume traded graphs highlight significant trading activity at various points, with spikes indicating high trading volumes, particularly noticeable in HDFCBANK and RELIANCE around early 2024.
These insights are crucial for understanding price movements and trading behaviours, which assist in making informed investment decisions.


### We have a look at the distribution of daily returns of these stocks

- The distributions we see are approximately normal, centred around zero, which indicates that most daily returns are close to the average return. However, there are tails on both sides, which reflect occasional significant gains or losses.
- INFY and RELIANCE appear to have slightly wider distributions, which suggests higher volatility compared to HDFCBANK and TCS.


### We see if there’s any correlation between all the stocks

- INFY and TCS have a high positive correlation (0.71), which indicates that they tend to move in the same direction. HDFCBANK has a moderate positive correlation with RELIANCE (0.37) and a low correlation with INFY (0.17) and TCS (0.10).
- RELIANCE shows a low correlation with INFY (0.19) and TCS (0.13).
These varying correlations suggest potential diversification benefits; combining stocks with lower correlations can reduce overall portfolio risk.

### Portfolio Optimization
Now, using Modern Portfolio Theory, we can construct an efficient portfolio by balancing risk and return. We will:
- Calculate the expected returns and volatility for each stock.
- Generate a series of random portfolios to identify the efficient frontier.
- Optimize the portfolio to maximize the Sharpe ratio, which is a measure of risk-adjusted return.


### We calculate the expected returns and volatility for each stock

- We see that RELIANCE has the highest expected return (29.73%) and moderate volatility (21.47%), which indicates a potentially high-reward investment with relatively higher risk.
- INFY and TCS also have high expected returns (21.38% and 22.09% respectively) with moderate volatility (23.23% and 19.69%).
- HDFCBANK has the lowest expected return (1.37%) and moderate volatility (20.69%), which makes it the least attractive in terms of risk-adjusted returns.

### Next, we will:
- Generate a large number of random portfolio weights.
- Calculate the expected return and volatility for each portfolio.
- Plot these portfolios to visualize the efficient frontier.


### We will generate the random portfolios and plot the efficient frontier:

- Each dot represents a portfolio, with the colour indicating the Sharpe ratio, a measure of risk-adjusted return.
- Portfolios on the leftmost edge of the frontier (closer to the y-axis) offer the highest expected returns for a given level of volatility, which represent optimal portfolios.
- The gradient shows that portfolios with higher Sharpe ratios (darker blue) provide better risk-adjusted returns.

### Here’s how to identify the portfolio with the maximum Sharpe ratio:

The portfolio with the maximum Sharpe ratio has the following characteristics:
- Expected Return: ~31.34%
- Volatility: ~16.13%
- Sharpe Ratio: ~1.94

### Next, we identify the weights of the stocks in the portfolio that yield the maximum Sharpe ratio:

The output shows a diversified portfolio with the following allocations:
- HDFCBANK (30.85%)
- INFY (10.59%)
- RELIANCE (18.02%)
- TCS (40.53%)

TCS has the highest allocation, which indicates its significant contribution to the portfolio’s performance, while INFY has the smallest allocation. This balanced allocation aims to maximize returns while minimizing risk by leveraging individual stock performances and their correlations.

## Summary
So, this is how stock market portfolio optimization works. Stock market portfolio optimization involves analyzing price trends, calculating expected returns and volatilities, and determining the correlations between different stocks to achieve diversification.

