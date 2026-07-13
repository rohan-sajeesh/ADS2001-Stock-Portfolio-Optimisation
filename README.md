# Stock Portfolio Optimisation

Quantitative finance project investigating portfolio construction strategies and optimisation methods to maximise risk-adjusted returns using historical S&P500 stock data.

---

## Overview

Portfolio optimisation is the process of selecting asset allocations that balance expected returns against investment risk.

This project compares 25+ portfolio construction strategies across classical optimisation, risk-based allocation, tail-risk methods, technical strategies, and machine learning-driven approaches using historical S&P500 stock returns.

**Project:** ADS2001 – Data Challenges (Monash University)  
**Project Type:** Group project completed with five members

---

## Objective

The project aimed to investigate how different portfolio construction strategies balance investment return and risk, and provide evidence-based recommendations for portfolio allocation decisions.

The analysis focused on:

- Comparing traditional, risk-based, and machine learning portfolio strategies
- Evaluating the trade-off between portfolio return and risk
- Determining whether complex optimisation methods outperform simple diversification approaches
- Identifying robust strategies for stakeholder decision-making

---

## Repository Structure

```text
.
├── data/                  Raw and processed datasets
├── notebooks/             Portfolio optimisation notebooks
├── report/                Final technical report
├── Final Presentation/    Presentation slides
├── graphs & images/       Figures used throughout the project
└── README.md              Project documentation
```

Further information about the contents of each folder is provided in the individual folder README files.

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

More than 25 portfolio strategies were developed and evaluated across several categories:

- **Classical Optimisation:** Mean-variance optimisation, Maximum Sharpe ratio, Minimum Variance, and equal-weight benchmarks
- **Risk-Based Methods:** Risk Parity, Hierarchical Risk Parity (HRP), and Maximum Diversification
- **Tail-Risk Methods:** CVaR, EVaR, and Distributionally Robust Optimisation
- **Machine Learning Strategies:** LSTM and XGBoost return prediction models, momentum strategies, and dynamic allocation methods

Strategies were evaluated using risk-adjusted performance metrics including Sharpe ratio, return, volatility, maximum drawdown, and Value-at-Risk.

### Model Evaluation

Portfolio performance was compared using:

- Sharpe ratio
- Portfolio return
- Volatility
- Maximum drawdown
- Value-at-Risk (VaR)
- Conditional Value-at-Risk (CVaR)

Statistical significance was assessed using:

- Jobson-Korkie-Memmel Sharpe ratio tests
- Bootstrap confidence intervals
- Holm-Bonferroni correction

---

## Results

The analysis showed that portfolio optimisation methods can improve risk-adjusted performance compared with naive diversification.

### Key Findings

- Risk-based approaches achieved the strongest out-of-sample performance.
- Maximum Diversification produced the highest Sharpe ratio among all evaluated strategies.
- Machine learning approaches were explored but did not consistently outperform traditional portfolio optimisation methods.
- Equal-weight diversification remained a competitive benchmark.

### Top Performing Strategies

| Rank | Strategy | Sharpe Ratio | Annualised Return |
|-----:|-------------------------------|------------:|------------------:|
| 1 | Static Maximum Diversification | **1.7255** | **19.37%** |
| 2 | Static HRP | 1.7088 | 15.72% |
| 3 | Dynamic Risk Parity | 1.6945 | 15.80% |
| 4 | Static Risk Parity | 1.6409 | 15.97% |
| 5 | 1/N (Equal Weight) | 1.6234 | 16.16% |

*Complete results are available in the project report.*

---

## Stakeholder Recommendations

Based on the analysis, the following recommendations are provided:

- Use equal-weight allocation (1/N) as a strong baseline rather than assuming complex models will always outperform.
- Prioritise risk-based approaches such as Maximum Diversification and Hierarchical Risk Parity when moving beyond equal-weight portfolios.
- Avoid relying solely on return prediction models, as machine learning approaches did not consistently outperform simpler diversification strategies.
- Conduct longer out-of-sample testing and incorporate transaction costs before applying strategies in real investment settings.

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

- Implementing and evaluating portfolio optimisation approaches, including mean-variance optimisation and Maximum Sharpe ratio optimisation
- Analysing portfolio performance, efficient frontiers, and risk-return trade-offs across different strategies
- Applying statistical testing and performance analysis to compare optimisation approaches and interpret results
- Contributing to the development of stakeholder recommendations based on model findings
- Supporting the final report, presentation, and communication of results

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
