### Data

The raw dataset contained daily stock prices for 1,199 S&P 500 companies from 1993–2019.

**Raw data structure**

| Date       | AAPL US Equity | MSFT US Equity | AMZN US Equity | GOOG US Equity | ... |
| ---------- | -------------: | -------------: | -------------: | -------------: | --- |
| 1993-09-07 | 9.85 | 10.83 | 18.18 | 7.58 | ... |
| 1993-09-08 | 9.90 | 10.79 | 18.22 | 7.60 | ... |
| 1993-09-09 | 9.88 | NaN | 18.11 | 7.55 | ... |

*Only a small snippet is shown due to the size of the dataset (1,199 columns × 9,459 rows).*

### Data Cleaning

The raw data underwent several preprocessing steps before modelling:

- Converted dates to `datetime` format.
- Removed stocks with insufficient historical coverage.
- Forward-filled short missing-value gaps.
- Winsorised extreme daily returns to ±50%.
- Added GICS sector labels for each stock.
- Removed inactive and illiquid stocks.
- Selected the top 5 stocks from each sector based on training-period Sharpe ratio.

This reduced the investment universe from **1,199 stocks to 55 stocks**.

### Final Dataset

The optimisation models were trained using **daily percentage returns**, with each column representing a stock and each row representing a trading day.

| Date | ECL US Equity | SHW US Equity | APD US Equity | PPG US Equity | VMC US Equity |
|------|--------------:|--------------:|--------------:|--------------:|--------------:|
|1993-09-08|0.0000|0.00737|0.00301|-0.00182|-0.00283|
|1993-09-09|0.01445|0.01463|-0.02096|-0.00742|-0.00831|
|1993-09-10|0.00856|0.01086|0.00000|0.01864|-0.00551|
|1993-09-11|0.00000|0.00000|0.00000|0.00000|0.00000|
|1993-09-12|0.00000|0.00000|0.00000|0.00000|0.00000|

*Only a representative subset of columns and rows is shown.*
