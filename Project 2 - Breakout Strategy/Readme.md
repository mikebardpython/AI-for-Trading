## Project #2 – Breakout Strategy
Implement the breakout strategy, find and remove outliers, and test to see if it can be profitable.
* def get_high_lows_lookback – get the maximum high price and minimum low price over a window of days not including the current day
* def get_long_short – compute long/short/flat signals: SHORT if low > close, LONG if high < close, otherwise flat
* def clear_signals – filter signals as you do not want to go long if you capital is already committed long or short if capital is already commited to the downside
* def get_lookahead_prices – evaluating how many days to short or long stocks
* def get_return_lookahead – generate the log price return between the closing price and the lookahead price
* def get_signal_return – determine the returns generated by the signal using the long/short/flat signal and the returns determined from lookahead returns
* def calculate_kstest – use the scripy.stats.kstest to see if your population is normally distributed
* def find_outliers – outliers are determined by: symbols that passthe null hypothesis with a  p-value less than the threshold (5%) and symbols that have a KS value above the KS threshold
