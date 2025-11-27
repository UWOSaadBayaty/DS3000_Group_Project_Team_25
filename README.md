# 🌧️ DS3000 — Rain Prediction at London Heathrow Airport  
## Final Group Project (Fall 2025)

This project aims to predict **whether it will rain tomorrow at Heathrow Airport** using daily weather observations from the **Weather Prediction Dataset (Huber, 2024)**.  

The goal is to build, compare, and evaluate machine learning models that improve upon simple baselines and provide interpretable insights into what weather features most influence next-day rainfall.

---

## 👥 Group Members
- **Bingrui Wang**  
- **Fatemah Sayed Noor**
- **Hassan Sohail**
- **Mohammed Al-Hashimi**     
- **Saad Al-Bayaty**  
  
All group members contributed to code, analysis, presentation, and the final report.

## 📝 Problem Statement

Predict **rain tomorrow** at Heathrow using:

- Today's local weather features  
- The **MONTH** (to capture seasonality)  
- Historical recordings from 2000–2010

We formulate a **binary classification** task:
We create this target by shifting the precipitation column by one day.

## 📊 Dataset Description

The dataset contains more than 10 years of daily weather observations from multiple European cities.  
For Heathrow specifically, we use:

- `MONTH`
- `HEATHROW_cloud_cover`
- `HEATHROW_humidity`
- `HEATHROW_pressure`
- `HEATHROW_global_radiation`
- `HEATHROW_precipitation`
- `HEATHROW_sunshine`
- `HEATHROW_temp_mean`
- `HEATHROW_temp_min`
- `HEATHROW_temp_max`

The target label (`HEATHROW_rain_tomorrow`) is engineered by shifting tomorrow’s precipitation upward.

The dataset is **nearly perfectly balanced** (≈50.8% rainy, 49.2% not rainy), making it well-suited for unbiased classification.
## 🖥️ How to Run the Notebook

### **1. Install dependencies**
Make sure the following packages are installed:

```bash
pip install numpy pandas scikit-learn matplotlib
