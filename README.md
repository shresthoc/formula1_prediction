# 🏎️ F1 Race Outcome Predictor – 2025 Season

This repository contains Python scripts to **predict the outcome of Formula 1 races** using real-world data and machine learning models. The system leverages [FastF1](https://theoehrly.github.io/Fast-F1/) for race telemetry, [OpenWeatherMap](https://openweathermap.org/api) for weather data, and scikit-learn for training regression models that estimate driver race performance.

## 💡 Project Overview

For each Grand Prix in the 2025 F1 season, this project:
- Gathers sector-wise lap timing data using FastF1
- Integrates clean air race pace and qualifying performance
- Retrieves weather forecasts for the race location
- Factors in team performance and historical driver trends
- Trains a machine learning model to **predict race times**
- Outputs predicted podium finishers with performance plots

## 🔍 Key Features
- **FastF1 Integration**: Access to official session telemetry and lap data
- **Clean Air Race Pace Modeling**: Uses historical stint data to approximate performance without traffic
- **Qualifying-Based Prediction**: Uses qualifying time with race pace trends for performance estimation
- **Weather-Aware Predictions**: Adjusts based on rain probability and temperature
- **Team Scoring System**: Reflects relative constructor strength from current standings
- **ML-Driven Forecasts**: Gradient Boosting Regressor to predict lap times and overall outcome

## 🧠 Technologies Used

- **Python 3**
- **FastF1** – F1 telemetry and session data
- **pandas / numpy** – Data manipulation
- **scikit-learn** – Regression modeling (GradientBoostingRegressor)
- **matplotlib** – Data visualization
- **OpenWeatherMap API** – Weather forecasting
- **SimpleImputer** – Handling missing values


> Each script is modular and can run independently to predict a specific Grand Prix using up-to-date inputs.

Includes visualizations:

Clean air race pace vs predicted time
Feature importance (qualifying, weather, team, etc.)

## 🚀 Future Improvements

Automate clean-air stint detection from full race data
Include tire strategy and pit stop modeling
Build a Streamlit or Gradio interface for live predictions
Explore classification models for podium/points range prediction
