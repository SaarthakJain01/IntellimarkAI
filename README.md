# Intellimark AI Task

**Author**: Saarthak Jain
**LinkedIn**: [linkedin.com/in/saarthakjain01](https://www.linkedin.com/in/saarthakjain01/)
**GitHub**: [github.com/SaarthakJain01](https://github.com/SaarthakJain01)

---

## 📌 Overview

This repository presents a time series forecasting project for predicting product quantities using statistical and machine learning models. The focus was on understanding seasonal trends and improving accuracy by combining model predictions.

---

## 🧰 Libraries Used

* `pandas`, `numpy`
* `matplotlib`, `seaborn`
* `xgboost`, `sklearn`
* `statsmodels`, `prophet`
* `joblib`, `pickle`

---

## 🗃️ Data Description

The dataset consists of categorical and time-based variables:

* **Categorical Variables**:

  * `Channel`: Channel1, Channel2, Channel3
  * `Brand`: B1, B2
  * `Category`: Cat1, Cat2, Cat3
  * `Sub-Category`: Sub-Cat1, Sub-Cat2, Sub-Cat3, Sub-Cat4
  * `Serial Number`: 1 to 5

---

## 📊 Exploratory Data Analysis

* **Time Series Plots**: Indicated a slight upward trend and strong seasonality.
* **Seasonal Decomposition**: Confirmed a periodic pattern of \~84 days.
* **ACF Plot**: Supported the presence of seasonality with a lag of 12 periods.

---

## 🛠️ Feature Engineering

Features created include:

* Lags: `lag_1` to `lag_7`
* Rolling statistics: `rolling_mean_4`, `rolling_mean_8`, `rolling_median_4`, `rolling_median_8`
* Date-based: `year`, `month`

---

## 📈 Forecasting Models

Three main approaches were used:

1. **SARIMA**
2. **Prophet**
3. **Ensemble**: Combined forecast using `0.5 * SARIMA + 0.5 * Prophet`

---

## ✅ Model Performance

* **SARIMA**: Best accuracy for initial months
* **Prophet**: Moderate performance
* **Combined Approach**: Achieved average monthly accuracy of **65%**

---

## 📦 Model Saving

The models were serialized for reuse:

```bash
sarima_model.pkl
prophet_model.pkl
```

Combined forecasts are generated using both.

---

## 🔁 Suggested Improvements

* Extend historical data range for better learning.
* Prefer statistical models (like SARIMA) for stability.
* Use rolling forecasts to prevent performance decay due to engineered features.

---

## 📅 Predictions

* Accurate forecasts made for **June to November 2024**.
* Combined model outperformed individual models in most cases.

---

## 📂 Project Structure

```bash
├── data/                  # Raw and processed data
├── notebooks/             # Jupyter notebooks for EDA and modeling
├── models/                # Saved SARIMA and Prophet models
├── results/               # Prediction outputs and plots
├── Presentation.pptx      # Project summary presentation
└── README.md              # Project documentation
```

---

## 📬 Contact

Feel free to reach out via [LinkedIn](https://www.linkedin.com/in/saarthakjain01/) or [GitHub](https://github.com/SaarthakJain01) for any queries or collaborations.

---
