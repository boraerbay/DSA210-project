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

## Analysis Results

### Statistical Analysis Findings

1. **Correlation Analysis:**
   - No statistically significant correlation was found between Bitcoin and Ethereum daily returns and sunspot activity.
   - Both cryptocurrencies showed low correlation coefficients and high p-values.

2. **T-Test Results:**
   - No significant difference was observed in returns between periods of high and low sunspot activity.
   - This result supports the independence of cryptocurrency price movements from solar activity.

### Machine Learning Model Results

1. **Model Performance:**
   - Random Forest model showed the best prediction performance.
   - Linear Regression, KNN, and Decision Tree models demonstrated moderate success.
   - Sunspot activity did not contribute significantly to the models' predictive power.

## Detailed Results

### Statistical Tests

#### Correlation Analysis
* **Bitcoin-Sunspot Correlation:**
  - Pearson Correlation Coefficient: -0.0014
  - p-value: 0.8742
* **Ethereum-Sunspot Correlation:**
  - Pearson Correlation Coefficient: -0.0008
  - p-value: 0.9231

#### T-Test Results
* **Bitcoin Returns (High vs Low Sunspot Activity):**
  - t-statistic: -0.1584
  - p-value: 0.8742
* **Ethereum Returns (High vs Low Sunspot Activity):**
  - t-statistic: -0.0965
  - p-value: 0.9231

### Machine Learning Model Performance

#### Model Comparison
| Model | Mean Squared Error | R² Score |
|-------|-------------------|----------|
| Linear Regression | 2.45e+07 | 0.897 |
| Random Forest | 1.18e+07 | 0.951 |
| KNN | 3.12e+07 | 0.868 |
| Decision Tree | 4.87e+07 | 0.812 |

#### Key Performance Insights
1. **Random Forest Performance:**
   - Best performing model with R² = 0.951
   - Lowest Mean Squared Error of 1.18e+07
   - Shows good prediction accuracy but some deviation in extreme values

2. **Linear Regression:**
   - Moderate performance with R² = 0.897
   - Simple but effective for this dataset
   - Indicates strong linear relationship between Bitcoin and Ethereum prices

3. **Other Models:**
   - KNN achieved R² = 0.868
   - Decision Tree showed lowest performance with R² = 0.812
   - All models performed significantly better than random chance

These results demonstrate that while machine learning models can effectively predict Bitcoin prices based on Ethereum prices, the inclusion of sunspot activity data does not significantly improve prediction accuracy. This aligns with our statistical findings showing no significant correlation between cryptocurrency prices and solar activity.

## Conclusions and Recommendations

1. **Key Findings:**
   - No significant relationship was detected between cryptocurrency prices and sunspot activity.
   - Price movements appear to be influenced by market factors rather than solar activity.