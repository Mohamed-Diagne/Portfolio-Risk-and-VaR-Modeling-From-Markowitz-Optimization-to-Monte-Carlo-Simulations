# 📊 Portfolio Optimization and Risk Modeling: VaR, CVaR, and Macroeconomic Stress Testing

## Overview
This project builds a complete portfolio risk management pipeline: from **data collection** to **portfolio optimization**, **VaR/CVaR estimation**, **backtesting**, and **macro stress analysis**.  
It simulates both normal and stressed financial conditions.

---

## 🎯 Objectives
* Optimize a diversified portfolio using **Markowitz optimization** (weight constraints applied).
* Quantify portfolio risk through **Historical**, **Parametric (Student-t)**, and **Monte Carlo** VaR and CVaR models.
* Validate models using **Kupiec tests**.
* Analyze **Monte Carlo VaR sensitivity** to macroeconomic shocks.

---

## 🛠 Methodologies Implemented
**Portfolio Construction:**
* Markowitz framework with rolling rebalancing.
* Comparison with CAC 40 benchmark.

**Risk Estimation:**
* Value at Risk (VaR): Historical, Parametric Student-t, Monte Carlo simulations.
* Conditional VaR (CVaR): Historical, Parametric Student-t, Monte Carlo.

**Backtesting:**
* Kupiec Proportion of Failures (POF) test.

**Macro Stress Testing:**
* OLS regressions linking macroeconomic variables (Unemployment, Consumer Sentiment, Financial Conditions, Corporate Bond Spreads, Oil Prices) to VaR dynamics.

---

## 📚 Data Sources
* **Assets**: 40 diversified stocks and commodities (CAC 40 + global equities + commodities).
* **Macroeconomic Indicators**: FRED API (Unemployment Rate, NFCI, etc.).
* **Period**: 2010-01-01 to present.

---

## 📈 Key Results
* Optimized portfolio **outperformed** CAC 40 with lower volatility.
* **Monte Carlo Student-t VaR** delivered the most robust risk estimation.
* Macro variables (especially Unemployment and Financial Conditions) significantly explain VaR fluctuations.


---

## 🚀 How to Run
1. Clone the repository.
2. Install dependencies:
```bash
pip install -r requirements.txt

---

## 🔮 Future Improvements
* Test GARCH models for volatility clustering.
* Integrate copula-based dependency models for better tail risk estimation.
* Extend to portfolio-level Expected Shortfall under Basel III/IV frameworks.

---

## 📖 References
* Jorion, P. (2006). Value at Risk: The New Benchmark for Managing Financial Risk.
* McNeil, Frey & Embrechts (2015). Quantitative Risk Management: Concepts, Techniques and Tools.
* Glasserman, P. (2004). Monte Carlo Methods in Financial Engineering.
---

## 📑 License
This project is for educational purposes only.

