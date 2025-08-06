# 📊 Time Series Smoothing Techniques

This repository contains common smoothing methods used in time series analysis to reduce noise and highlight patterns.

---

## 1. Simple Moving Average (SMA)

- Averages the last `k` data points to smooth the series.

**Formula:**
\[
\text{SMA}_t = \frac{1}{k} \sum_{i=0}^{k-1} y_{t-i}
\]

---

## 2. Weighted Moving Average (WMA)

- Like SMA, but gives more weight to recent observations.

**Formula:**
\[
\text{WMA}_t = \frac{\sum_{i=1}^{k} w_i y_{t-i+1}}{\sum_{i=1}^{k} w_i}
\]

---

## 3. Exponential Moving Average (EMA)

- Applies exponentially decreasing weights to past values.

**Formula:**
\[
\text{EMA}_t = \alpha y_t + (1 - \alpha) \cdot \text{EMA}_{t-1}
\]

---

## 4. Simple Exponential Smoothing (SES)

- Smooths data assuming no trend or seasonality.

**Formula:**
\[
S_t = \alpha y_t + (1 - \alpha) S_{t-1}
\]

---

## 5. Double Exponential Smoothing (Holt’s Linear Trend)

- Adds trend component to SES.

**Formulas:**
\[
\begin{aligned}
L_t &= \alpha y_t + (1 - \alpha)(L_{t-1} + T_{t-1}) \\
T_t &= \beta (L_t - L_{t-1}) + (1 - \beta) T_{t-1} \\
\hat{y}_{t+h} &= L_t + h T_t
\end{aligned}
\]

---

## 6. Triple Exponential Smoothing (Holt-Winters Method)

- Handles both trend and seasonality.

**Additive Version Formulas:**
\[
\begin{aligned}
L_t &= \alpha (y_t - S_{t-s}) + (1 - \alpha)(L_{t-1} + T_{t-1}) \\
T_t &= \beta (L_t - L_{t-1}) + (1 - \beta) T_{t-1} \\
S_t &= \gamma (y_t - L_t) + (1 - \gamma) S_{t-s} \\
\hat{y}_{t+h} &= L_t + h T_t + S_{t-s+h}
\end{aligned}
\]

---
