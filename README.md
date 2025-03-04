# S&P 500 Quant Strategy
### *Unsupervised Learning, Efficient Frontier Optimization, and Monthly Rebalancing*

This project crafts a quantitative trading strategy for the S&P 500, using 10 years of daily data (2015–2025) from `yfinance`. It computes monthly technical indicators (RSI, MACD, etc.), selects stocks with K-means clustering, and optimizes portfolios monthly using `PyPortfolioOpt`’s Efficient Frontier for maximum Sharpe ratio. With monthly rebalancing and a 5-year backtest against the S&P 500, rolling normalization ensures precision and eliminates biases.

---

## Features
- **Data**: 10 years of S&P 500 daily data, aggregated monthly.
- **Indicators**: RSI, MACD, Bollinger Bands, ATR, Garman-Klass Volatility, Dollar Volume.
- **Stock Selection**: K-means clustering for data-driven picks.
- **Optimization**: Monthly Efficient Frontier for max Sharpe ratio with rebalancing.
- **Backtesting**: 5-year performance benchmarked against S&P 500.
- **Precision**: Rolling normalization to banish look-ahead bias.

## Prerequisites
```bash
pip install pandas numpy yfinance pandas-ta scikit-learn pypfopt matplotlib
