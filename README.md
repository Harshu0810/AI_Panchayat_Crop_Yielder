# 🌾 AI Panchayat – Real-Time Crop Advisory System

**AI Panchayat** is an intelligent, zero‑cost advisory tool for farmers. It combines:
- **Live weather forecasts** (Open‑Meteo)
- **Historical crop yield data** (FAOSTAT)
- **Historical climate data** (NASA POWER / Open‑Meteo archive)
- **Machine learning models** (Random Forest / Gradient Boosting) trained per crop
- **SHAP explainability** to show which factors drive the prediction
- **What‑if analysis** for sowing date shifts

## 🚀 Try it live
👉 [Hugging Face Space](https://huggingface.co/spaces/Jindal909/ai-panchayat)

## 📊 Features
- **Location‑aware**: Enter any Indian village, city, or pincode.
- **7‑day forecast**: Visualise temperature, precipitation, humidity, solar radiation.
- **Yield prediction**: Forecast‑based expected yield for your selected crop.
- **Sowing date optimisation**: Compare yields if you sow 5 days earlier/later.
- **SHAP explanation**: Understand what influences the prediction.
- **Historical context**: Compare with last year's estimate and national trends.
- **Natural language advisory**: Simple, actionable suggestions.

## 🛠️ How it works
1. **Geocode** location → lat/lon (Open‑Meteo Geocoding)
2. **Fetch 7‑day forecast** (Open‑Meteo)
3. **Build feature vector** from forecast + sowing date
4. **Predict yield** using a pre‑trained model (RandomForest/GradientBoosting)
5. **Run what‑if** for sowing date shifts (±5 days)
6. **Compute SHAP values** for explainability
7. **Generate advisory** based on optimal conditions and forecast

## 📁 Project Structure
