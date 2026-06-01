# 🚗 Car Price Prediction with Machine Learning

A machine learning project that predicts the **selling price of used cars** based on various features such as fuel type, transmission, car age, and more. Multiple regression algorithms are trained, evaluated, and compared to identify the best-performing model.

---
**CodeAlpha Internship Project**

![MasterHead](https://img.freepik.com/free-vector/car-showroom-center-with-autos-exhibition-inside-automobile-dealership-store-shop-interior-new-modern-vehicles-models-demonstration-sale-trading_575670-1511.jpg?w=826)

## Problem Statement

**Project Overview:**

In the automotive industry, determining the price of a car involves various factors such as brand reputation, car features, fuel type, transmission, and kilometers driven. Car price prediction is a crucial application of machine learning that helps buyers and sellers make informed decisions.

**Key Objectives:**

- Explore the factors affecting used car prices.
- Build and compare multiple machine learning regression models to predict car prices.
- Evaluate models using MAE, MSE, RMSE, and R-squared score.
- Identify the best-performing model for accurate price prediction.

---

## Project Summary

**Objective:** Develop a machine learning model to predict used car selling prices based on various influencing factors.

**Why Car Price Prediction?** Used car prices are influenced by numerous variables including fuel type, transmission, seller type, kilometers driven, and car age. Machine learning models can capture these complex relationships and provide accurate price predictions.

**Key Tasks:**

1. **Data Collection:** Load car dataset containing attributes and corresponding selling prices.
2. **Data Preprocessing:** Handle missing values, duplicate records, and prepare data for modeling.
3. **Feature Engineering:** Create `Car_Age` from the Year column; encode categorical variables using Label Encoding.
4. **Model Building:** Train 5 regression models — Linear Regression, Decision Tree, Random Forest, SVR, and XGBoost.
5. **Model Evaluation:** Assess each model using MAE, MSE, RMSE, and R-squared score.
6. **Feature Importance:** Analyze which features most influence car selling price using Random Forest.

---

## Dataset

- **File:** `car data.csv`
- **Target Variable:** `Selling_Price`

| Feature | Description |
|---------|-------------|
| Car_Name | Name of the car model |
| Year | Year of manufacture (engineered to Car_Age) |
| Selling_Price | Price the car was sold at (target) |
| Present_Price | Current showroom price |
| Kms_Driven | Total kilometers driven |
| Fuel_Type | Petrol / Diesel / CNG |
| Selling_type | Dealer / Individual |
| Transmission | Manual / Automatic |
| Owner | Number of previous owners |

---

## Tech Stack

| Category | Libraries |
|----------|-----------|
| Data Manipulation | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn` |
| Machine Learning | `scikit-learn`, `xgboost` |
| Environment | Jupyter Notebook |

---

## Data Visualization

- **Correlation Heatmap** — feature correlation matrix
- **Selling Price Distribution** — histogram with KDE curve
- **Fuel Type Count** — bar chart of fuel type distribution
- **Car Age vs Selling Price** — scatter plot showing price trend with age
- **Model Performance Comparison** — bar chart comparing R-squared scores
- **Feature Importance** — Random Forest feature importance ranking

---

## Results

Models are evaluated and ranked by R-squared score:

| Model | MAE | RMSE | R2 Score |
|-------|-----|------|----------|
| Linear Regression | — | — | ~0.64 |
| Decision Tree Regressor | — | — | ~0.70 |
| Support Vector Regressor | — | — | ~0.60 |
| Random Forest Regressor | — | — | ~0.93 |
| XGBoost Regressor | — | — | ~0.90 |

> Exact scores are generated when the notebook is run.

---

## Conclusion

This project explores the dynamics of the used car market, aiming to predict selling prices accurately using machine learning.

**Key Insights:**

- **Petrol** is the most common fuel type in the dataset, followed by Diesel and CNG.
- **Dealer** sellers generally ask for higher prices than individual sellers.
- **Manual** transmission cars significantly outnumber Automatic ones, but Automatic cars typically sell at higher prices.
- **First Owner** cars command higher selling prices compared to Second or Third Owner vehicles.
- Cars with **fewer kilometers driven** tend to have higher selling prices — a clear negative relationship.
- **Car Age** is one of the strongest predictors of selling price — newer cars fetch higher prices.
- **Random Forest** and **XGBoost** consistently outperformed other models with R-squared scores above 90%.
- The **Random Forest model** was selected as the best model due to its balance of accuracy and generalization.

---

## How to Run

1. **Clone the repository**
```bash
git clone https://github.com/khadijaabid0900/CodeAlpha_Car_Price_Prediction.git
cd CodeAlpha_Car_Price_Prediction
```

2. **Install dependencies**
```bash
pip install numpy pandas matplotlib seaborn scikit-learn xgboost jupyter
```

3. **Launch Jupyter Notebook**
```bash
jupyter notebook Car_Price_Predicition.ipynb
```

4. **Run all cells** from top to bottom.

---

## Requirements

```
numpy
pandas
matplotlib
seaborn
scikit-learn
xgboost
jupyter
```

---

## Author

**Khadija Abid**
Data Scientist | Machine Learning Engineer
[LinkedIn](https://www.linkedin.com/in/khadija-abid-61bbba314/)

---

## Reference

- [CodeAlpha](https://www.codealpha.tech/)




