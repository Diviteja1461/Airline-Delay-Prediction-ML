# Airline Flight Delay Prediction Project

**Author:** Dimmiti Divi Teja  


---

## Project Overview

This project analyzes and predicts airline flight delays using the **U.S. Flight Delay Dataset (2008)**.  
It aims to understand delay patterns and build predictive models for:

1. **Classification** – Predicting whether a flight will be delayed by more than 15 minutes.  
2. **Regression** – Predicting the actual delay duration (in minutes).

---

## Objectives

- Perform **data cleaning and preprocessing** (handle missing values, duplicates, and outliers).  
- Conduct **Exploratory Data Analysis (EDA)** to identify delay trends by month, airline, and cause.  
- Train and evaluate **machine learning models** for both classification and regression.  
- Provide **key insights** and recommendations based on the data analysis.

---

## Workflow

### 1. Data Preprocessing
- Handled missing and duplicate values.  
- Clipped extreme outliers for delay columns.  
- Created a new binary column **`Delayed_15`** (1 = delayed >15 min, 0 = on-time).

### 2. Exploratory Data Analysis (EDA)
- Analyzed arrival delay distributions, delay causes, and seasonal trends.  
- Found strong correlation between **departure delay** and **arrival delay (r ≈ 0.95)**.  
- Discovered that **December** and **early-morning flights** face the highest delays.

### 3. Modeling
- **Classification Models:**
  - Logistic Regression  
  - Random Forest Classifier
- **Regression Models:**
  - Linear Regression  
  - Random Forest Regressor

### 4. Evaluation
- **Classification metrics:** Accuracy, Precision, Recall, F1, ROC-AUC  
- **Regression metrics:** RMSE, R²  

---

## Results Summary

| Task | Model | Key Metric | Performance |
|------|--------|-------------|--------------|
| Classification | Logistic Regression | AUC = 0.95, F1 = 0.91 | Excellent accuracy |
| Classification | Random Forest Classifier | AUC = 0.94 | Very good |
| Regression | Random Forest Regressor | R² = 0.96, RMSE ≈ 11 min | Highly accurate |
| Regression | Linear Regression | R² = negative | Poor fit |

---

## Key Insights

- Around **63%** of flights are delayed by more than 15 minutes.  
- **Departure delay** strongly predicts **arrival delay**.  
- **Late aircraft** and **carrier delays** are the top contributors.  
- **December** and **early-morning flights** show maximum delay duration.  
- Airlines such as **JetBlue (B6)** and **YV** have higher average delays.

---

## Conclusion

- Logistic Regression and Random Forest achieved high accuracy in predicting flight delays.  
- Random Forest Regressor estimated delay duration with about 11-minute average error.  
- These models can help airlines optimize scheduling and improve punctuality.

---

## Future Work

- Add weather and airport congestion data for deeper insights.  
- Apply **hyperparameter tuning (GridSearchCV)** to optimize models.  
- Test advanced algorithms like **XGBoost** or **LightGBM**.  
- Deploy a **web dashboard or API** for real-time delay prediction.

---

## Dataset

**Source:** [Kaggle – Airline Delay Causes (2008)](https://www.kaggle.com/datasets/giovamata/airlinedelaycauses)

---

**Dimmiti Divi Teja**  
Email: divitejadimmiti248@gmail.com  
LinkedIn: [linkedin.com/in/diviteja1461](https://www.linkedin.com/in/diviteja1461)
