## Techniques to Make Data Stationary

###  1. Differencing
- **First-order differencing**: `Y(t) - Y(t-1)`
- **Second-order differencing**: Applied on differenced series
- **Seasonal differencing**: `Y(t) - Y(t-s)` where `s` is seasonal period

###  2. Transformations
- **Logarithmic transformation**
- **Square root / Cube root**
- **Box-Cox transformation**
- **Power transformation**

Used to stabilize **variance** (remove heteroscedasticity)

###  3. Detrending
- **Linear detrending**: Fit and subtract linear regression trend
- **Moving average detrending**: Subtract a smoothed (rolling) mean

###  4. Seasonal Adjustment
- **STL decomposition (Seasonal-Trend decomposition using Loess)**
- **Classical decomposition (Additive / Multiplicative)**

---
