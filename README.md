# 🌱 Week2_Greenhouse_Gas_Emission

This project focuses on analyzing greenhouse gas emissions across supply chains using real-world datasets. The goal is to build a machine learning model that predicts the **Supply Chain Emission Factors without Margins**, based on various quality, geographical, and technological features.

---

## 📂 Dataset

The dataset contains 22,000+ rows and 14 columns, including:

- **Substance**: Material name (e.g., Steel, Cement)
- **Unit**: Measurement unit (e.g., kg, ton)
- **Supply Chain Emission Factors with/without Margins**: Emission values
- **DQ Reliability, Temporal, Geographical, Technological, Data Collection**: Data Quality indicators
- **Source & Year**: Reference metadata

---

## 🧠 Objective

To build a **regression model** that accurately predicts:

> **`Supply Chain Emission Factors without Margins`**

based on other numerical and categorical features.

---

## 🛠️ Workflow

1. **Data Preprocessing**
   - Handle missing values
   - Convert categorical columns using `LabelEncoder`
   - Convert margin columns to `float`
   - Scale features with `StandardScaler`

2. **Model Training**
   - Train/test split (80/20)
   - Train using `RandomForestRegressor`
   - Evaluate using `R² Score` and `Mean Squared Error`
