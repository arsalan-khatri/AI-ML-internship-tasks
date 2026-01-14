# Task 2: Stock Market Prediction & Forecasting

## 1. Task Objective
The objective of this project was to build a Machine Learning model to predict the **future closing price** of a stock (Apple Inc.) based on its historical data. The project aims to:
- Analyze historical stock trends (2021-2026).
- Visualize price movements and moving averages.
- Train a regression model to forecast the *next day's* closing price.

## 2. Dataset Used
- **Source:** Historical Stock Data (Loaded from `data.csv`).
- **Time Period:** January 2021 to January 2026.
- **Total Records:** 1278 days of trading data.
- **Key Features:**
  - `Open`: Opening price of the day.
  - `High`: Highest price of the day.
  - `Low`: Lowest price of the day.
  - `Close`: Closing price (Used to generate the Target).
  - `Volume`: Number of shares traded.

## 3. Methodologies & Models Applied
### Data Preprocessing
- **Cleaning:** Handled missing values and removed commas from the 'Volume' column.
- **Type Conversion:** Converted `Date` to datetime objects and numeric columns to float.
- **Feature Engineering:**
  - Calculated **50-Day Moving Average (MA50)** for trend analysis.
  - Created a `Next_Close` target variable by shifting the closing price backwards by 1 day (predicting $t+1$ using data from $t$).

### Machine Learning Model
- **Algorithm:** **Linear Regression** (`sklearn.linear_model`).
- **Training Strategy:** Used an 80-20 Train-Test split with `shuffle=False` to maintain the chronological order of time-series data.
- **Input Features:** `Open`, `High`, `Low`, `Volume`.

## 4. Key Results and Findings
### Performance
- **Model Accuracy:** The Linear Regression model achieved a score of **97.15%**, indicating a strong correlation between daily indicators and the next day's price.

### Insights
- **Trend Analysis:** The 50-Day Moving Average plot showed the overall upward/downward trends, filtering out daily noise.
- **Volatility:** Daily return analysis highlighted the market's volatility, identifying the single biggest profit day (+15.33%) and loss day (-9.25%).

### Future Prediction
- The model successfully predicted the share price for **Jan 7, 2026**, to be approximately **$263.11** based on the previous day's market data.
