# 🩺 Predicting Heart Disease: Kaggle Classification Project

[![Kaggle Score](https://img.shields.io/badge/Kaggle%20Score-87.97%25-gold?style=for-the-badge&logo=kaggle)](https://www.kaggle.com/)
[![Python](https://img.shields.io/badge/Python-3.9+-blue?style=for-the-badge&logo=python)](https://www.python.org/)
[![ML](https://img.shields.io/badge/Model-Random%20Forest-green?style=for-the-badge)](https://scikit-learn.org/)

An end-to-end data science project utilizing the Kaggle Heart Disease dataset to identify key biological indicators of cardiac issues and build a high-precision predictive model.

## 📌 Project Overview
This project focuses on predicting the presence of heart disease based on clinical parameters. By transitioning from deep Exploratory Data Analysis (EDA) to an optimized Random Forest model, I achieved a competition score of **87.97%**.

## 📊 Key EDA Insights
The initial analysis revealed critical patterns in patient data:
* **Demographic Risks:** Risk factors increase significantly in patients aged **50–65**.
* **Primary Indicators:** Lower **Max Heart Rate** (below 150 BPM) and higher **ST Depression** (above 1.0) are the strongest individual predictors of disease.
* **Feature Distribution:** Identified right-skewness in `Cholesterol` and `ST Depression`, addressed via standard scaling.
* **Low Impact Factors:** Fasting Blood Sugar (FBS) and Cholesterol showed surprisingly low direct correlation with the target in this specific cohort.



## 🛠️ The Machine Learning Pipeline

### 1. Data Preprocessing
* **Cleaning:** Removed `id` column to prevent noise.
* **Encoding:** Transformed target variable (`Presence`/`Absence`) into binary format ($1$/$0$).
* **Scaling:** Implemented `StandardScaler` on numerical features to ensure unit variance for the classifier.

### 2. Modeling & Performance
I chose the **Random Forest Classifier** for its robustness against skewed data and ability to capture non-linear relationships.

* **Final Score:** 87.97% Accuracy
* **Validation Strategy:** Train/Test Split with stratified sampling.

### 3. Feature Importance
Analysis of the model's internal logic confirmed that clinical test results outweigh basic demographics:



## 🚀 Future Enhancements
- [ ] **Hyperparameter Tuning:** Implement `GridSearchCV` to optimize `n_estimators` and `max_depth`.
- [ ] **Advanced Ensembles:** Test XGBoost and LightGBM to improve the score beyond 88%.
- [ ] **Deployment:** Create a simple Streamlit web app for real-time risk assessment.

## 🧰 Tech Stack
* **Analysis:** `Pandas`, `NumPy`
* **Visualization:** `Seaborn`, `Matplotlib`
* **Machine Learning:** `Scikit-Learn`

---
## 🧬 Dataset Credits
The data is sourced from the [Kaggle Heart Disease Dataset](https://www.kaggle.com/).
