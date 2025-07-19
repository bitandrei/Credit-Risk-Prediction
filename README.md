# Phase 1 – ETL & EDA Summary

## ✅ 1. ETL – Extract, Transform, Load

We loaded the dataset from the Kaggle "Default of Credit Card Clients (Taiwan)" dataset.  
We explored the structure and performed cleaning operations:

- Renamed columns for clarity (e.g., `SEX` → `gender`, `PAY_0` → `pay_sep`)
- Replaced numeric encodings with meaningful labels:
  - Gender: `1=Male`, `2=Female`
  - Education: `1=Graduate`, ..., `5/6=Unknown`
  - Marital Status: `1=Married`, `2=Single`, `3=Other`
- Checked for nulls, data types, and outliers
- Saved the cleaned dataset for future steps

---

## 📊 2. EDA – Exploratory Data Analysis

We visualized the data to understand distributions and trends:

- Histograms showed right-skewed distributions in `limit_balance`, `bill_sep`, and `pay_sep`
- Correlation matrix helped detect relationships
- Target variable `default` showed weak correlation with most individual features
- Detected mild multicollinearity in some billing/payment features

---

## 📁 Files Created

- `clean_credit_data.csv` – cleaned and ready for analysis
- `eda_visuals.ipynb` – EDA code and charts

---

## ✅ Phase 1 Complete

We now have a clean, well-understood dataset ready for statistical analysis and modeling.
