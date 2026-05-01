# 📊 AI Trading Strategy using Market Sentiment

## 🔍 Objective

The goal of this project is to analyze the relationship between trader performance and market sentiment (Fear & Greed Index) and build an AI-driven trading strategy that improves profitability using machine learning and quantitative techniques.

---

## 📁 Datasets Used

1. **Historical Trader Data**
   - Includes trade-level details such as price, size, side, PnL, timestamp

2. **Bitcoin Fear & Greed Index**
   - Daily sentiment classification (Fear, Greed, Extreme Fear, etc.)

---

## ⚙️ Approach

### 1. Data Preprocessing
- Cleaned and standardized column names
- Converted timestamps into datetime format
- Extracted date for merging datasets

### 2. Data Integration
- Merged trade data with sentiment data on date
- Handled missing sentiment values using forward fill

### 3. Feature Engineering
- Encoded categorical variables (Side, Sentiment)
- Created time-based features (hour, day of week)
- Built rolling features:
  - Rolling sentiment average
  - Price volatility
  - Trade intensity
- Generated profit classification label

---

## 🤖 Models Used

### 1. Regression Model
- **Random Forest Regressor**
- Predicts trade-level PnL

### 2. Classification Model
- **Gradient Boosting Classifier**
- Predicts probability of profitable trade

---

## 📈 Trading Strategy

An AI-based trading signal is generated using:

- Predicted PnL (from ML model)
- Market sentiment conditions

### Signal Logic:
- **BUY** → Positive predicted PnL + Greed sentiment
- **SELL** → Negative predicted PnL + Fear sentiment
- **HOLD** → Otherwise

---

## 🔄 Backtesting

- Simulated strategy returns based on generated signals
- Compared against raw trading performance
- Calculated cumulative returns

---

## 📊 Results

### Key Findings:

- Market sentiment significantly impacts trading outcomes
- Rolling sentiment improves prediction accuracy
- Time-based features (hour/day) influence profitability
- ML models can predict PnL with reasonable performance

### Strategy Performance:

- AI-based strategy outperformed raw trading
- Improved cumulative returns
- Better risk-adjusted performance

### Risk Metric:

- **Sharpe Ratio** used to evaluate strategy stability

---

## 💡 Conclusion

This project demonstrates how combining:

- Market sentiment  
- Trade-level data  
- Machine learning  

can lead to a more intelligent and adaptive trading strategy.

---

## 🚀 Future Improvements

- LSTM / Time-series modeling
- Real-time trading system
- Portfolio optimization
- Reinforcement learning-based trading agent

---

## 👨‍💻 Author

**Saafin Hasan**  
B.Tech CSE (AI & ML)  
Aspiring AI Engineer & Quant Developer
