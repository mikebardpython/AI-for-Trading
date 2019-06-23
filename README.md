# AI-for-Trading
## Udacity Nanodegree - AI for Trading

### Project 3 - Smart Beta and Portfolio Optimization

*Part1 – Smart Beta Portfolio*
* Build portfolio using dividend yield to show portfolio weights
* Compare the portfolio to a market cap weighted index to see how well it performed
* For this exercise we will simulate a market cap weighted index
* Index weights – generate the weights based on dollar volume traded for that date
* def generate_dollar_volume_weights(close, volume)
* def calculate_dividend_weights returns the weights for each stock based on its total dividend yield over time. This is similar to generating the weight for the index, but its using dividend data instead. 
* def generate returns  to generate returns data for all the stocks and dates from priced data. You might notice we’re implementing returns and not log returns. Since we’re not dealing with volatility, we don’t have to generate log returns.
* def generate_weighted_returns with the returns computed for each stock, we can use it to comute the returns for an index or etf. Implement generate_weighted_returns to create weighted returns using the returns and weights.
* def calculate_cumulative_returns – to compre the performs between the etf and index, we’re going to calculate the tracking error. Before we do that, we first need to calcuate the index and etf comulative returns. Implement calcualte_cumulative_returns to calcualte the cumulative retuns over tiem given the returns
* def tracking_error – in order to check the performance of the smart beta portfolio, we can calculate the annualized tracking error against the index. Implement tracking error to return the tracking error between the etf vs the benchmark

Part 2 – Optimization 
•	Create 2nd portfolio independent from dividend-weighted portfolio created in part 1
•	We want to BOTH minimize the portfolio variance and also want to clsoly track a market cap weighted index, i.e. we are trying to minimize the distance between the weightes of our portfolio and the weights of the index
•	def get_covariance_returns – calculates the covariance of returns 
•	def get_optimal_weights – minimize portfolio variance and closely track benchmark index (aka – minimize the distance between the weights of our portfolio and the weights of the index.
•	def rebalance_portfolio – rebalance portfolio every n number of days and compute the optimal weights using above functions get_optimal_weights & get_covariance_returns
•	def get_portfolio_turnover  - porfolios with higher turnover have higher costs.Wwith the portfolio rebalanced, we need to use a metric to measure the cost of rebalancing the portfolio.

