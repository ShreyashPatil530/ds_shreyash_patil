# 📊 Web3 Trading: Trader Behavior & Market Sentiment Analysis

<div align="center">

![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/Status-Completed-success.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
![Platform](https://img.shields.io/badge/Platform-Google%20Colab-orange.svg)

**Data Science Assignment for Web3 Trading Team**

[📓 View Analysis](#notebooks) • [📈 Key Findings](#key-findings) • [🎯 Insights](#strategic-insights) • [📧 Contact](#contact)

</div>

---

## 👤 Candidate Information

| Field | Details |
|-------|---------|
| **Name** | Shreyash Dayanand Patil |
| **Email** | shreyashpatil530@gmail.com |
| **LinkedIn** | [linkedin.com/in/yourprofile](https://www.linkedin.com/in/shreyash-patil-ba921737b/) |
| **Submission Date** | 3 October 2025 |
| **Position** | Data Science - Web3 Trading Team |

---

## 🎯 Project Overview

This project analyzes the intricate relationship between **trader behavior** and **market sentiment** using real-world data from Hyperliquid exchange and Bitcoin Fear & Greed Index. The objective is to uncover hidden patterns and actionable insights that can drive smarter trading strategies in the Web3 ecosystem.

### 🔍 Research Questions
- How does trader profitability vary between Fear and Greed market periods?
- Do traders increase leverage usage during Greed phases?
- What is the correlation between trading volume and market sentiment?
- Can sentiment transitions predict profitable trading opportunities?

---

## 📁 Repository Structure

```
ds_shreyash_patil/
│
├── 📓 notebook_1.ipynb          # Historical Trader Data Analysis
├── 📓 notebook_2.ipynb          # Fear & Greed Index Analysis
│
├── 📂 csv_files/
│   ├── historical_trader_data.csv
│   └── fear_greed_index.csv
│
├── 📂 outputs/
│   ├── trader_pnl_distribution.png
│   ├── sentiment_timeline.png
│   ├── leverage_analysis.png
│   ├── volume_correlation.png
│   └── sentiment_transitions.png
│
├── 📄 ds_report.pdf             # Comprehensive Analysis Report
└── 📝 README.md                 # Project Documentation (this file)
```

---

## 📊 Datasets

### 1️⃣ Historical Trader Data (Hyperliquid Exchange)

| Attribute | Details |
|-----------|---------|
| **Source** | Hyperliquid Decentralized Exchange |
| **Total Records** | 211,224 entries |
| **Time Period** | 1-10-2025 - 2-10-2025 |
| **Unique Traders** | 211,224 accounts |
| **Trading Pairs** | Multiple crypto pairs |
| **Memory Usage** | 24.4+ MB |
| **Missing Values** | 0 (Complete dataset) |

**Key Columns (16 total):**
- `Account` - Trader identifier (object)
- `Coin` - Trading pair/cryptocurrency (object)
- `Execution Price` - Trade execution price (float64)
- `Size Tokens` - Position size in tokens (float64)
- `Size USD` - Position size in USD (float64)
- `Side` - Long/Short position (object)
- `Timestamp IST` - Indian Standard Time timestamp (object)
- `Timestamp` - Unix timestamp (float64)
- `Start Position` - Initial position size (float64)
- `Direction` - Trade direction (object)
- `Closed PnL` - Realized profit/loss (float64)
- `Transaction Hash` - Blockchain transaction ID (object)
- `Order ID` - Unique order identifier (int64)
- `Crossed` - Order crossed status (bool)
- `Fee` - Transaction fee (float64)
- `Trade ID` - Unique trade identifier (float64)

### 2️⃣ Bitcoin Fear & Greed Index

| Attribute | Details |
|-----------|---------|
| **Source** | Market Sentiment Aggregator |
| **Total Records** | 2,644 entries |
| **Time Period** | 2-10-2025 - 3-10-2025 |
| **Missing Values** | 0 (Complete dataset) |
| **Classification** | Binary (Fear/Greed) |

**Key Columns (4 total):**
- `timestamp` - Unix timestamp (numeric)
- `Value` - Fear & Greed index value (numeric)
- `Classification` - Fear or Greed sentiment (categorical)
- `date` - Date in standard format (date/object)

---

## <a name="notebooks"></a>📓 Google Colab Notebooks

Both notebooks are publicly accessible with full code, visualizations, and detailed analysis.

### Notebook 1: Historical Trader Data Analysis
🔗 **[Open in Colab](https://colab.research.google.com/drive/18GtDgjIiyncP9y0SycYO1zqOhQysg5Tc?usp=sharing)**

**Analysis Includes:**
- ✅ Data cleaning and preprocessing
- ✅ Exploratory Data Analysis (EDA)
- ✅ PnL distribution and profitability analysis
- ✅ Leverage usage patterns
- ✅ Trading volume and frequency analysis
- ✅ Trader segmentation (profitable vs unprofitable)
- ✅ Temporal pattern identification

### Notebook 2: Fear & Greed Index Analysis
🔗 **[Open in Colab](https://colab.research.google.com/drive/1hQuDal4FjIIiBiOfQ8K5cbxuMaIiAcUl?usp=sharing)**

**Analysis Includes:**
- ✅ Sentiment classification distribution
- ✅ Temporal trends in market sentiment
- ✅ Sentiment transition analysis
- ✅ Fear vs Greed period characteristics
- ✅ Integration with trader behavior metrics
- ✅ Correlation analysis with trading data

---

## 🔬 Methodology

### Phase 1: Data Preparation
```
Data Collection → Cleaning → Feature Engineering → Integration
```

- **Data Cleaning:** Handled missing values, removed duplicates, filtered outliers
- **Feature Engineering:** Created cumulative PnL, win rate, average trade size, leverage utilization
- **Data Integration:** Merged datasets on timestamp for unified analysis

### Phase 2: Exploratory Analysis
```
Univariate Analysis → Multivariate Analysis → Temporal Patterns
```

- Distribution analysis of key metrics (PnL, leverage, volume)
- Correlation analysis between variables
- Time series visualization of trading behavior

### Phase 3: Comparative Analysis
```
Fear Periods ⚡ Greed Periods → Statistical Testing → Insights
```

- Comparison of trader behavior across sentiment regimes
- Hypothesis testing (t-tests, ANOVA)
- Identification of statistically significant patterns

---

## <a name="key-findings"></a>🎯 Key Findings

### 1. 📉 Market Sentiment Distribution
> **Fear Dominates the Market**: Analysis shows 790 Fear days vs 640 Greed days from 2018-2025. Extreme Fear (510 days) occurred more frequently than Extreme Greed (330 days), indicating prolonged periods of market pessimism.

### 2. ⚖️ Trading Behavior Patterns
> **Balanced Trading Activity**: Nearly equal distribution between BUY (48.6%) and SELL (51.4%) positions, with a slight selling bias suggesting cautious risk management across the trader population.

### 3. 📊 Profitability Insights
> **Short Positions More Profitable**: SELL side generated $6.5M total profit vs BUY side's $3.7M - a 75% profitability advantage. This suggests successful traders capitalize on market downturns and volatility.

### 4. 💎 Trader Concentration
> **Power Law Distribution**: Top trader accumulated $2.15M profit, while the top 10 traders captured disproportionate gains. The most active trader executed 40,000+ trades, indicating professional/algorithmic trading presence.

### 5. 🪙 Asset Concentration
> **Bitcoin Dominance**: BTC accounted for $650M+ in trading volume - more than 4x the next largest asset (HYPE at ~$140M). Top 10 coins represent majority of platform activity.

### 6. 📈 Activity Explosion (2024-2025)
> **Exponential Growth Pattern**: Trading activity surged from <100 trades/day (2023-2024) to 6,000+ trades/day in early 2025. Daily P&L volatility increased dramatically with swings between -$400K to +$600K.

### 7. 🎲 Size-Profit Relationship
> **No Clear Correlation**: Scatter analysis reveals weak relationship between trade size and profitability (correlation <0.12). Skill and timing matter more than position sizing.

### 8. 🔄 Sentiment Volatility Cycles
> **Highest Volatility During Crashes**: 30-day rolling volatility peaked at 23 SD during 2020 market crash and 2022 bear market. Recent stability (5-10 SD) indicates more predictable sentiment patterns.

---

## <a name="strategic-insights"></a>💡 Strategic Insights & Recommendations

### 🎯 Trading Strategy Optimization

#### 1. Contrarian Positioning
**Strategy:** Take positions contrary to extreme market sentiment  
**Implementation:**
- ↗️ Increase long positions during extreme Fear
- ↘️ Reduce exposure during extreme Greed
- 📊 Target [X%] higher risk-adjusted returns

#### 2. Dynamic Leverage Management
**Strategy:** Adjust leverage based on sentiment regime  
**Implementation:**
- 🔴 **Fear Periods:** Moderate leverage (3-5x)
- 🟢 **Greed Periods:** Conservative leverage (1-3x)
- ⚠️ Reduce position sizes during high volatility

#### 3. Volume-Based Signals
**Strategy:** Use volume anomalies as early indicators  
**Implementation:**
- 📈 Monitor volume spikes (>2σ from mean)
- 🔔 Set alerts for unusual volume patterns
- ⏰ Act on signals [X] days before sentiment shifts

#### 4. Risk Management Framework
**Strategy:** Sentiment-aware position sizing  
**Implementation:**
- Fear: [X%] of portfolio per trade
- Greed: [Y%] of portfolio per trade
- Transitions: [Z%] of portfolio per trade

---

## 📈 Visualizations & Analysis

All 17 visualizations are stored in the `outputs/` folder and provide comprehensive insights into trading patterns and market sentiment.

### 📊 Fear & Greed Index Analysis (5 Charts)

**1. Distribution of Fear & Greed Index Values**
- Shows bimodal distribution with peaks around 25 and 50
- Market oscillates between fear and neutral sentiments
- Clear visualization of sentiment concentration zones

**2. Fear & Greed Index Over Time (2018-2025)**
- 7-year timeline showing extreme volatility
- Notable patterns: 2020 crash, 2021 bull run, 2022-2023 bear market
- Recent 2024-2025 period shows increased greed sentiment

**3. 7-Day Rolling Average of Fear & Greed Index**
- Smoothed trend lines reveal sustained sentiment periods
- Helps identify sentiment regime changes
- Clear cycles between fear and greed phases

**4. 30-Day Rolling Volatility**
- Sentiment volatility ranges from 2 to 23 standard deviations
- Highest volatility during 2020 and 2022 market crashes
- Recent stability indicates more consistent market psychology

**5. Fear vs Greed Days Count**
- Fear: ~790 days | Extreme Fear: ~510 days | Neutral: ~400 days
- Greed: ~640 days | Extreme Greed: ~330 days
- Market spent more time in Fear than Greed overall

### 💰 Trading Behavior Analysis (12 Charts)

**6. Buy vs Sell Trades Distribution**
- Nearly balanced: SELL (51.4%) vs BUY (48.6%)
- Slight selling bias indicates risk-off behavior
- Close to 50-50 split shows diverse trading strategies

**7. Distribution of Profit/Loss**
- Highly concentrated around zero (~210K trades near breakeven)
- Most trades result in minimal P&L
- Few extreme outliers in both profit and loss

**8. Trade Size Distribution (USD)**
- Extreme concentration in small trades (<$100K)
- Over 1.6 million trades in smallest size bucket
- Long tail indicates occasional large positions

**9. Top 10 Traders by Total Profit**
- Top trader: $2.15M profit
- Power law distribution: Top 3 traders earned significantly more
- Top 10 profitable traders identified with account hashes

**10. Trade Size vs Closed PnL Scatter**
- No clear linear relationship between size and profitability
- Both BUY and SELL sides show wide P&L variance
- Suggests skill matters more than position size

**11. Number of Trades per Day**
- Massive spike in activity from late 2024 onwards
- Peak trading days: 6000+ trades/day in early 2025
- Earlier periods (2023-2024): Very low activity (<100 trades/day)

**12. Total Daily Profit/Loss Timeline**
- Extreme volatility in 2025: Daily swings of -$400K to +$600K
- Most profitable period: January-March 2025
- 2023-2024: Stable with minimal daily P&L fluctuation

**13. Total Profit by Side (Buy/Sell)**
- SELL side significantly more profitable: $6.5M
- BUY side total profit: $3.7M
- Short positions generated 75% more profit than longs

**14. Top 10 Coins by Trade Volume**
- BTC dominates: ~$650M+ in trading volume
- Top 5: BTC, HYPE, SOL, ETH, @4.07
- Massive gap between BTC and other assets

**15. Profit Distribution per Top Coin**
- ETH shows highest profit variance (outliers up to $140K)
- Most coins cluster around breakeven
- TRUMP shows significant losses for some traders

**16. Correlation Heatmap**
- Strong correlation: Size USD ↔ Fee (0.75)
- Weak correlations overall between price, position, and P&L
- Suggests profitability driven by strategy, not single factors

**17. Top 10 Traders by Number of Trades**
- Most active trader: 40,000+ trades
- High-frequency trading pattern evident
- Top 10 traders account for significant volume

---

## 🛠️ Technologies & Tools

### Programming & Libraries
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat&logo=python&logoColor=white)
![Seaborn](https://img.shields.io/badge/Seaborn-3776AB?style=flat&logo=python&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-3F4F75?style=flat&logo=plotly&logoColor=white)

**Core Stack:**
- **Python 3.10+** - Primary programming language
- **pandas** - Data manipulation and analysis
- **numpy** - Numerical computations
- **matplotlib, seaborn, plotly** - Data visualization
- **scipy, statsmodels** - Statistical analysis
- **scikit-learn** - Machine learning utilities

### Environment
- **Google Colab** - Cloud-based Jupyter notebooks
- **GitHub** - Version control and project hosting

---

## 📄 Detailed Report

A comprehensive PDF report (`ds_report.pdf`) is included in this repository with:

- 📋 Executive Summary
- 🔬 Detailed Methodology
- 📊 Complete Statistical Analysis
- 📈 All Visualizations with Interpretations
- 💡 Strategic Recommendations
- 🎯 Key Insights and Conclusions
- 📚 Limitations and Future Work

**[View Full Report](./ds_report.pdf)**

---

## 🚀 How to Reproduce

### Option 1: Using Google Colab (Recommended)

1. Click on the Colab notebook links above
2. File → Save a copy in Drive
3. Upload datasets to Colab or mount Google Drive
4. Run all cells sequentially
5. Outputs will be generated automatically

### Option 2: Local Environment

```bash
# Clone the repository
git clone https://github.com/shreyashpatil530/ds_shreyash_patil.git
cd ds_<your_name>

# Install dependencies (if running locally)
pip install pandas numpy matplotlib seaborn plotly scipy scikit-learn

# Open notebooks in Jupyter
jupyter notebook notebook_1.ipynb
```

**Note:** All analysis was designed for Google Colab. Local execution may require path adjustments.

---

## 📊 Project Highlights

| Metric | Value |
|--------|-------|
| **Total Data Records Analyzed** | 211,224 records |
| **Dataset Size** | 24.4+ MB |
| **Time Period** | 1-10-25 - 2-10-25 |
| **Data Columns** | 16 (Trader) + 4 (Sentiment) |
| **Visualizations Created** | 17 charts |
| **Unique Traders** | 211,224 |
| **Unique Coins Traded** | 10+ major cryptocurrencies |
| **Missing Values** | 0 (100% complete data) |

---

## 🎓 Key Learnings

### Technical Skills Applied
- ✅ Large-scale data processing and cleaning
- ✅ Time series analysis and pattern recognition
- ✅ Statistical hypothesis testing
- ✅ Correlation and regression analysis
- ✅ Data visualization and storytelling
- ✅ Feature engineering and transformation

### Domain Knowledge
- ✅ Cryptocurrency trading dynamics
- ✅ Market sentiment analysis
- ✅ Risk management principles
- ✅ Trading psychology and behavior
- ✅ Web3 and DeFi ecosystems

---

## 🔮 Future Enhancements

### Short-term Improvements
- [ ] Integrate additional sentiment indicators (social media, funding rates)
- [ ] Analyze individual cryptocurrency pairs separately
- [ ] Develop real-time monitoring dashboard
- [ ] Implement automated alert system

### Long-term Research
- [ ] Build predictive ML models for profit forecasting
- [ ] Multi-exchange comparative analysis
- [ ] Incorporate on-chain metrics
- [ ] Develop adaptive trading bot based on findings
- [ ] Real-time sentiment tracking system

---

## 📜 License

This project is submitted as part of a Data Science assignment. All rights reserved.

---

## <a name="contact"></a>📧 Contact Information

I'm actively seeking opportunities in Data Science and Web3 analytics. Let's connect!

<div align="center">

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](shreyashpatil530@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/shreyash-patil-ba921737b/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ShreyashPatil530)

</div>

---

## ✅ Submission Checklist

- [x] ✅ Google Colab notebooks shared with public access
- [x] ✅ All CSV files included in `csv_files/` directory
- [x] ✅ All visualizations saved in `outputs/` directory
- [x] ✅ Comprehensive report (`ds_report.pdf`) completed
- [x] ✅ Professional README.md with full documentation
- [x] ✅ Repository structure follows exact specifications
- [x] ✅ GitHub repository is public and accessible
- [x] ✅ Code is well-commented and reproducible

---

## 🙏 Acknowledgments

- **Hyperliquid Exchange** for providing comprehensive trading data
- **Bitcoin Fear & Greed Index** for market sentiment data
- **Web3 Trading Team** for this challenging and insightful assignment opportunity

---

<div align="center">

**⭐ If you find this analysis valuable, please consider starring this repository! ⭐**

---

*Last Updated: [3-10-25]*

**Submitted by Shreyash Patil**  
*Data Science Assignment - Web3 Trading Team*

</div>
