# Google Stock Analysis: Quant Modeling & Deep Learning Forecasting

A comprehensive quantitative finance and machine learning project analyzing Alphabet Inc. (GOOGL) stock. This project bridges traditional statistical finance (Geometric Brownian Motion & Black-Scholes) with modern deep learning architectures (RNN, LSTM, GRU) to forecast prices and price financial derivatives.

## Features

### Part 1: Quantitative Finance & Option Pricing
* **Exploratory Data Analysis (EDA):** Rolling volatility, log returns, and correlation studies.
* **Monte Carlo Simulations:** Future price forecasting utilizing Geometric Brownian Motion (GBM).
* **Options Pricing:** Implementation of the Black-Scholes-Merton model for European Call and Put options.

### Part 2: Deep Learning & Time-Series Forecasting
* **Data Pipeline:** Advanced preprocessing, min-max scaling, and sequence generation for recurrent networks.
* **Architectures Implemented:** Vanilla RNN, Long Short-Term Memory (LSTM), and Gated Recurrent Units (GRU).
* **Comparative Analysis:** Performance benchmarking using metrics like RMSE, MAE, and MAPE to evaluate predictive accuracy.

---

## 🛠️ Tech Stack
* **Languages:** Python
* **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, Scikit-Learn, TensorFlow/Keras (or PyTorch)
* **Models:** Black-Scholes, Geometric Brownian Motion, Vanilla RNN, LSTM, GRU

---

## Key Insights & Results

### 1. Quantitative Modeling
* **GBM Simulation:** Generated $N$ simulation paths over a $T$-day horizon to establish probabilistic price bounds.
* **Options Pricing:** Calculated theoretical values for near-the-money options, comparing historical vs. implied volatility impacts.

### 2. Deep Learning Performance

2. Deep Learning Performance

<img width="338" height="227" alt="image" src="https://github.com/user-attachments/assets/98263257-c6c1-415c-9ad6-bcd7ba24cbe0" />


> **Summary:** The GRU/LSTM model outperformed the Vanilla RNN by 81.6% in RMSE, successfully capturing long-term temporal dependencies in stock trends without suffering from severe vanishing gradient issues.
