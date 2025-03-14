# Analyzing the Relationship Between Cryptocurrency Prices and Solar Activity

## Project Overview
My project aims to investigate the potential relationship between cryptocurrency price fluctuations and solar activity. By analyzing **Bitcoin and Ethereum price histories** alongside **daily sunspot data**, we will examine whether solar activity has any measurable influence on cryptocurrency markets.

## Motivation
Cryptocurrency markets are highly volatile and influenced by various factors, including macroeconomic trends, investor sentiment, and technical developments. However, some researchers have speculated that external environmental factors, such as solar activity, might also play a role in financial market behavior. This project seeks to explore whether there is any correlation between sunspot activity and cryptocurrency price movements.

## Data Sources

### 1. Bitcoin Price History (`bitcoin_price.csv`)
- **Description:**  
  This dataset contains historical Bitcoin (BTC) price data in USD, including daily open, close, high, and low prices.
- **Source and Access:**  
  - Provided as a CSV file.
  - **Kaggle Reference:** [Bitcoin Price History](https://www.kaggle.com/datasets/saswattulo/bitcoin-price-history-btc-usd)

### 2. Ethereum Price History (`ethereum_data.csv`)
- **Description:**  
  This dataset includes historical Ethereum (ETH) price data in USD, with daily open, close, high, and low prices.
- **Source and Access:**  
  - Provided as a CSV file.
  - **Kaggle Reference:** [Ethereum Price Data](https://www.kaggle.com/datasets/varpit94/ethereum-data)

### 3. Daily Sunspot Activity (`daily_sunspots.csv`)
- **Description:**  
  This dataset contains daily sunspot observations from 1850 to 2025, representing solar activity levels.
- **Source and Access:**  
  - Provided as a CSV file.
  - **Kaggle Reference:** [Daily Sunspot Data](https://www.kaggle.com/datasets/patrickfleith/daily-sunspots-dataset?select=daily_sunspots_time_series_1850-01_2025-01.csv)

## Project Proposal and Methodology

### Objectives
- **Primary Objective:**  
  To determine if there is any correlation between daily sunspot activity and cryptocurrency price fluctuations.
- **Secondary Objective:**  
  To identify whether extreme solar activity (e.g., solar storms) coincides with significant cryptocurrency market events.

### Methodology
1. **Data Preprocessing:**  
   - Clean all datasets by handling missing values and ensuring date alignment.
   - Standardize data formats and convert timestamps if necessary.
2. **Data Integration:**  
   - Merge the cryptocurrency price datasets with the sunspot activity dataset based on matching dates.
   - Create new variables such as moving averages and volatility indicators.
3. **Statistical Analysis:**  
   - Perform correlation analysis to assess potential relationships between sunspot activity and price changes.
   - Use time series analysis and regression modeling to explore patterns.
4. **Visualization:**  
   - Develop line charts to visualize price trends and sunspot activity over time.
   - Use scatter plots and heatmaps to highlight potential correlations.
5. **Interpretation and Reporting:**  
   - Analyze the results to determine whether solar activity has any noticeable effect on cryptocurrency markets.
   - Discuss limitations and suggest areas for future research.
