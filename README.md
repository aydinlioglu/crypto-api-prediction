
# Crypto Coin Analysis Project

This project is a complete end-to-end analysis of cryptocurrency data using the **CoinGecko API**, developed in a Jupyter Notebook environment.  
It allows users to fetch real-time data, visualize trends, and predict future prices using machine learning techniques.

---

## About the API: CoinGecko

This project uses the [CoinGecko API](https://www.coingecko.com/en/api/documentation), which provides free and open access to cryptocurrency market data.

### What We Use from the API:
- `/coins/{id}` — to get general information, description, categories, supply, community & developer stats
- `/coins/{id}/market_chart` — to get historical price data (7, 30, 365 days)

No API key or authentication is required.

Rate Limit: 10–30 requests per minute (as per CoinGecko’s free tier)

---

## Objectives

- Fetch real-time data for any coin using its `coin_id`.
- Display descriptions, community stats, and developer metrics.
- Analyze word frequency from the coin's description.
- Show supply-related data including max and circulating supply.
- Plot price trends for the last 7, 30, and 365 days.
- Apply Linear Regression to forecast the next 3 days’ prices.
- Evaluate model performance using R², MAE, and RMSE metrics.

---

## Features Explained

### 1. User Input
Prompt the user to input a coin ID (e.g., `bitcoin`, `ethereum`, `solana`).

### 2. Coin Description & Word Frequency
- Display the first 500 characters of the coin’s English description.
- Use `re` and `Counter` to count and list the top 10 most frequent words.

### 3. Community and Developer Statistics
- Twitter followers
- Reddit subscribers
- GitHub stars and forks

### 4. Supply Metrics
- Maximum supply
- Circulating supply
- Circulation ratio (calculated and shown as a percentage)

### 5. Price Visualization
- Plot the last 7 days of price data
- Plot additional charts for the last 30 and 365 days

### 6. Forecasting Future Prices
- Use Linear Regression to forecast prices for the next 3 days
- Plot model predictions vs. actuals
- Performance metrics:
  - R² Score (coefficient of determination)
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)

---

## Required Libraries

python
requests
pandas
matplotlib
sklearn
numpy
re
collections.Counter

> Make sure to install missing packages using pip (e.g., `!pip install pandas matplotlib scikit-learn`).

---

## How to Run

1. Launch Jupyter Notebook or JupyterLab.
2. Open the file `coin_API.ipynb`.
3. Run all the cells from top to bottom.
4. When prompted, enter the `coin_id` (e.g., `bitcoin`).
5. View analysis, charts, and predictions.

---

## Project Files

- `coin_API.ipynb` — Main notebook file with code, visualizations, and model
- `README.md` — Project documentation and usage instructions

---

## Contact

For questions or improvements, feel free to reach out or fork the project on GitHub!
