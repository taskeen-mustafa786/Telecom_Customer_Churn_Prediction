# Predict_Future_Stock_Prices
A short project demonstrating how to **predict the next day's closing price** of a stock using
historical data and simple machine learning models.

## 📋 Objective
Use historical stock market data to build regression models that forecast the
next trading day's closing price. The focus is on short‑term, one‑day ahead
predictions.

## 📁 Dataset
- Data is retrieved from **Yahoo Finance** via the `yfinance` Python library.
- Historical price information (Open, High, Low, Close, Volume) is used.
- Example ticker: `AAPL` (Apple Inc.), but any valid symbol can be substituted.

## 🛠️ Models Applied
1. **Linear Regression** – a simple baseline for continuous target prediction.
2. **Random Forest Regressor** – a tree‑based ensemble capable of capturing
	 nonlinear relationships.

Both models use the previous day’s Open, High, Low, and Volume as features and
predict the following day’s Close price.

## 📊 Key Results & Findings
- Performance metrics (MSE, R²) are computed on a hold‑out test set.
- A plot comparing actual vs. predicted closing prices illustrates model
	behavior over time.
- In many cases the Random Forest model outperforms linear regression on this
	type of short‑term forecasting problem, though results will vary with the
	chosen stock and time period.

## 🧠 Skills Demonstrated
- Time series data handling with pandas
- Regression modeling with scikit‑learn
- Visualization of predictions vs. reality

## 📝 Usage
Open the notebook at `notebooks/stock_prediction.ipynb` to step through the data
loading, model training, evaluation, and plotting. The README and notebook act
as a self‑contained example for beginners exploring stock price prediction.

