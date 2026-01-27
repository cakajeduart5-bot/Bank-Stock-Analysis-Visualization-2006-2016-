# **Financial Time-Series Analysis: The 2008 Banking Crisis**
*A quantitative study of major U.S. bank stocks (BAC, JPM, GS, MS, C, WFC) to analyze market volatility, risk profiles, and sector correlation during the Great Recession.*

---

## **Project Overview**
[cite_start]This project explores 10 years of historical stock data (2006–2016) to audit the behavior of the "Big Six" banks during one of the most volatile periods in financial history[cite: 206, 210]. [cite_start]The goal was to demonstrate proficiency in handling high-frequency time-series data and extracting actionable risk metrics[cite: 206].

---

## **Financial EDA & Market Insights**
[cite_start]Before modeling, I performed deep-dive analytics to identify structural trends in equity behavior[cite: 355].

### **1. Long-Term Sector Trends**
![Bank Stock Trends](bank_stock_trends.png)
[cite_start]Visualized the 10-year trajectory of Closing prices[cite: 720]. [cite_start]I specifically audited the "recovery" period post-2009 to observe how different institutional risk profiles influenced price action[cite: 210, 720].

### **2. Volatility & Return Analysis**
![Returns Pairplot](returns_pairplot.png)
[cite_start]Generated a pairplot of daily percentage returns to analyze the "tightness" of sector movement[cite: 415, 419]. 
* [cite_start]**Observation:** The plot identifies significant outliers (specifically Citigroup), which I cross-referenced against historical events like the 2011 stock split[cite: 415, 551].

### **3. Technical Analysis: BAC Moving Averages**
![BAC Moving Average](bac_moving_avg.png)
[cite_start]I focused a technical audit on Bank of America (BAC) during the 2008 crash, applying a 30-day rolling window to visualize the smoothing of high-volatility price action[cite: 814, 815, 819].

### **4. Sector Correlation & Clustering**
![Bank Correlation Clustermap](bank_correlation_clustermap.png)
[cite_start]Applied hierarchical clustering to correlation matrices of stock prices[cite: 952, 953].
* [cite_start]**The Insight:** This revealed the mathematical proximity of specific banks (e.g., JPM and WFC) during market stress, demonstrating a "sector-wide" contagion effect[cite: 953].

---

## **Scientific Rigor & Logic**
* [cite_start]**Event Correlation:** Identified Jan 20, 2009 (Inauguration Day) as a shared worst-return day for 4 major banks, proving how political macro-events drive market sentiment[cite: 531, 532].
* [cite_start]**Risk Categorization:** Calculated standard deviations to classify the "riskiest" stocks, noting how Citigroup and Morgan Stanley displayed significantly higher volatility compared to peers in 2015[cite: 568, 570, 584, 595].

---

## **Tools & Technical Skills**
- [cite_start]**Python Libraries:** Pandas (MultiIndex), NumPy, Matplotlib, Seaborn[cite: 220, 221, 222, 223, 347, 418].
- [cite_start]**Data Sourcing:** Utilized `yfinance` to programmatically download historical OHLCV data[cite: 226, 301].
- [cite_start]**Financial Analytics:** Time-series wrangling, rolling windows, and percentage change modeling[cite: 381, 382, 815, 819].

---

## **How to Run**
```bash
pip install pandas_datareader yfinance
jupyter notebook "04-Finance Project.ipynb"
