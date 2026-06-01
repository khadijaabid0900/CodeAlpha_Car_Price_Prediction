# 🚗 Car Price Prediction

A machine learning project that predicts the **selling price of used cars** based on various features such as fuel type, transmission, car age, and more. Multiple regression algorithms are trained, evaluated, and compared to identify the best-performing model.

---

## Project Overview

Used car pricing is a critical problem in the automotive industry. This project builds a complete ML pipeline — from data preprocessing and feature engineering to model training and evaluation — comparing 5 regression models to determine which predicts car prices most accurately.

---

## Dataset

- **Source:** `car data.csv` (local dataset)
- **Target Variable:** `Selling_Price`
- **Features:**

| Feature | Description |
|---------|-------------|
| Car_Name | Name of the car |
| Year | Year of manufacture (converted to Car_Age) |
| Selling_Price | Price the car was sold at (target) |
| Present_Price | Current showroom price |
| Kms_Driven | Total kilometers driven |
| Fuel_Type | Petrol / Diesel / CNG |
| Selling_type | Dealer / Individual |
| Transmission | Manual / Automatic |
| Owner | Number of previous owners |

---

## 🔧 Tech Stack

| Category | Libraries |
|----------|-----------|
| Data Manipulation | `pandas`, `numpy` |
| Visualization | `matplotlib`, `seaborn` |
| Machine Learning | `scikit-learn`, `xgboost` |
| Environment | Jupyter Notebook |

---

## Project Structure

```
Car_Price_Prediction/
│
├── Car_Price_Predicition.ipynb    # Main notebook
├── car data.csv                   # Dataset
└── README.md                      # Project documentation
```

---

## Project Pipeline

### 1. Import Libraries
All necessary libraries imported for data processing, visualization, and machine learning.

### 2. Load Dataset
Dataset loaded from `car data.csv` into a Pandas DataFrame.

### 3. Data Exploration
- First 5 rows preview
- Dataset shape and info
- Missing value check
- Statistical summary
- Duplicate value check

### 4. Data Preprocessing
- **Feature Engineering:** Created `Car_Age` column from `Year` (2026 - Year), then dropped the `Year` column
- **Label Encoding:** Converted categorical columns (`Car_Name`, `Fuel_Type`, `Selling_type`, `Transmission`) into numerical values
- **Feature Scaling:** Applied `StandardScaler` to normalize all features
- **Train-Test Split:** 80% training / 20% testing with `random_state=42`

### 5. Data Visualization
- **Correlation Heatmap** — feature correlation matrix
- **Selling Price Distribution** — histogram with KDE curve
- **Fuel Type Count** — bar chart of fuel type distribution
- **Car Age vs Selling Price** — scatter plot showing price trend with age

###  Model Training & Evaluation
Five regression models trained and evaluated using MAE, MSE, RMSE, and R-squared score:

| Model | Type |
|-------|------|
| Linear Regression | Baseline linear model |
| Decision Tree Regressor | Tree-based non-linear model |
| Random Forest Regressor | Ensemble of 100 decision trees |
| Support Vector Regressor (SVR) | Kernel-based regression |
| XGBoost Regressor | Gradient boosting model |

### 7. Model Comparison & Best Model
- All models ranked by R-squared score
- Bar chart visualizing performance comparison
- Best model selected automatically

### 8. Feature Importance (Random Forest)
- Feature importance scores extracted from Random Forest
- Ranked and visualized to show which features most influence car price

---

## Evaluation Metrics

| Metric | Description |
|--------|-------------|
| MAE | Mean Absolute Error — average prediction error |
| MSE | Mean Squared Error — penalizes large errors |
| RMSE | Root Mean Squared Error — interpretable error in original units |
| R-squared | Proportion of variance explained by the model (higher = better) |

---

## Conclusion

1. Successfully performed data preprocessing and feature engineering.
2. Created `Car_Age` as a more meaningful feature than raw `Year`.
3. Trained 5 regression models and evaluated each with 4 metrics.
4. Compared model performances visually using bar charts.
5. **Random Forest and XGBoost** consistently perform best for car price prediction tasks.

---

##  How to Run

1. **Clone the repository**
```bash
git clone https://github.com/khadijaabid0900/Car_Price_Prediction.git
cd Car_Price_Prediction
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
khadijaabid0900@gmail.com
[LinkedIn](https://www.linkedin.com/in/khadija-abid-61bbba314/)

---

## License

This project is open source and available under the [MIT License](LICENSE).
