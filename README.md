# Projects
 
A series of independent projects in R, Python, and SQL: statistics and machine learning applied to various fields.
 
---
 
## Probability & Statistics (R)
 
[Convergence rate of the Poisson approximation to the Binomial](probability-statistics/poisson-binomial/poisson-binomial.md) Tests the accuracy of the Poisson approximation to the Binomial across a range of λ, using Total Variation Distance as the error metric. Finds the approximation holds within 3% error at λ = 12, and traces the residual error to the variance gap Var(X_Bin) = λ(1−p) < λ = Var(X_Pois). `R` `Total Variation Distance` `MGF`
 
[Empirical verification of the memoryless property of the Geometric distribution](probability-statistics/geometric-memoryless/geometric-memoryless.md) 50,000-trial Monte Carlo simulation confirming P(Y > a+b | Y > a) = P(Y > b) numerically, by conditioning on survival past a cutoff and comparing against a fresh baseline distribution. `R` `Monte Carlo Simulation`
 
---
 
## Regression & Machine Learning (Python, SQL)
 
[Forecasting inflation using macroeconomic indicators](Inflation_Forecasting/notebook/analysis.ipynb) Tests whether unemployment, the federal funds rate, and consumer sentiment predict US CPI inflation one month ahead (FRED, monthly, 1991–2026). Finds they do not: OLS and Ridge both return a negative R² against a persistence baseline, and adding the indicators to that baseline raises test RMSE by 13% while improving in-sample fit. `Python` `SQL` `Ridge Regression` `Time Series Cross-Validation`
 
[Predicting car prices from vehicle features](Machine_Learning/auto_price/auto_price.ipynb) Compares OLS, Ridge, Lasso, and ElasticNet on the UCI Automobile dataset (205 cars, 26 attributes) to predict price, with penalty strength chosen by cross validation. Ridge scores slightly worse than plain OLS on the 41 car test set, but repeated cross validation shows the gap is smaller than the fold to fold variance, so the difference is not reliable. Lasso's surviving coefficients, engine size, curb weight, and horsepower, match the strongest correlations with price found in the initial data exploration. `Python` `Ridge Regression` `Lasso` `Cross-Validation`
 
---
 
## Libraries and Tools
 
`R`, `Python` (NumPy, pandas, scikit-learn, matplotlib), `SQL` (SQLite), `R Markdown`, `Jupyter`

