Risk-Aware Portfolio Optimization and Value at Risk Modeling
============================================================

This project implements a portfolio optimization framework in Python, combining financial theory with risk analytics. It uses mean-variance optimization, Sharpe ratio maximization, Value at Risk (VaR), and basic stress testing to evaluate portfolio performance under uncertainty.

Objective
---------
To build a tool that constructs an optimal asset allocation based on historical return data, while providing quantitative risk metrics such as Value at Risk and stress-tested scenarios.

Key Features
------------
- Mean-variance optimization (Sharpe ratio maximization)
- Historical and parametric (Gaussian) Value at Risk (VaR) estimation
- Simulated stress testing to evaluate downside exposure
- Efficient frontier visualization using Monte Carlo simulation
- Configurable asset list and time period

Methodology
-----------
1. Data Collection: Historical daily prices are fetched using the yfinance API.
2. Returns Calculation: Daily returns computed using adjusted close prices.
3. Portfolio Optimization:
   - Objective: Maximize Sharpe ratio
   - Constraints: Full investment (sum of weights = 1), no short selling
4. Risk Metrics:
   - Historical VaR (5% quantile)
   - Parametric VaR using standard deviation and mean
5. Stress Testing: Simulates a market shock (e.g., 2% daily drop) to assess cumulative portfolio impact.
6. Efficient Frontier: Simulated portfolios to compare expected returns vs. risk.

Technologies Used
-----------------
- Python 3.8+
- NumPy, Pandas
- yfinance
- SciPy (for constrained optimization)
- Matplotlib, Seaborn

Use Cases
---------
- Risk-aware asset allocation for individual portfolios
- Exploratory tool for finance students and analysts
- Interview project for roles in risk, portfolio management, or quantitative finance
- Simulation and benchmarking of market stress scenarios

Author
------
Pratyush Raman
National Institute of Technology Rourkela
August 2025
