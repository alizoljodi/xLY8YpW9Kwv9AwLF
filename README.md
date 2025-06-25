
# 📘 Value Investor

## Overview

**Value Investor** is a data-driven project designed to support long-term investment decisions in emerging markets using intelligent time series analysis and deep learning methods. The project combines financial domain knowledge with modern AI to assess asset performance and identify undervalued opportunities.

---

## Data Description

The project utilizes **stock market data from portfolio companies operating in emerging markets**, spanning the year **2020** and the **first quarter of 2021**. Each company’s stock data is provided in a separate sheet, reflecting real-world conditions such as **asynchronous market operating days** influenced by national holidays, time zones, and exchange-specific schedules.

- **Training Data**: 2020 stock prices  
- **Prediction Target**: Q1 2021 stock prices  

---

## Project Steps

### 🔍 1. Exploratory Data Analysis (EDA)
We begin with a comprehensive exploratory analysis to:
- Understand each company’s price and volume trends.
- Identify missing data and align timeframes across markets.
- Examine volatility, trends, and seasonality that align with long-term value behavior.

### 🧠 2. Multimodal Modeling
To enhance predictive performance, we tested **multimodal models** that integrate **stock price time series** with **financial news headlines**. These models attempt to capture market sentiment and macroeconomic events alongside traditional price movements. While promising in concept, they introduced added complexity and moderate noise due to the difficulty of aligning textual data with financial time steps.

### 📈 3. Time Series Modeling
We implemented and benchmarked a variety of time series forecasting models, including:

- **Classical statistical methods**: ARIMA, SARIMAX, ARIMAX  
- **Deep learning models**: LSTM, FCN, CNN  
- **State-of-the-art frameworks**:  
  - **TimesFM**, a foundation model trained on diverse temporal patterns  
  - **Chronos**, an industrial-grade time series forecasting toolkit  
  - **LLaMA2-8B**, adapted for sequence prediction through fine-tuning

Despite the sophistication of large-scale models, results showed that **simple LSTM networks** consistently delivered the best trade-off between accuracy, generalization, and interpretability across all companies.

---

## Objective

The ultimate goal of the **Value Investor** project is to develop a **robust, intelligent investment decision-support system** that:
- Leverages historical stock price behavior,
- Aligns with value investing principles,
- Integrates relevant external signals like news sentiment,
- And improves capital allocation decisions in volatile emerging markets.

By combining structured EDA, cross-modal experimentation, and comparative model analysis, the project reveals that **simplicity and domain alignment often outperform raw model complexity**. The result is a refined tool that empowers long-term investors with clear, data-driven signals.

---

## ✅ Conclusion

Through comprehensive analysis, modeling, and experimentation, this project underscores a key insight: **pragmatic, interpretable models like LSTM can outperform more complex and resource-intensive alternatives** in real-world financial settings, especially in emerging markets with noisy or inconsistent data.

While transformer-based models and multimodal approaches offer theoretical promise, their performance is often sensitive to preprocessing and fine-tuning, making them less suitable for smaller, less-structured datasets. Conversely, LSTM models provided robust forecasts with lower computational demands and more explainable outputs.

In summary, **Value Investor** successfully delivers a scalable, intelligent decision-support tool for long-term investment, reaffirming the power of simplicity when grounded in strong domain understanding and solid data practices.
