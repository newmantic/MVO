# MVO

Mean-Variance Optimization (MVO) is a foundational concept in portfolio management, introduced by Harry Markowitz. It aims to construct a portfolio that maximizes expected return for a given level of risk (variance), or equivalently, minimizes risk for a given level of return. In the context of a fixed income portfolio, MVO is used to allocate investments among different bonds or fixed income assets to achieve the best possible trade-off between expected return and risk.


Portfolio Return:
The expected return of a portfolio is the weighted sum of the expected returns of the individual assets (e.g., bonds) in the portfolio.
Portfolio Return (R_p) = sum(w_i * R_i)
Where:
R_p is the expected return of the portfolio.
w_i is the weight of asset i in the portfolio.
R_i is the expected return of asset i.

Portfolio Variance:
The variance of the portfolio is a measure of the portfolio's risk and is calculated using the covariance matrix of the asset returns and the portfolio weights.
Portfolio Variance (Var_p) = sum(sum(w_i * w_j * Cov(R_i, R_j)))

Alternatively, in matrix form:
Var_p = w.T * Cov * w
Where:
Var_p is the variance of the portfolio.
w is the vector of asset weights.
Cov is the covariance matrix of the asset returns.
w.T is the transpose of the weight vector.

Portfolio Standard Deviation (Volatility):
The standard deviation (or volatility) of the portfolio is the square root of the portfolio variance.
Portfolio Std Dev (σ_p) = sqrt(Var_p)

Sharpe Ratio:
The Sharpe Ratio measures the risk-adjusted return of the portfolio. It is calculated as the ratio of the portfolio's excess return over the risk-free rate to the portfolio's standard deviation.
Sharpe Ratio = (R_p - R_f) / σ_p
Where:
R_f is the risk-free rate.
R_p is the expected return of the portfolio.
σ_p is the portfolio's standard deviation.

Optimization Problem:
To maximize the Sharpe Ratio or minimize variance for a given target return, the optimization problem can be formulated as:
Minimize: w.T * Cov * w
Subject to: sum(w_i) = 1
and (optional): sum(w_i * R_i) = Target Return

Portfolio Return:
R_p = sum(w_i * R_i)

Portfolio Variance:
Var_p = sum(sum(w_i * w_j * Cov(R_i, R_j)))

Or in matrix form:
Var_p = w.T * Cov * w

Portfolio Standard Deviation:
σ_p = sqrt(Var_p)

Sharpe Ratio:
Sharpe Ratio = (R_p - R_f) / σ_p

Optimization Problem:
Minimize: w.T * Cov * w
Subject to: sum(w_i) = 1
Optional: sum(w_i * R_i) = Target Return

In MVO, the goal is to allocate portfolio weights (w_i) among different fixed income assets to achieve the desired balance between return and risk. The expected portfolio return is a linear combination of the expected returns of the assets, while the portfolio variance (and thus risk) depends on both the variance of individual assets and the covariances between them.

The Sharpe Ratio is used to assess the efficiency of the portfolio in terms of risk-adjusted return. The optimization process involves solving a quadratic programming problem to find the portfolio weights that either minimize the portfolio variance for a given return or maximize the Sharpe Ratio.

These concepts and equations are fundamental to constructing an optimized fixed income portfolio that meets specific investment objectives while managing risk.

