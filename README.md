# 🌫️ Air Quality Index (AQI) Prediction System

ML-powered web application that predicts Air Quality Index (AQI) for Indian cities using machine learning (Stacking Ensemble – Random Forest, Gradient Boosting, Extra Trees, XGBoost) and provides a user-friendly Flask interface.

---

## 🔍 Project Overview

This project predicts AQI based on major air pollutants (PM2.5, PM10, NO2, SO2, CO, O3) along with spatial (latitude, longitude) and temporal (hour, month, day) features.  
Two real-world Excel datasets of Indian cities were merged, cleaned, and used to train a machine learning pipeline that is deployed as a Flask web app.

Main goals:
- Build an end‑to‑end ML pipeline: data preprocessing → model training → evaluation → deployment.
- Provide a simple web UI for real‑time AQI prediction.
- Classify AQI into categories such as *Good*, *Satisfactory/Moderate*, *Moderate to Poor*, *Poor*, *Very Poor*, and *Severe*.

---

## 🧠 Machine Learning Approach

- **Datasets**:  
  - `Dataset_AQI4-5.xlsx`  
  - `Dataset_AQI30-4.xlsx`  
  (City-wise AQI and pollutant readings across India)

- **Features**:
  - Categorical: `City`
  - Numeric: `PM2.5`, `PM10`, `NO2`, `SO2`, `CO`, `O3`, `Latitude`, `Longitude`, `Hour`, `Month`, `Day`


- **Models Trained**:
  - RandomForestRegressor
  - GradientBoostingRegressor
  - ExtraTreesRegressor
  - XGBRegressor
  
- **Target**:
  - Continuous AQI value (regression)

---

## 💻 Tech Stack

- **Language**: Python
- **Libraries**: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `openpyxl`
- **Web Framework**: Flask
- **Frontend**: HTML, CSS, Font Awesome (in `templates/index.html`)
- **Model Persistence**: `pickle` (`model.pkl`)

---

## 🚀 How to Run Locally

 **Clone the repository**
Colab notebook detected. To show errors in colab notebook, set debug=True in launch()
* Running on public URL: https://6f63b29b120b9a937e.gradio.live


Enter city, pollutant values, latitude/longitude and time → click **Predict AQI** to see predicted value and category.

## 📸 Screenshots
<img width="822" height="361" alt="app ss" src="https://github.com/user-attachments/assets/1008e0d4-ec90-42a5-a4d8-c855f40135eb" />
<img width="1888" height="998" alt="Screenshot 2025-12-15 193710" src="https://github.com/user-attachments/assets/0bfaa7a9-2820-459c-970d-183ed1012461" />




---

## 🙌 Credits

- Developed by Nidhi as part of **Infosys Springboard Virtual Internship 6.0**.  
- Datasets: Publicly available Indian city AQI measurements.

