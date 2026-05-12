# 🌍 Multi-Target Regression for Urban Air Quality Prediction

## A Comparative Study of Machine Learning Approaches

---

## 📌 Overview

Urban air pollution is a critical global health crisis. This project presents a **comprehensive comparative study** of machine learning approaches for **multi-target regression** of air quality parameters across diverse urban locations. We evaluate four algorithms for predicting **multiple air pollutants simultaneously** — enabling more holistic air quality management systems.

---

## 🎯 Key Contributions

- ✅ **Multi-target prediction framework** — Simultaneous prediction of 8 air quality parameters (NO₂, PM₂.₅, SO₂, NOₓ, O₃, formaldehyde, benzene)
- ✅ **Comprehensive feature engineering** — Temporal lags (1-3 hours), rolling statistics (3-hour windows), calendar indicators, location-based features
- ✅ **Comparative analysis** — SVR, Gradient Boosting, Random Forest, XGBoost evaluated on real-world urban data
- ✅ **State-of-the-art results** — Gradient Boosting achieved **MSE = 8.2894** and **R² = 0.8088**

---

## 🧠 Algorithms Evaluated

| Algorithm | Key Parameters | Performance (R²) |
|-----------|---------------|------------------|
| **Gradient Boosting** | estimators=100, lr=0.05, depth=4 | **0.8088** 🏆 |
| **Random Forest** | estimators=100, depth=5 | 0.7373 |
| **XGBoost** | estimators=200, lr=0.05, depth=4 | 0.7483 |
| **SVR** | RBF kernel, C=100, γ=0.01 | 0.5978 |

> **Gradient Boosting** outperformed all models — best for multi-pollutant forecasting.

---

## 📊 Methodology

### Data Preprocessing
- Data integration from multiple monitoring locations
- Missing value handling (location-specific imputation)
- Temporal alignment to hourly intervals
- Outlier detection & correction

### Feature Engineering (50+ features)
- **Temporal:** Lag features (1,2,3 hrs), rolling mean/std (3-hr windows)
- **Calendar:** Month, quarter, year, day-of-year
- **Location:** Categorical encoding, differential features, spatial context

### Evaluation Metrics
- **MSE** — Mean Squared Error
- **R²** — Coefficient of determination

