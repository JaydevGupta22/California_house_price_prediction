# 🏠 House Price Prediction

This project focuses on building a predictive model to estimate house prices using machine learning algorithms. It leverages **Linear Regression** and **Random Forest Regressor**, and applies **GridSearchCV** for hyperparameter tuning to optimize model performance.

---

## 📌 Project Overview

Predicting housing prices is a classic regression problem and is useful for real estate insights, investment analysis, and economic forecasting. This project demonstrates how machine learning models can be trained and evaluated on structured tabular data to predict housing prices.

---

## 📂 Dataset

- The dataset contains features such as:
  - Total rooms
  - Total bedrooms
  - Population
  - Households
  - Median income
  - Location (ocean proximity)
  - And more...

- Target variable: `median_house_value` (continuous)

---

## ⚙️ Algorithms Used

### 1. **Linear Regression**
- Simple and interpretable baseline model.
- Achieved an R² score of **66%** on the test set.

### 2. **Random Forest Regressor**
- Ensemble learning method that handles non-linear relationships.
- Hyperparameters tuned using **GridSearchCV**.
- Achieved an R² score of **81%** on the test set.

---

## 🔍 GridSearchCV
Used to tune key parameters of the Random Forest model:
- `n_estimators`
- `max_depth`
- `min_samples_split`

This helped improve performance significantly over default parameters.

---

## 📈 Results Summary

| Model              | R² Score (Test Set) |
|-------------------|---------------------|
| Linear Regression | 66%                 |
| Random Forest     | 81%                 |

---

## 📚 Key Learnings

- Gained a strong understanding of the **basics of Linear Regression and Random Forest** algorithms.
- Learned how to apply **log transformation** to normalize skewed data and improve model performance.
- Developed skills in **hyperparameter tuning** using GridSearchCV.
- Enhanced knowledge of **model evaluation metrics** and **data preprocessing**.

---

## 🛠️ Libraries Used
- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/JaydevGupta22/house-price-prediction.git
   cd house-price-prediction
