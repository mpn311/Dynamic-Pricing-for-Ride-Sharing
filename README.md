# 🚕 Dynamic Pricing for Ride-Sharing 

## 📌 Project Overview

This project aims to build a machine learning-based **dynamic pricing engine** for ride-sharing platforms. The system adjusts ride prices based on **real-time supply and demand**, **ride features**, and **external factors**  weather, time, and traffic. The goal is to maximize revenue while maintaining user satisfaction and fair pricing.

---

## 📊 Dataset

### 1. Ride Data
- Pickup and Dropoff Times
- GPS Coordinates
- Trip Distance and Duration
- Ride Fare (Actual Price)
- Estimated Wait Time
- Number of Ride Requests (Demand)
- Number of Available Drivers (Supply)

### 2. External Factors
- Weather Information (temperature, rainfall)
- Traffic Conditions
- Time Features: Hour of Day, Day of Week
- Event Flags (Holiday, Weekend, Local Events)

---

## 🎯 Problem Statement

> Predict the **optimal ride price** given the context of a ride using machine learning models. The system should consider supply-demand imbalance and external variables to generate a **real-time surge multiplier or price**.

---

## 🔍 Features

| Feature | Description |
|--------|-------------|
| `hour_of_day`, `day_of_week` | Time-based patterns |
| `ride_density_in_area` | Proxy for ride demand |
| `driver_density_in_area` | Proxy for driver supply |
| `weather_score` | Rain, temperature-based scoring |
| `historical_avg_price` | Average past price for area & time |
| `is_peak_time`, `is_weekend`, `is_holiday` | Event flags for surge detection |

---

## 🧠 Machine Learning Models

### Baseline
- Linear Regression
- Random Forest Regressor

### Advanced
- Gradient Boosted Trees (XGBoost)
- Neural Networks (LSTM or GRUfor time-series forecasting)

---

## 📈 Evaluation Metrics

- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**
- **Revenue Impact Simulation**
- **User Drop-off Rate Estimation** (based on price elasticity)

---

