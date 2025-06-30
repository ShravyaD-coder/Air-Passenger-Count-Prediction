# Time Series Forecasting on Air Passengers Dataset

This project demonstrates time series forecasting on the classic **Air Passengers dataset**, comparing the performance of three deep learning models — **LSTM**, **TCN**, and **TFT** — using the powerful [`darts`](https://github.com/unit8co/darts) time series library.

---

## Models and Results

- **LSTM** and **TFT** outperformed other approaches, achieving:
  - LSTM: **MAPE = 2.67%**
  - TFT: **MAPE = 4.73%**

Evaluations were performed on:
- A **fixed 12-month forecasting horizon**
- A **backtesting process**, which simulates how the models would have performed over multiple rolling windows on past data.

---

## About the Tools Used

### Darts
- A Python library for easy manipulation and forecasting of time series.
- Supports classical models (ARIMA, Theta), machine learning regressors, and deep learning (LSTM, TCN, TFT, NBEATS, Transformer).
- Simplifies:
  - Time series splitting and preprocessing
  - Training and evaluating models
  - Backtesting and forecasting

### Backtesting
- More robust than a simple train-test split.
- Involves repeatedly training on historical windows and validating on subsequent unseen data.
- Provides a realistic estimate of forecasting performance over time.

### Models Compared
- **LSTM (Long Short-Term Memory):** A type of RNN capable of learning long-range dependencies, ideal for time series sequences.
- **TCN (Temporal Convolutional Network):** Uses causal convolutions to model sequential data without recurrence, enabling parallelism and long effective memory.
- **TFT (Temporal Fusion Transformer):** Combines attention mechanisms with gating layers, designed for multi-horizon forecasting and interpretable insights.

---

## Dataset
- The **Air Passengers dataset** records monthly totals of international airline passengers from 1949 to 1960.
- A standard benchmark for univariate time series forecasting.

---

## Usage

All datasets and code are included in this repository — simply clone and run.

---

