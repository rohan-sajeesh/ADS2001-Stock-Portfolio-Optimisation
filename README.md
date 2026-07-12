# Stock Portfolio Optimisation

Quantitative finance project investigating portfolio construction strategies and optimisation methods to maximise risk-adjusted returns using historical S&P500 stock data.

---

## Overview

Portfolio optimisation is the process of selecting asset allocations that balance expected returns against investment risk.

The project compares 25+ portfolio construction strategies across classical optimisation, risk-based allocation, tail-risk methods, technical strategies, and machine learning-driven approaches using historical S&P500 stock returns.


**Project:** ADS2001 – Data Challenges (Monash University)  
**Project Type:** Group project completed with five members
---

## Objective

The goal of this project was to determine:

- The optimal allocation of stocks within a portfolio
- How different optimisation techniques affect portfolio performance
- Whether advanced mathematical and machine learning approaches outperform naive diversification

The project investigates the relationship between:

- Portfolio return
- Portfolio risk
- Asset allocation
- Risk-adjusted performance

---

## Dataset

Historical daily stock price data from companies included in the **S&P500 index** was used for portfolio analysis.

The dataset was used to calculate:

- Daily returns
- Portfolio returns
- Volatility
- Risk metrics
- Performance measures

**Period:** 1993–2019

---

## Project Workflow

### Data Preparation

- Processed historical stock price data
- Calculated asset returns
- Cleaned and prepared datasets for portfolio modelling
- Selected stocks for portfolio construction

### Portfolio Optimisation

More than 25 portfolio strategies were developed and evaluated across several methodological families:

### Classical Optimisation
- Equal-weight (1/N) benchmark
- Mean-variance optimisation
- Maximum Sharpe ratio optimisation
- Minimum variance optimisation
- Minimum CVaR optimisation

### Risk-Based Methods
- Risk Parity
- Hierarchical Risk Parity (HRP)
- Maximum Diversification
- Minimum Drawdown-based optimisation

### Tail-Risk and Robust Methods
- Entropic Value-at-Risk (EVaR)
- Conditional Value-at-Risk (CVaR)
- Wasserstein Distributionally Robust Optimisation (DRO)
- Composite risk-based optimisation methods

### Dynamic and Machine Learning Strategies
- Moving average strategies
- Momentum strategies
- LSTM return prediction models
- XGBoost return prediction models
- Dynamic portfolio allocation strategies

### Model Evaluation

Portfolio performance was compared using:

- Sharpe ratio
- Portfolio return
- Volatility
- Maximum drawdown
- Value-at-Risk (VaR)
- Conditional Value-at-Risk (CVaR)
- Statistical significance testing using:
  - Jobson-Korkie-Memmel Sharpe ratio tests
  - Bootstrap confidence intervals
  - Holm-Bonferroni correction

---

## Results

The analysis showed that portfolio optimisation methods can improve risk-adjusted performance compared with naive diversification.

Key findings:

- Risk-structure based approaches achieved the strongest out-of-sample performance.
- Maximum Diversification produced the highest Sharpe ratio among tested strategies.
- Machine learning approaches were explored but did not consistently outperform traditional portfolio methods.
- Simple equal-weight diversification remained a strong benchmark.

---

## Technologies Used

- Python
- Pandas
- NumPy
- SciPy
- Scikit-learn
- TensorFlow / Keras
- XGBoost
- CVXPY
- Matplotlib
- Jupyter Notebook

---

## My Contribution

This project was completed as part of a five-person team for **ADS2001 – Data Challenges** at Monash University.

My contributions included:

- Implementing mean-variance portfolio optimisation methods
- Developing Maximum Sharpe ratio optimisation routines
- Analysing efficient frontiers and portfolio performance
- Comparing optimisation results against benchmark strategies
- Contributing to model evaluation and final reporting

---

## Future Improvements

Potential extensions include:

- Longer out-of-sample testing periods
- Incorporating transaction costs
- Applying walk-forward validation
- Exploring additional financial factors and alternative asset classes

---

## License

This project is licensed under the MIT License.
