## Crypto Trading Analysis: Fear & Greed Index vs Trading Performance

## 📊 Project Overview
This project analyzes the relationship between cryptocurrency market sentiment (Fear & Greed Index) and trading performance metrics. The analysis examines how different market sentiment conditions (Extreme Fear, Fear, Neutral, Greed, Extreme Greed) impact trading profitability, win rates, and risk metrics.

## 📁 Dataset Description

### Data Sources
1. **Trader Historical Data** (`historical_data.csv`)
   - Trading execution details
   - Profit/Loss metrics
   - Trade timing and sizing
   - Transaction metadata

2. **Fear & Greed Index** (`fear_greed_index.csv`)
   - Daily market sentiment scores (0-100)
   - Sentiment classifications:
     - Extreme Fear (0-24)
     - Fear (25-49)
     - Neutral (50-74)
     - Greed (75-94)
     - Extreme Greed (95-100)

### Key Features
- **211,224 trades** analyzed
- **Date range**: Multiple trading periods
- **Market conditions**: Various sentiment environments

## 🔍 Analysis Performed

### 1. Data Preprocessing
- Date format standardization
- Data merging and cleaning
- Missing value handling

### 2. Core Analysis
- **Profit Analysis**: Average PnL by sentiment category
- **Win Rate Analysis**: Success rates across market conditions
- **Risk Assessment**: Standard deviation of returns
- **Risk-Return Ratios**: Efficiency metrics

### 3. Key Findings

#### Market Sentiment Distribution
```
Extreme Fear:     21,400 trades (10.1%)
Fear:             61,837 trades (29.3%)
Neutral:          37,686 trades (17.8%)
Greed:            50,303 trades (23.8%)
Extreme Greed:    39,992 trades (18.9%)
```

#### Performance Metrics by Sentiment

| Sentiment      | Avg Profit | Win Rate | Risk (Std) | Risk-Return Ratio |
|----------------|------------|----------|------------|-------------------|
| Extreme Fear   | $35        | 37.1%    | $1,136     | 0.03              |
| Fear           | $54        | 42.1%    | $935       | 0.06              |
| Neutral        | $34        | 39.7%    | $517       | 0.07              |
| Greed          | $43        | 38.5%    | $1,116     | 0.04              |
| Extreme Greed  | $68        | 46.5%    | $767       | 0.09              |

## 📈 Key Insights

### 🎯 Best Performing Conditions
- **Extreme Greed**: Highest average profit ($68) and best win rate (46.5%)
- **Optimal Risk-Return**: Extreme Greed shows best efficiency (0.09 ratio)

### ⚠️ Risk Observations
- **Extreme Fear**: Lowest win rate (37.1%) and poorest risk-return ratio
- **Greed Periods**: Highest volatility but decent returns
- **Neutral Markets**: Lowest risk but moderate returns

### 📊 Trading Strategy Implications
1. **Bullish Signals**: Extreme Greed periods offer best profit opportunities
2. **Risk Management**: Extreme Fear conditions require caution
3. **Consistent Performance**: Neutral markets provide stable, low-risk environment

## 🛠 Technical Implementation

### Libraries Used
- `pandas` - Data manipulation and analysis
- `numpy` - Numerical computations
- `matplotlib` & `seaborn` - Data visualization
- `scikit-learn` - Statistical analysis

### Analysis Features
- Correlation analysis between sentiment and PnL
- Statistical aggregation by sentiment categories
- Risk-adjusted performance metrics
- Multi-panel visualization of key findings

## 📊 Visualizations
The project includes comprehensive visualizations showing:
- Average profit distribution across sentiment categories
- Win rate comparisons
- Risk metrics (standard deviation)
- Risk-return efficiency ratios

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn
```

### Running the Analysis
1. Place your CSV files in the project directory
2. Update file paths in the notebook
3. Execute cells sequentially for full analysis

## 📈 Business Applications
- **Trading Strategy Development**: Optimize entry/exit timing based on market sentiment
- **Risk Management**: Adjust position sizing according to sentiment-driven volatility
- **Performance Monitoring**: Track strategy effectiveness across market conditions
- **Sentiment-Based Hedging**: Develop counter-cyclical trading approaches

## 🔮 Future Enhancements
- Real-time sentiment integration
- Machine learning models for predictive analytics
- Multi-asset class analysis
- Advanced risk modeling techniques
