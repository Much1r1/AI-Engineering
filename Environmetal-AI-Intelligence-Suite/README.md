🌍 Environmental Impact Analyzer (AI Intelligence Suite)
------
📌 Project Overview
A multi-modal AI system designed to tackle environmental challenges from two angles:
- Macro-Level (The Sentinel): An LSTM-based Time-Series model for predicting city-wide Air Quality (AQI).
- Micro-Level (The Tracker): A Random Forest Classifier that segments individual carbon footprints based on lifestyle behaviors.

🧠 Technical Architecture
1. Pollution Forecaster (Deep Learning)
  Model: LSTM (Long Short-Term Memory).Data: Global Air Quality 2024 (Kaggle).
  Goal: Predict the 25th hour of pollution based on a 24-hour sliding window.
  Performance: Achieved a low MSE on the validation set, successfully identifying periodic "toxic spikes" in city data.
2. Carbon Footprint Classifier (Machine Learning)
Model: Random Forest Classifier.
Input Features: Diet, transport mode, electricity usage, and waste generation.
Accuracy: ~85% precision in identifying "High Impact" vs "Low Impact" lifestyles.
