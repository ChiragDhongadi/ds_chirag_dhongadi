# 📊 Trader Behavior Insights: Market Sentiment vs Trader Performance

## 🚀 Project Overview
This project explores the relationship between **Bitcoin market sentiment (Fear & Greed Index)** and **trader behavior/performance** on the Hyperliquid trading platform.  
By combining historical trader data with daily sentiment classifications, the analysis uncovers patterns in profitability, trading bias, and risk behavior across different market regimes.

The goal is to derive **actionable insights** that can help design smarter, sentiment-aware trading strategies.

---

## 🎯 Objectives
- Analyze how market sentiment influences:
  - Trader profitability
  - Buy vs sell behavior
  - Risk and volatility
- Identify whether extreme sentiment regimes lead to better or worse trading outcomes
- Provide data-driven insights relevant to Web3 and crypto trading environments

---

## 📂 Datasets Used

### 1️⃣ Bitcoin Market Sentiment Dataset (Fear & Greed Index)
**Columns**
- `date`
- `classification` (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

### 2️⃣ Historical Trader Data 
**Key Columns**
- `Account`
- `Side` (BUY / SELL)
- `Execution Price`
- `Size USD`
- `Closed PnL`
- `Timestamp`
- `Leverage`
- Other trade metadata

---

## 🧪 Methodology

1. **Data Cleaning & Preprocessing**
   - Converted timestamps to daily granularity
   - Standardized date formats across datasets
   - Handled missing values and inconsistencies

2. **Feature Engineering**
   - `Profit_Rate`: Profitable trades / Total trades per day
   - `Buy_Ratio`: Proportion of buy trades per day
   - `Avg_PnL`: Average profit/loss per trade per day
   - Binary encoding for trade direction (Buy/Sell)

3. **Data Aggregation**
   - Aggregated data at **account-day level**
   - Merged trader data with sentiment classification by date

4. **Exploratory Data Analysis (EDA)**
   - Used boxplots to compare distributions across sentiment regimes
   - Focused on variability, medians, and outliers

---

## 📈 Key Visualizations

### 1️⃣ Daily Profit Rate vs Market Sentiment
- Shows how consistently traders are profitable under different sentiment conditions

### 2️⃣ Buy Ratio per Day vs Market Sentiment
- Captures directional bias (buy-heavy vs balanced trading)

### 3️⃣ Average PnL per Day vs Market Sentiment
- Highlights volatility and extreme profit/loss events

---

## 🔍 Key Insights

### 📌 Profitability
- Profit rates are broadly similar across sentiment regimes
- **Extreme Greed** shows slightly higher median profit rates
- Market sentiment alone is not a reliable predictor of consistent profitability

### 📌 Trader Behavior
- Buy ratios remain close to 0.5 across all regimes
- Traders maintain balanced exposure even during extreme sentiment
- Indicates disciplined, strategy-driven behavior rather than emotional trading

### 📌 Risk & Volatility
- Extreme Fear and Extreme Greed show higher dispersion in PnL
- Large gains and losses cluster in high-emotion market phases
- Sentiment impacts **risk more than returns**

---

## 🧠 Conclusions
- Market sentiment acts as a **volatility amplifier**, not a profit guarantee
- Successful trading depends more on:
  - Execution quality
  - Risk management
  - Strategy discipline
- Sentiment should be used as **context**, not a standalone signal

---

## 💡 Practical Implications
- Avoid sentiment-only trading strategies
- Apply stronger risk controls during extreme sentiment phases
- Combine sentiment with price action, volume, and volatility indicators
- Extreme sentiment environments may suit experienced traders more than beginners

---

## 🔮 Future Scope
- Segment traders by experience or capital size
- Analyze leverage-adjusted returns
- Incorporate volatility and liquidity metrics
- Build predictive models combining sentiment + market data

---

## 🛠 Tech Stack
- **Python**
- **Pandas, NumPy**
- **Matplotlib, Seaborn**
- **Jupyter Notebook / Google Colab**

---

## 👤 Author
**Chirag Dhongadi**  
Aspiring Data Scientist | Web3 & Trading Analytics  
- GitHub: [[Your GitHub Link](https://github.com/ChiragDhongadi)]
- LinkedIn: [[Your LinkedIn Link](https://www.linkedin.com/in/chirag-dhongadi/)]

---

## ✅ Final Note
This project demonstrates how **data-driven analysis** can uncover meaningful insights in crypto trading environments, emphasizing the importance of disciplined strategies over sentiment-driven decisions.
