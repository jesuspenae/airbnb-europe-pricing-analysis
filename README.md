# 🏠 Airbnb Europe: Strategic Market Analysis

End-to-end data analytics project analyzing Airbnb pricing patterns across 10 European cities — from raw data cleaning to an XGBoost ML model deployed in a Power BI interactive dashboard.

---

## ✅ Key Metrics

| KPI | Value |
|---|---|
| Total Listings | 51,571 |
| Cities Covered | 10 |
| Avg Price per Night | €67.46 |
| Avg Guest Rating | 9.26 / 10 |
| Model R² | 0.737 |
| Model MAE | ±15.20 EUR/night |

---

## 🔍 Main Insights

- **City** is the strongest price driver — Amsterdam and London lead by a wide margin.
- **Entire home/apt** listings are significantly more expensive than private or shared rooms across all cities.
- **Weekend prices** are slightly higher than weekday prices in all cities.
- **Superhost status** does not significantly affect pricing — trust, not price, is the differentiator.
- **Athens and Budapest** show the highest proportion of underpriced listings — potential investment opportunity.

---

## 🤖 ML Model

- **Algorithm:** XGBoost Regressor (300 estimators, max_depth=6)
- **Target:** `price_per_night`
- **Train/Test split:** 80% / 20%
- **Top features:** City, room type, number of bedrooms
- **Output columns:** `predicted_price_ml`, `price_deviation`, `investment_opportunity`

---

## 📊 Power BI Dashboard

5-page interactive report built on the ML-enriched dataset:

| Page | Content |
|---|---|
| Overview | Treemap by city, KPIs, city filter |
| Pricing Analysis | Avg price by city, room type and weekday vs weekend |
| Location & Ratings | Price vs distance to center, ratings by city |
| City Deep Dive | Interactive panel — select any city to see all indicators |
| ML Predictions | Actual vs predicted prices, investment opportunities, deviation by city |

---

## 📘 Notebooks

| File | Description |
|---|---|
| `01_Data_Cleaning_Airbnb.ipynb` | Data ingestion, cleaning and feature engineering |
| `02_EDA_Airbnb.ipynb` | Exploratory data analysis and visualizations |
| `03_ML_XGBoost_Airbnb.ipynb` | XGBoost model training, evaluation and export |

> 🗒️ **Note:** Notebooks run on Google Colab. Update the `FOLDER` path in the first cell to match your Google Drive structure. Run notebooks in order (01 → 02 → 03).

---

## 🛠️ Tools

Python · Pandas · XGBoost · Scikit-learn · Matplotlib · Seaborn · Power BI · Google Colab
