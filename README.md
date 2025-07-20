# 🏠 House Price Prediction Project

This project focuses on predicting house prices using two popular machine learning algorithms — **Linear Regression** and **Random Forest Regressor**. The goal is to build an efficient and interpretable regression model using feature engineering, data preprocessing, and hyperparameter tuning techniques.

---

## 📌 Project Flow

1. **Data Loading**  
   Loaded the California housing dataset and checked for basic structure.

2. **Missing Value Treatment**  
   - Checked for null values  
   - Dropped missing entries for simplicity

3. **Exploratory Data Analysis (EDA)**  
   - Explored features through summary statistics  
   - Visualized distributions and relationships using plots

4. **Log Transformation**  
   - Applied log transformation on skewed features (like target)  
   - Resulted in a more **Gaussian bell-shaped distribution** suitable for regression models

5. **Encoding Categorical Features**  
   - Used **One-Hot Encoding** for `ocean_proximity` categorical column

6. **Feature Engineering**  
   - Created new meaningful features such as:  
     `rooms_per_household = total_rooms / households`  
     `bedrooms_per_room = total_bedrooms / total_rooms`  
     `population_per_household = population / households`

7. **Train-Test Split**  
   - Split the dataset into training and testing sets

8. **Model Development**

   - ### 🔹 Linear Regression
     - No significant difference with or without StandardScaler  
     - **R² Score**: 0.6829  
     - **MAE**: 46,835.53  
     - **MSE**: 4.14 × 10⁹  
     - **RMSE**: 64,400.72  
     - **Accuracy (approx)**: 68.2%

   - ### 🔹 Random Forest Regressor
     - **R² Score**: 0.8066  
     - **MAE**: 32,844.84  
     - **MSE**: 2.52 × 10⁹  
     - **RMSE**: 50,292.89  
     - **Accuracy (approx)**: 80.66%

   - ### 🔹 After Hyperparameter Tuning (GridSearchCV)
     - Best parameters found:  
       `{'max_depth': None, 'min_samples_split': 2, 'n_estimators': 150}`
     - **R² Score**: 0.8089  
     - **MAE**: 32,711.51  
     - **MSE**: 2.49 × 10⁹  
     - **RMSE**: 49,995.83  
     - **Accuracy (approx)**: 80.88%

---

## 📈 Evaluation Metrics (Used)

- **R² Score**: Measures how well the predictions approximate actual values (closer to 1 is better).
- **MAE (Mean Absolute Error)**: Average absolute difference between actual and predicted prices.
- **MSE (Mean Squared Error)**: Penalizes larger errors more than MAE.
- **RMSE (Root Mean Squared Error)**: Interpretable error metric in the same units as price.

---

## 💡 Key Learnings

- Gained hands-on understanding of both **Linear Regression** and **Random Forest** algorithms.
- Learned the impact of **log transformation** to make the data normally distributed for better model performance.
- Understood the importance of **feature engineering** and **hyperparameter tuning** in improving model accuracy.

---

## 🚀 Future Improvements

- Try **XGBoost** and **Gradient Boosting Regressors**
- Deploy model using Flask or Streamlit
- Automate preprocessing and model pipeline

---

## 📂 Directory Structure




---

## 🧠 Author

- **Jaydev Gupta**  
  3rd-year B.Tech Student – AI & Data Science  
  Passionate about ML, DL, and Data Analytics

---


