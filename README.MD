# Credit Risk & CAPM Analysis

## Overview

This repository contains code and data for analyzing stock returns using the **Capital Asset Pricing Model (CAPM)** and applying **risk modeling techniques**. The workflow demonstrates how to calculate betas, evaluate portfolio performance, and visualize risk–return tradeoffs using real stock data.

---

## Contents

* **`stocks_dataset.csv`** → Historical stock price dataset (FB, TWTR, NFLX, BA, T, MGM, TSLA, S\&P 500).
* **`Finance_101_Capital_Asset_Pricing_Model_(CAPM)-Copy5.ipynb`** → Jupyter notebook implementing CAPM, regression analysis, and portfolio optimization.

---

## Key Features

* Data preprocessing: cleaning, scaling, normalization of stock price data.
* Return calculation: daily returns and excess returns relative to market.
* CAPM Estimation:

  * Linear regression of stock excess returns vs. S\&P 500.
  * Calculation of **β (systematic risk)** and **α (Jensen’s alpha)**.
* Portfolio Construction:

  * Modeled **11 allocation scenarios (0%–100%)**.
  * Constructed the **efficient frontier** curve.
* Risk Metrics:

  * Calculated **variance, standard deviation, covariance, correlation**.
  * Computed **Sharpe ratio** for portfolio evaluation.

---

## Results & Insights

* **Betas ranged from \~0.75 (defensive stocks like AT\&T) to \~1.65 (higher-risk stocks like MGM).**
* **Sharpe ratio \~0.34** for baseline portfolio; optimization improved it to \~0.7.
* **Logistic Regression model (credit risk dataset)** achieved **up to 83% accuracy** in predicting defaults.
* Efficient frontier visualization showed clear tradeoffs between risk and return across allocation scenarios.

---

## Technologies Used

* Python (NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, Statsmodels)
* Jupyter Notebook

---

## How to Run

1. Clone this repo:

   ```bash
   git clone https://github.com/yourusername/yourrepo.git
   cd yourrepo
   ```
2. Install requirements:

   ```bash
   pip install -r requirements.txt
   ```
3. Open Jupyter Notebook:

   ```bash
   jupyter notebook
   ```
4. Run **`Finance_101_Capital_Asset_Pricing_Model_(CAPM)-Copy5.ipynb`** to reproduce results.

---

## Future Improvements

* Add Monte Carlo simulation for portfolio stress testing.
* Extend to multi-factor models (Fama–French 3 factor).
* Deploy results on an interactive dashboard (Plotly/Streamlit).


