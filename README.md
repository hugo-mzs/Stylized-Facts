# 📊 Stylized Facts of Financial Time Series

This project analyzes Coca-Cola stock data to empirically verify the **8 stylized facts** commonly observed in financial markets. Using statistical tests and visualizations, we evaluate whether these stylized facts hold on the dataset.

---

## ✅ Stylized Facts Covered

1. **Fat tails**  
   Returns exhibit higher kurtosis than the normal distribution, with extreme values occurring more often than expected under Gaussian assumptions.

2. **Volatility clustering**  
   High-volatility periods are followed by high-volatility periods, and low-volatility periods follow low-volatility periods.

3. **Absence of autocorrelation in raw returns**  
   Asset returns show little to no significant linear autocorrelation.

4. **Leverage effect**  
   Negative returns are often followed by higher volatility than positive returns of equal magnitude.

5. **Aggregational Gaussianity**  
   As we move from daily to weekly or monthly frequencies, returns become more normally distributed.

6. **Volume-volatility correlation**  
   Higher trading volume tends to be associated with higher price volatility.

7. **Long memory in volatility**  
   Squared and absolute returns display significant autocorrelation even at long lags.

8. **Asymmetry in return distribution**  
   The distribution of returns is typically skewed, often to the left for equity data.

---

## 🔬 Tests and Visualizations

For each stylized fact, we perform the following checks:

- **Fat tails**
  - Histogram and kernel density estimate (KDE)
  - Comparison to normal distribution
  - QQ-plot
  - Kurtosis and Jarque-Bera test

- **Volatility clustering**
  - Rolling volatility (std)
  - ACF plot of squared returns

- **Absence of autocorrelation**
  - ACF plot of raw returns
  - Ljung-Box test (if implemented)

- **Leverage effect**
  - Conditional volatility after positive vs negative returns
  - Scatter plot of past returns vs future squared returns

- **Aggregational Gaussianity**
  - QQ-plots at daily, weekly, and monthly frequencies
  - Comparison of histograms

- **Volume-volatility correlation**
  - Scatter plot of volume vs squared returns

- **Long memory in volatility**
  - ACF plots of |returns| and returns² over extended lags

- **Asymmetry**
  - Skewness calculation
  - Histogram with skewness annotation

---

## 🧰 Dependencies

- Python 3.x
- `pandas`
- `numpy`
- `matplotlib`
- `scipy`
- `statsmodels`
- `yfinance` *(if downloading live data)*






