# ADF-Test

ADF Test in Python

The statsmodel package provides a reliable implementation of the ADF test via the adfuller() function in statsmodels.tsa.stattools. It returns the following outputs:

* The p-value
* The value of the test statistic
* Number of lags considered for the test
* The critical value cutoffs.
* When the test statistic is lower than the critical value shown, you reject the null hypothesis and infer that the time series is stationary.

An optional argument the adfuller() accepts is the number of lags you want to consider while performing the OLS regression.

By default, this value is 12*(nobs/100)^{1/4}, where nobs is the number of observations in the series. But, optionally you can specify either the maximum number of lags with maxlags parameter or let the algorithm compute the optimal number iteratively.
