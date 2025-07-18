# Healthcare Claims Cost Forecasting with Meta Prophet
## 📋 Project Overview
This notebook demonstrates the use of Meta Prophet, a robust time series forecasting library developed by Meta (formerly Facebook), to model and forecast synthetic healthcare claims cost data. The dataset simulates realistic cost behavior such as:

📈 Long-term upward trends

🌦 Seasonal patterns (e.g. flu season spikes in winter months)

🎄 Holiday effects (e.g. increased or decreased cost around December)

📉 Random noise to emulate real-world unpredictability

Prophet is ideal for this use case due to its ability to handle:

  1. Additive and multiplicative seasonality

  2. Missing data

  3. Outliers

  4. Seasonaity and Holiday effects

## 🔢 Dataset Description
Two columns
  1. ds	Timestamp in YYYY-MM-DD format (monthly granularity)
  2. y	Total healthcare claims cost in dollars

The dataset spans 5+ years of monthly data and includes typical seasonal and trend characteristics found in the U.S. healthcare system.

