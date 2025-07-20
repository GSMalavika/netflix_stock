# netflix_stock
Data analysis of netflix stock price that ranges from 2002 to 2025
# 📈 Netflix Stock Analysis (2002–2025)

This project analyzes Netflix (NFLX) stock data from 2002 to 2025 using Python in Google Colab. The analysis includes technical indicators like Bollinger Bands, RSI, and EMA, along with buy/sell signal generation based on strategy rules.

## 🧰 Tools & Libraries

- Python (Google Colab)
- pandas
- numpy
- matplotlib / seaborn
- plotly graph objects

## 📊 Key Features
- 📈 Bollinger Bands visualization
- 🔁 RSI and EMA crossover-based buy/sell signal generation
- 📉 Trend and volatility analysis
- 🧠 Signal-based strategy logic
- 💾 CSV export of cleaned data with signals
## 📌 Strategy Used

**Buy Signal:**
- Close < Lower Bollinger Band  
- RSI < 30 (oversold)  
- EMA20 > EMA50 (bullish crossover)

**Sell Signal:**
- Close > Upper Bollinger Band  
- RSI > 70 (overbought)  
- EMA20 < EMA50 (bearish crossover)

Signals are stored in a `signal` column (1 for buy, -1 for sell).
## 📁 Project Structure

```bash
├── Netflix_Stock_Analysis.ipynb  # Main notebook
├── data/                         # Optional: Raw and processed CSVs
├── plots/                        # Saved plot images (optional)
└── README.md
