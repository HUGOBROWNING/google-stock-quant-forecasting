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

+-------------------+------------+------------+------------+
| Model             | MAE        | RMSE       | R-squared  |
+-------------------+------------+------------+------------+
| Fine-tuned GRU    | 3.373477   | 4.831708   | 0.995383   |
| Initial GRU       | 4.757230   | 7.207941   | 0.989724   |
| Initial LSTM      | 5.670447   | 8.256966   | 0.986516   |
| Fine-tuned LSTM   | 8.197898   | 10.505571  | 0.978171   |
| Initial RNN       | 15.316250  | 26.323886  | 0.862946   |
+-------------------+------------+------------+------------+

> **Summary:** The GRU/LSTM model outperformed the Vanilla RNN by 81.6% in RMSE, successfully capturing long-term temporal dependencies in stock trends without suffering from severe vanishing gradient issues.
