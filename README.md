## BIST Banking Stocks - Data Science & Quantitative Analysis
This project performs a complete data science, quantitative finance, and portfolio analytics study on major Turkish banking stocks listed on Borsa İstanbul (BIST).

The goal is to understand price behavior, risk characteristics, correlations, and portfolio performance using real-world financial data.

### Project Overview:
This project analyzes daily price movements, returns, volatility, correlations, portfolio behavior, factor exposure, and strategy performance of BIST banking stocks.

It also compares a bank portfolio against the BIST 100 index and evaluates whether trading strategies outperform buy-and-hold.

The project covers:
- Exploratory Data Analysis (EDA)
- Return calculations and volatility measurement
- Correlation analysis between banks
- Outlier detection (price/volume shocks)
- Lead–lag (leader–follower) behavior
- Portfolio construction (equal-weighted)
- Comparison with BIST 100 index
- Moving Average strategy backtest
- Regression & factor analysis
- Business insights + numeric interpretation

### Dataset Description:

The dataset consists of:

📌 Banking Stocks

Daily historical data for selected BIST-listed banks, including:
- Open
- High
- Low
- Close
- Adjusted Close
- Volume

📌 Benchmark
- BIST100 index (XU100) downloaded from Yahoo Finance
- Fields: Date, Adj Close, Daily Returns

🧹 Data Preprocessing
- Missing values handled
- Dates standardized
- Daily returns calculated
- Outliers detected using Z-scores
- Merged bank returns with BIST100 returns
- Portfolio constructed using equal weights
- Regression variables created (market factor)

### Methodology
✔ Daily Return Analysis

Compute log returns and visualize distribution, volatility, and trends.

✔ Correlation Analysis

Identify how strongly banks move together (+ heatmap).

✔ Outlier Detection

Detect abnormal return/volume spikes and identify potential causes (macro news, earnings, rate changes, geopolitical events).

✔ Leader–Follower Pattern

Cross-correlation to test whether large banks influence smaller ones.

✔ Portfolio Construction

Equal-weighted portfolio of all banks.

✔ Compare with BIST 100

Cumulative returns, volatility, Sharpe ratio, and beta.

✔ Strategy Backtesting

50-day moving average (MA50) strategy vs. Buy & Hold.

✔ Regression & Factor Analysis

OLS to estimate portfolio sensitivity to market returns.

### Key Insights
1. Portfolio vs Market
- Portfolio annualized return: ~54.8%
- BIST100 annualized return: ~20%
- Some banks outperform the index substantially.

2. Risk
- Portfolio volatility: 2.49%
- BIST100 volatility: 0.99%

3. Beta
- Portfolio beta: -0.11 → Almost uncorrelated with market.

4. Moving Average Strategy
- Buy & Hold cumulative return: 10.26× growth
- MA Strategy cumulative return: 5.55× growth
- Buy & Hold outperforms in trending markets.

### Numerical Interpretation
- Sharpe Ratio: Portfolio (1.38) > BIST100 (1.25)
→ Higher risk-adjusted return.
- Negative Beta suggests bank stock portfolio sometimes acts independently of market conditions.
- Correlations among banks are high → sector-driven movement.
- Outliers correspond to news events: Interest rate announcements, Inflation reports, Banking regulations

### Business Insights
- Banking stocks in BIST are highly sensitive to macroeconomic news.
- Sector moves in clusters, meaning shocks spread across banks.
- A diversified portfolio of bank stocks still has sector concentration risk.
- For long-term investors, Buy & Hold outperforms timing strategies in stable macro periods.

### Conclusion
- This data science project demonstrates:
- Banking stocks in BIST are volatile but generate high returns.
- Portfolio performance exceeds the benchmark significantly.
- Market beta is surprisingly low, indicating weak dependence on overall index movement.
- Technical strategies do not consistently outperform Buy & Hold.

### Future Scope
- Add more factors (interest rates, inflation, credit spreads)
- Apply machine learning forecasting models (LSTM, Random Forest)
- Build a Streamlit dashboard (outside Kaggle environment)
- Compare banking sector with other sectors in BIST
- Sentiment analysis using news / Twitter data
