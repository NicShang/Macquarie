# AUD/USD Option Risk Diagnostics Tool

## Project Overview

This project is a Python-based risk diagnostics tool designed to evaluate and visualize the risk sensitivities (Greeks) of European-style FX options on AUD/USD, using the Black-Scholes pricing framework.

By simulating call and put options across various spot prices and expiry horizons (3M, 6M, 12M), the tool helps assess how volatility, time decay, and delta exposure evolve under changing market conditions—critical for traders managing directional and volatility risk in FX markets.

## Key Features

- **Custom Black-Scholes Engine**: Implemented a modular BS model in Python to compute option prices and Greeks (Delta, Gamma, Vega, Theta, Rho).
- **Real Market Data**: Pulled minute-level AUD/USD FX rates to anchor the analysis on current market conditions.
- **Interactive Risk Visualization**: Used Plotly to dynamically plot each Greek across spot price ranges and tenors, supporting real-time decision diagnostics.
- **Expiry Sensitivity Analysis**: Compared short- and long-dated options to evaluate how time-to-maturity influences vega risk, delta convexity, and theta decay.

## Key Insights

- **Vega** peaks around the at-the-money strike, with longer-tenor options showing significantly higher sensitivity to volatility shifts—highlighting the importance of vega hedging in macro or carry trades.
- **Theta** is most negative around ATM strikes for short-dated options, indicating rapid time decay—a key consideration for short volatility positions or calendar spreads.
- **Delta** curves shift as expiry increases, revealing more gradual slope changes, consistent with lower gamma risk in long-dated options.

## Relevance to FIC Trading

- Demonstrates deep understanding of FX options pricing mechanics and non-linear payoff structures.
- Applies structured quantitative techniques to evaluate risk under real-world trading scenarios.
- Reinforces ability to translate market data and theoretical models into practical decision-support tools—aligned with CBA’s AI-first approach to flow trading and hedging.

## Technologies Used

- Python (NumPy, Pandas, SciPy, Plotly)
- Quantmod API for market data
- Jupyter Notebook for modular diagnostics and visualization

---
