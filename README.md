# Master--Thesis
Project on forecasting commodity prices using sentiment from geopolitical news. Used FinBERT for sentiment analysis, XGBoost and Random Forest for classification, and LSTM for time-series forecasting. Achieved 76% accuracy, insights useful for trading, risk, and policy decision-making.
# Geopolitical Sentiment Analysis & Commodity Price Prediction

## Overview
This master thesis explores how geopolitical events influence commodity prices using sentiment analysis and machine learning. We focus on four major commodities—crude oil, gold, wheat, and natural gas—evaluating both the direction and magnitude of price changes following global news events.

## Objectives
- Analyze the impact of geopolitical news on commodity price volatility.
- Use NLP to extract sentiment from news headlines using FinBERT.
- Predict short-term price direction using XGBoost and Random Forest.
- Forecast price magnitude using LSTM time-series models.
- Make model outputs explainable using SHAP.

## Tools & Technologies
- **FinBERT** (HuggingFace)
- **XGBoost**, **Random Forest**
- **LSTM** (Keras/TensorFlow)
- **SHAP** for interpretability
- **Python**, **Pandas**, **scikit-learn**, **Matplotlib**
- **GNews API**, **Yahoo Finance API** (for real-time data)

## Dataset
- 1,246 news headline–price pairs from Jan 2021 to Apr 2025
- ETFs used as commodity proxies: USO (Oil), GLD (Gold), WEAT (Wheat), UNG (Gas)
- Event windows: ±3 days to match price movement with sentiment

## Key Findings
- Negative geopolitical sentiment strongly correlates with gold and oil price surges.
- **XGBoost** outperformed other classifiers with **76% accuracy** and **0.81 ROC-AUC**.
- **LSTM** model achieved an **RMSE of 1.2%** in forecasting price magnitudes for oil and gold.
- **SHAP analysis** revealed that sentiment, time, and commodity type are key prediction drivers.

## Limitations
- Small dataset size for deep learning (LSTM)
- ETF prices may not fully reflect spot market behavior
- Sentiment models limited by sarcasm/figurative language

## Future Work
- Multilingual sentiment models for global coverage
- Larger dataset across longer time horizons
- Incorporate macroeconomic indicators and event-specific variables

## Authors
- **Madhuri Panchumarti**
- **Hardik Sethi**

## Advisor
- Prof. Sachin Kamble – EDHEC Business School

This project bridges NLP, behavioral finance, and machine learning to deliver real-time, interpretable forecasts for politically sensitive commodities.

