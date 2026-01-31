# Financial Time-Series Analysis: The 2008 Banking Crisis

Analysis of historical stock price data for major U.S. banks (BAC, JPM, GS, MS, C, WFC) to study volatility, correlations, and technical indicators before, during, and after the 2008 financial crisis.

---

## Project Overview
In this project, I analyzed 10 years of daily stock price data (2006–2016) for the six largest U.S. banks to understand how the financial crisis affected the sector and how different institutions recovered over time.

---

## Exploratory Data Analysis
Before applying technical indicators, I explored long-term price behaviour and daily returns.

### 1. Long-Term Price Trends
![Bank Stock Trends](bank_stock_trends.png)  
Plotted closing prices over a 10-year period to visualise the 2008 crash and compare recovery patterns across banks.

### 2. Returns and Volatility
![Returns Pairplot](returns_pairplot.png)  
Analysed daily percentage returns to compare volatility levels and identify higher-risk stocks within the sector.

---

## Technical Analysis: Bank of America (BAC)
I used Bank of America as a case study to apply common technical indicators.

### 3. 30-Day Moving Average
![BAC Moving Average](bac_moving_avg.png)  
Applied a 30-day rolling average to smooth short-term price fluctuations and highlight broader trends during periods of high volatility.

### 4. Bollinger Bands
![BAC Bollinger Bands](bac_bollinger_bands.png)  
Used Bollinger Bands to examine how BAC’s price moved relative to its recent mean and standard deviation, highlighting periods of unusually high or low prices.

---

## Correlation Analysis
![Bank Correlation Clustermap](bank_correlation_clustermap.png)  
Computed correlations between bank stocks and applied hierarchical clustering to show how closely the banks moved together during periods of market stress.

---

## Key Takeaways
- Major banks experienced their worst daily returns around the peak of the financial crisis, demonstrating the impact of macroeconomic events on stock prices.
- Citigroup and Morgan Stanley showed higher volatility compared to other banks in the dataset.
- Financial data was sourced programmatically using `yfinance` and processed using pandas, including handling MultiIndex DataFrames.

---

## How to Run
```bash
pip install pandas_datareader yfinance
jupyter notebook "04-Finance Project.ipynb"
