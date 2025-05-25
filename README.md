# 📈 Macro Event-Based Stock Market Prediction

This project analyzes the impact of macroeconomic events and social sentiment on stock market behavior—specifically Dow Jones closing prices. It combines sentiment analysis on Reddit posts with economic indicators (inflation, natural disasters, pandemics, and seasonality) to predict market movements using both classification and regression techniques.

## 🚀 Project Overview

We developed a two-phase machine learning pipeline:
1. **Sentiment Classification** – Determines the sentiment impact of Reddit posts on market movement.
2. **Stock Price Regression** – Predicts actual market changes using LSTM-based time series modeling.

## 🧠 Key Features

- **Multimodal Inputs**: Combines textual Reddit sentiment with structured macroeconomic data.
- **Classification Models**: Voting Classifier ensemble of XGBoost, Random Forest, and SGD.
- **Regression Model**: LSTM-based neural network using TensorFlow.
- **Web Integration**: Angular-based front-end to visualize predictions and model outputs.

## 🗃️ Datasets Used

### Sentiment Analysis
- Source: Daily top 25 ‘hot’ Reddit posts
- Labels: Binary (0 = price drop, 1 = price rise or same)
- Preprocessing: Tokenization, sentiment scoring, and feature extraction

### Regression Features
- **Reddit Sentiment**: Output from Phase 1
- **Natural Calamities**: Wildfires, hurricanes, floods, tornadoes, etc.
- **Pandemic Impact**: COVID-related indicators
- **Inflation Rate (US)**: Annual percentage
- **Seasonal Trends**: Encoded quarterly indicators

## 🛠️ Tech Stack

| Component         | Stack/Library                         |
|------------------|---------------------------------------|
| Language          | Python, TypeScript                    |
| ML Libraries      | XGBoost, Random Forest, SGD, TensorFlow |
| Deep Learning     | TensorFlow Sequential + LSTM         |
| Frontend          | Angular 8, HTML, CSS                  |
| Visualization     | Matplotlib, Seaborn                   |

## 📊 Results

- **Voting Classifier** improved prediction over individual estimators for sentiment classification.
- **LSTM Regression** effectively captured temporal dependencies, outperforming linear models for time series prediction.
- Visual comparison of predicted vs. actual Dow Jones values revealed high correlation on major events.

