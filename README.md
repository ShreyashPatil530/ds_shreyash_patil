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
| **Name** | [Your Full Name] |
| **Email** | [your.email@example.com] |
| **LinkedIn** | [linkedin.com/in/yourprofile](https://linkedin.com/in/yourprofile) |
| **Submission Date** | [October 2024] |
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
ds_<your_name>/
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
| **Time Period** | [Start Date] - [End Date] |
| **Unique Traders** | [XXX accounts] |
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
| **Total Records** | [XXX entries] |
| **Time Period** | [Start Date] - [End Date] |
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
🔗 **[Open in Colab](YOUR_COLAB_LINK_1_HERE)**

**Analysis Includes:**
- ✅ Data cleaning and preprocessing
- ✅ Exploratory Data Analysis (EDA)
- ✅ PnL distribution and profitability analysis
- ✅ Leverage usage patterns
- ✅ Trading volume and frequency analysis
- ✅ Trader segmentation (profitable vs unprofitable)
- ✅ Temporal pattern identification

### Notebook 2: Fear & Greed Index Analysis
🔗 **[Open in Colab](YOUR_COLAB_LINK_2_HERE)**

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

### 1. 📉 Profitability Patterns
> **[Insert your finding]**  
> Example: "Traders achieved 18% higher average returns during Fear periods compared to Greed periods (p < 0.05), suggesting contrarian opportunities."

### 2. ⚖️ Leverage Behavior
> **[Insert your finding]**  
> Example: "Average leverage usage increased by 23% during Greed phases, correlating with a 31% increase in loss probability."

### 3. 📊 Volume Dynamics
> **[Insert your finding]**  
> Example: "Trading volume spiked by 45% within 2 days before sentiment transitions, serving as a potential predictive signal."

### 4. 🔄 Sentiment Transitions
> **[Insert your finding]**  
> Example: "The 3-day window following Fear→Greed transitions showed 27% higher trading opportunities with improved risk-reward ratios."

### 5. 👥 Trader Segmentation
> **[Insert your finding]**  
> Example: "Top 20% of profitable traders exhibited consistent contrarian positioning and maintained leverage below 5x regardless of sentiment."

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

## 📈 Visualizations

All visualizations are stored in the `outputs/` folder and referenced in the notebooks and report.

### Sample Insights from Visualizations:

1. **PnL Distribution by Sentiment**
   - Clear performance differences across market regimes
   - [Add specific insight from your chart]

2. **Leverage Usage Over Time**
   - Correlation between leverage and sentiment phases
   - [Add specific insight from your chart]

3. **Volume vs Sentiment Timeline**
   - Volume spikes preceding sentiment changes
   - [Add specific insight from your chart]

4. **Correlation Heatmap**
   - Key relationships between variables
   - [Add specific insight from your chart]

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
git clone https://github.com/yourusername/ds_<your_name>.git
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
| **Total Data Records Analyzed** | 211,224+ records |
| **Dataset Size** | 24.4+ MB |
| **Data Columns** | 16 (Trader) + 4 (Sentiment) |
| **Visualizations Created** | [XX charts] |
| **Statistical Tests Performed** | [XX tests] |
| **Analysis Duration** | [X weeks] |
| **Report Pages** | [XX pages] |
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

[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:your.email@example.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/yourprofile)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yourusername)

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

*Last Updated: [Current Date]*

**Submitted by [Your Name]**  
*Data Science Assignment - Web3 Trading Team*

</div>
