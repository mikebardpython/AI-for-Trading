Implement a trading strategy on your own, and test to see if it has the potential to be profitable. You will be supplied with a universe of stocks and time range. You will also be provided with a textual description of how to generate a trading signal based on a momentum indicator. You will then compute the signal for the time range given and apply it to the dataset to produce projected returns. Finally, you will perform a statistical test on the mean of the returns to conclude if there is alpha in the signal. For the dataset, we'll be using the end of day from Quotemedia.
*	def resample_prices -  implement the `resample_prices` to resample `close_prices` at the sampling frequency of `freq`.
*	def compute_log_returns – accepts dataframe and produces a dataframe of log returns using Numpy’s log function
*	def shift_returns – shift_returns to calcualte returns over time period chosen by the shift parameter
*	def get_top_n – based previous returnsdetern which ones were the top performers
*	def portfolio_returns – eme Implement the portfolio returns function to compuyte the expected portfolio returns within a look ahead window
*	def analyze_alpha – perform a t-test with the null hypothesis being that the mean return is zero
