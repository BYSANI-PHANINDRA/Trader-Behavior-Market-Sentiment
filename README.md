Trader Behavior vs Market Sentiment Analysis
Objective

The objective of this project is to analyze how Bitcoin market sentiment influences trader behavior and performance. By combining historical trader data with the Fear & Greed Index, the analysis aims to identify behavioral patterns that can help inform smarter and more disciplined trading strategies.

Datasets Used
1. Bitcoin Fear & Greed Index

Daily sentiment classification: Fear, Greed, and Neutral

Represents overall market psychology on each trading day

2. Hyperliquid Historical Trader Data

Trade-level data including:

Trader account

Trade execution details

Realized (closed) PnL

Trade timestamps

Methodology

Loaded and inspected raw datasets to understand schema inconsistencies

Normalized timestamps to daily granularity for accurate alignment

Merged trader data with sentiment data using trading date

Removed zero-PnL trades to eliminate non-closing or system-generated events

Created performance metrics:

Total PnL

Average PnL per trade

Win rate

Trade count

Aggregated results at both trader and sentiment levels

Visualized and interpreted behavioral patterns across sentiment regimes

Key Results Summary
Market Sentiment	Total PnL	Avg PnL per Trade	Win Rate	Trade Count
Fear	~1.78M	~253	~0.85	~7,038
Greed	~1.77M	~192	~0.87	~9,220
Neutral	~0.07M	~45	~0.82	~1,671
Key Insights

Greed periods show the highest trading activity, indicating aggressive participation and increased risk-taking behavior.

Despite higher activity during Greed, average PnL per trade is lower, suggesting overtrading reduces trade quality.

Fear periods have fewer trades but higher average PnL, indicating more disciplined and selective trading behavior.

Win rates remain relatively stable across sentiments, showing that higher trade frequency does not necessarily improve success rates.

Neutral sentiment periods show low participation and weak profitability, reflecting reduced conviction among traders.

Actionable Implications

Market sentiment can be used as a risk-adjustment signal rather than a directional indicator.

During Greed phases:

Reduce trade frequency

Avoid excessive risk exposure

During Fear phases:

Focus on high-conviction setups

Maintain disciplined position sizing

Incorporating sentiment awareness can help traders avoid emotionally driven decisions.

Conclusion

The analysis demonstrates that market sentiment has a measurable impact on trader behavior. Greed-driven markets encourage higher activity but lower trade efficiency, while Fear-driven markets promote caution and better average returns. These findings highlight the importance of sentiment-aware strategies in crypto trading environments.

Tools & Technologies

Python

Pandas, NumPy

Matplotlib, Seaborn

Google Colab

Author

B. Phanindra Kumar
B.Tech CSE (AI & ML), Jain University
