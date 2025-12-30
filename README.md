# Trader Behavior vs Market Sentiment

## Overview
This project analyzes how trader behavior and performance vary across different Bitcoin market sentiment regimes using historical trade data and the Bitcoin Fear & Greed Index. The goal is to understand how sentiment influences trade size, profitability, and risk-taking behavior.

---

## Datasets
- **Hyperliquid Historical Trader Data**: Trade-level data including position size, side, and realized PnL.
- **Bitcoin Fear & Greed Index**: Daily market sentiment classification (Extreme Fear to Extreme Greed).

The processed dataset is provided in compressed format due to GitHub file size limits.

---

## Methodology
- Cleaned and standardized raw trade and sentiment datasets.
- Parsed localized trade timestamps and aligned them with daily sentiment data.
- Merged datasets on date to associate each trade with market sentiment.
- Engineered additional features such as profitability indicators and risk-adjusted PnL.
- Performed exploratory analysis to compare trader behavior across sentiment regimes.

---

## Key Insights
- Trade sizes follow a heavy-tailed distribution, with larger trades occurring more frequently during Greed and Extreme Greed phases.
- Average profitability increases during Greed phases but is accompanied by higher volatility.
- Median trade-level PnL is approximately zero across all sentiment regimes, indicating that profits are driven by tail events rather than typical trades.
- Fear-driven markets show wider PnL dispersion, suggesting emotional and inconsistent trading behavior.

---

## Repository Structure
ds_gohul/
├── notebook_1.ipynb
├── csv_files/
│ └── processed_trader_sentiment_data.csv.zip
├── outputs/
│ ├── pnl_vs_sentiment.png
│ ├── trade_size_boxplot_log.png
│ └── pnl_distribution.png
├── ds_report.pdf
└── README.md


---

## Tools & Libraries
- Python
- pandas, numpy
- matplotlib, seaborn
- Google Colab

---

## Notes
- The analysis was conducted entirely in Google Colab as required.
- The processed CSV is provided as a `.zip` file due to GitHub’s 25 MB upload limit.

