# Intelligent System for Inventory Demand Forecasting

This repository contains code, models, and documentation for a project that builds an intelligent demand forecasting system for inventory management. The system is designed to support dining hall operations at Indiana University by minimizing food waste and improving stock prediction accuracy.

## 🚀 Project Objective

Develop an AI-powered inventory management tool to:
- Predict inventory needs using time series models
- Enhance operational efficiency
- Reduce overstocking and food waste
- Enable real-time inventory insights via a Large Language Model (LLM)

## 📊 Key Features

- **Time Series Forecasting Models:** ARIMA, Holt-Winters, and Multilayer Perceptron (MLP)
- **Advanced Preprocessing:** StandardScaler, Label Encoding, IQR-based outlier detection, and cyclic month encoding
- **Feature Engineering:** Aggregated demand statistics, lag features
- **LLM Integration:** Interactive Q&A for inventory insights using a locally-hosted LLaMA model
- **Visualization Tools:** Word clouds, correlation heatmaps, time-series trend plots

## 🧪 Methodology

1. **Data Cleaning & EDA**
   - Missing value handling
   - Outlier detection (IQR method)
   - Word cloud and temporal trend analysis

2. **Feature Engineering**
   - Demand scaling with StandardScaler
   - Cyclic encoding for time variables (Month)
   - Aggregated statistics (mean, median)

3. **Model Training**
   - **Holt-Winters** for additive trend and seasonality
   - **SARIMA** for auto-regressive seasonal forecasting
   - **MLP Regressor** for capturing non-linear patterns (best performance)

4. **LLM Component**
   - LLaMA model via Ollama for intelligent querying
   - Context-aware prompt-response for inventory queries

## 📈 Results

- **MLP outperformed** ARIMA and Holt-Winters with RMSE = 6.52
- Forecasting results show stable and accurate 12-month demand prediction for top products
- LLM component provided intuitive responses to user queries about historical and predicted inventory
