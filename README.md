# Time Series Forecasting Practices and Mini-Projects


...on it..

Welcome to my **Time Series Forecasting** repository — a collection of hands-on experiments and projects. This space explores the full pipeline: from **data preprocessing** to building and validating forecasting models on real-world datasets such as **stock prices**, **weather data**, and **sales trends**.

##  Key Areas Covered

- **Forecasting Models**: ARIMA, Exponential Smoothing, Prophet, LSTM, GRU, AutoARIMA, SARIMA  
- **Preprocessing**: Handling missing data, outliers, and seasonal adjustments  
- **Advanced Techniques**: Ensemble models, hybrid methods, and custom forecasting strategies  
- **Real-World Applications**: Financial, climate, and demand forecasting  

This repository is regularly updated with new techniques and experiments.  
**Contributions and feedback are welcome!**

### The root files...

## Stationarity Tests

### ADF Test (Augmented Dickey-Fuller)
- Hypothesis Test:
  - **Null (H0)**: Series has a unit root → **Non-stationary**
  - **Alt (H1)**: Series is **stationary**

### KPSS Test (Kwiatkowski–Phillips–Schmidt–Shin)
- Hypothesis Test:
  - **Null (H0)**: Series is **stationary**
  - **Alt (H1)**: Series is **non-stationary**

### KS 2-Sample Test (Kolmogorov–Smirnov)
- Tests whether two samples (e.g., different time segments) are from the **same distribution**
- Used to **indirectly evaluate strict stationarity**

---