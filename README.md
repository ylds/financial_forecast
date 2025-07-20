# Revenue Forecasting with Meta Prophet
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
Key columns
  1. ds	Timestamp in YYYY-MM-DD format (daily granularity)
  2. y	revenue


**fig 1.**  Overview of the data, I used the first 3.5 years train the prophet model, forecasting the last 1 year.
<img width="905" height="432" alt="image" src="https://github.com/user-attachments/assets/759a7eef-438e-4ad1-8167-2b6afb8ef035" />



**fig 2.** The Prophet model captures multiple components to improve forecast accuracy:

    Trend: Models long-term growth or decline in the data.

    Seasonality: Accounts for recurring patterns, including weekly and yearly cycles.

    Holidays: Incorporates the effects of known holidays, which often cause irregularities in time series data.

<img width="543" height="718" alt="image" src="https://github.com/user-attachments/assets/63a3a62e-fdaa-4595-84fb-486945d9d0a5" />

## 📈 Forecast Summary Using Prophet
**Performance:**

    RMSE: 110,920.79
    
    RMSE as % of Mean Actual: 13.25%

⚠️ Initially, U.S. holidays were used, which led to worse results. Switching to Ecuador-specific holidays improved performance noticeably.

**Insights:**

The model successfully captured growth trends and seasonality.

Including local holidays had a measurable impact on forecast accuracy.

Error remains moderate, adding oil price might help improve the model because Educador economy is heavily depending on the oil price.

<img width="1105" height="397" alt="image" src="https://github.com/user-attachments/assets/667b8b78-6687-449c-97bc-fae2b3273ce7" />

