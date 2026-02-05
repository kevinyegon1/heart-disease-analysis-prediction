# Predicting Heart Disease: EDA & Classification

An end-to-end data science project utilizing Kaggle's Heart Disease dataset to identify key biological indicators of cardiac issues and build a predictive model.

## 📌 Project Overview
This project explores the factors that contribute most to heart disease. By analyzing patient data (age, cholesterol, heart rate, etc.), the goal is to develop a machine learning model capable of predicting the presence of heart disease with high precision.

## 📊 Exploratory Data Analysis (EDA) Findings
I have completed the initial EDA phase. Key insights include:

* **Class Imbalance:** The target variable shows more "Absent" cases than "Present," indicating a need for data balancing techniques (e.g., SMOTE) before modeling.
* **Demographics:** Patients are primarily aged between 50 and 65.
* **Feature Distribution:** * **Cholesterol, Max HR, and ST Depression** are all skewed to the right.
    * Age is relatively evenly distributed.
* **Key Risk Correlations:**
    * Disease is more prevalent in patients **over age 50**.
    * Heart Rate **below 150 BPM** and ST Depression **above 1** are strong indicators of disease presence.
    * Interestingly, Cholesterol and BP showed minimal direct impact on the target variable in this specific dataset.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
* **Environment:** Jupyter Notebook / Kaggle Kernels

## 🚀 Future Roadmap
- [ ] Implement data balancing (Oversampling/Undersampling).
- [ ] Apply feature scaling to address right-skewed data.
- [ ] Train and compare classification models (Random Forest, Logistic Regression, XGBoost).
- [ ] Hyperparameter tuning for the best-performing model.

---
## 🧬 Dataset
The data used in this project is sourced from the [Kaggle Heart Disease Dataset](https://www.kaggle.com/).
