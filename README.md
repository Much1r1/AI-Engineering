# AI-Driven Fleet Management & Intelligence System
**Phase 1 & 2: Financial Engineering, Predictive Modeling, and NLP Insights**

[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Framework-FastAPI-green.svg)](https://fastapi.tiangolo.com/)
[![AI Engine](https://img.shields.io/badge/AI_Engine-TensorFlow_/_Scikit--Learn-orange.svg)](https://www.tensorflow.org/)

## Project Overview
This repository contains the core intelligence engine for a next-generation car rental application. By leveraging a real-world dataset of 1,300+ vehicles, this system moves beyond simple record-keeping to provide **predictive business insights**, **automated maintenance triggers**, and **AI-personalized recommendations**.

---

## Key AI Features

### 1. Contract Duration Predictor (Regression)
Instead of manual scheduling, the system uses a **Linear Regression & Random Forest** hybrid to forecast how long a vehicle will be off-lot based on customer industry and car category.
* **Performance:** Achieved a Mean Absolute Error (MAE) of **1.72 months**.
* **Key Insight:** AI identified the **Energy Sector** as the highest-stability client, providing **+12 months** of additional contract length compared to standard retail.

### 2. Smart-Match Recommendation Engine
A similarity-search algorithm based on **Cosine Similarity** that ensures 100% fleet utilization.
* **Logic:** If a specific model is unavailable, the AI parses the "Vehicle DNA" (Engine Size + Category) to suggest the top 3 nearest alternatives to the user.

### 3. Sentiment-Driven Maintenance (NLP)
Integrating **HuggingFace Transformers (DistilBERT)** to monitor the "pulse" of the fleet.
* **Automated Action:** The system analyzes raw text reviews; negative sentiment scores coupled with keywords like *"engine"* or *"noise"* automatically flag the vehicle for inspection in the backend.

---

## Data Engineering & Pipeline
Before modeling, the raw financial ledger was transformed via a robust pipeline:
* **Asset Monetization:** Grouped 1,300+ unique license plates to calculate individual **Net Profit/Loss** and ROI.
* **Feature Extraction:** Regex-based parsing of descriptions to isolate **Brand**, **Engine Displacement**, and **Vehicle Tier**.
* **Normalization:** Implemented Label Encoding and One-Hot Encoding for multi-segment categorical data (Mining, Agribusiness, Energy, etc.).



---

## Live Intelligence Report (Sample output)
The system generates unified reports combining financial, predictive, and qualitative data:
--- 📊 INTELLIGENCE REPORT: SGO-201 ---
💰 Lifetime Profit/Loss: $188,287.00
⏳ Predicted Next Rental Length: 32.2 months
🎭 Current Customer Pulse: NEGATIVE (99.1% confidence)
🚨 ACTION REQUIRED: Flagging vehicle for manual inspection.

---

## Technical Architecture
* **Data Science:** `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`
* **Machine Learning:** `Scikit-Learn`, `TensorFlow` (Deep Learning MLP)
* **NLP:** `TextBlob`, `Transformers` (BERT-based)
* **Inference:** `Joblib` for model serialization

---

## Roadmap
- [x] Phase 1: Financial Data Analysis & Cleaning
- [x] Phase 2: Predictive Modeling & Regression
- [x] Phase 3: Sentiment Analysis & NLP Integration
- [ ] **Next Step:** Deploy as a **REST API** using FastAPI & Docker.

---

## 🤝 Contact & Contribution
This project is part of my **AI Engineer Roadmap**. Feel free to reach out for collaboration on car-rental tech or AI optimization!
