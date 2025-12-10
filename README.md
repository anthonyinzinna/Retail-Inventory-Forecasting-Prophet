# Retail-Inventory-Forecasting-Prophet

Supply Chain Optimization: Retail Demand Forecasting & Inventory Planning

Objective: To optimize Q1 2025 inventory procurement for a retail operation by generating a precise 90-day demand forecast, minimizing the financial risks of both stockouts (lost revenue) and overstocking (holding costs).

Overview: This project applies advanced time-series modeling to historical sales data to solve a critical supply chain challenge: determining the optimal purchasing quantity for an upcoming quarter. By leveraging Facebook Prophet, the analysis decomposes sales patterns into trend, weekly, and yearly seasonality to isolate core demand drivers. The model goes beyond simple point forecasting by calculating dynamic "Safety Stock" levels using confidence intervals, ensuring the final purchasing recommendation accounts for demand volatility and supply chain uncertainty.

Methodology: • Data Preprocessing: Aggregated daily transaction data and handled missing date ranges to ensure a continuous time series for Prophet modeling. • Decomposition & Modeling: Trained a Prophet additive model to separate the underlying growth trend from seasonal fluctuations (weekly sales spikes and yearly holiday cycles). • Safety Stock Calculation: Instead of relying on standard averages, the model utilized the 95% confidence interval upper bound to quantify risk and calculate the necessary safety buffer. • Strategic Planning: Converted raw model outputs into a concrete purchasing recommendation, comparing the "Base Demand" against the "Risk-Adjusted Demand."

Findings: • Q1 2025 Demand Forecast: The model predicts a total baseline demand of 15,079 units for the upcoming 90-day period. • Seasonality Drivers: Identified strong weekly cyclicality with peak demand occurring on weekends, necessitating higher stock levels end-of-week. • Risk Assessment: Volatility analysis indicated a need for a 5.9% inventory buffer (895 units) to maintain a 95% service level during peak variance. • Final Purchasing Recommendation: Recommended a total procurement order of 15,974 units to satisfy demand while protecting against unforeseen spikes.

Recommendations: • Execute Q1 Purchase: Place immediate order for 15,974 units to align with the forecasted start of the quarter. • Dynamic Replenishment: Shift from static monthly ordering to a flexible weekly schedule that aligns with the identified weekend demand surges. • Monitor Variance: Track actuals vs. forecast for the first 30 days; if variance exceeds the 5.9% buffer, recalibrate the safety stock model.

Impact: This project bridges the gap between Data Science and Operations Management. It demonstrates how predictive modeling can directly influence financial decision-making, transforming raw sales data into an actionable procurement strategy that protects revenue and optimizes working capital.

Tools Used: Python (Facebook Prophet, Pandas, Matplotlib, Seaborn), Time Series Analysis, Inventory Management Theory, Jupyter Notebooks.
