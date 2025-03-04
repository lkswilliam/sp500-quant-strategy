# S&P 500 Quant Strategy
## Unsupervised Learning, Efficient Frontier Optimization, and Monthly Rebalancing

This project develops a quantitative trading strategy for the S&P 500 using 10 years of daily data (2015–2025) from `yfinance`. It calculates monthly technical indicators (RSI, MACD, etc.), selects stocks via K-means clustering, and optimizes portfolios monthly with `PyPortfolioOpt`’s Efficient Frontier for maximum Sharpe ratio. The strategy is rebalanced monthly and backtested over 5 years against the S&P 500, with rolling normalization to eliminate biases.

## Features
- **Data**: 10 years of S&P 500 daily data, aggregated monthly.
- **Indicators**: RSI, MACD, Bollinger Bands, ATR, Garman-Klass Volatility, Dollar Volume.
- **Stock Selection**: K-means clustering.
- **Optimization**: Efficient Frontier with monthly rebalancing for maximum Sharpe ratio.
- **Backtesting**: 5-year performance against S&P 500.
- **Bias Mitigation**: Rolling normalization to remove look-ahead bias.

## Prerequisites
```bash
pip install pandas numpy yfinance pandas-ta scikit-learn pypfopt matplotlib
