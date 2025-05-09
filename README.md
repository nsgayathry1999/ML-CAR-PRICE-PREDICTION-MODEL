# ML-CAR-PRICE-PREDICTION-MODEL
# 🚗 Car Price Prediction Using Machine Learning

## 📌 Problem Statement

A Chinese automobile company plans to enter the US market and wants to understand the key factors affecting car prices. The goal is to build a predictive model that can estimate the price of cars based on various features and help the company align its product design and pricing strategy with the American market.

---

## 🎯 Objectives

- Identify which features significantly influence car prices.
- Build and compare multiple regression models.
- Determine the best-performing model based on evaluation metrics.
- Perform feature importance analysis and hyperparameter tuning.

---

## 📂 Dataset

- **File**: `CarPrice_Assignment.csv`
- **Records**: 205 rows × 26 columns
- **Target Variable**: `price`

---

## 🔧 Step 1: Data Preprocessing

- Extracted car brand from `CarName` and corrected typos.
- Removed irrelevant features like `car_ID`, `CarName`.
- Handled categorical variables using one-hot encoding.
- Scaled numerical features using `StandardScaler`.
- Checked and confirmed no missing values or major outliers.

---

## 🤖 Step 2: Model Implementation

Five regression models were implemented:
1. **Linear Regression**
2. **Decision Tree Regressor**
3. **Random Forest Regressor**
4. **Gradient Boosting Regressor**
5. **Support Vector Regressor**

---

## 📊 Step 3: Model Evaluation

All models were evaluated using:
- **R² Score**
- **Mean Squared Error (MSE)**
- **Mean Absolute Error (MAE)**

| Model                  | R² Score | MSE      | MAE      |
|------------------------|----------|----------|----------|
| Random Forest Regressor | **0.93+** | Lowest   | Lowest   |
| Gradient Boosting      | ~0.91    | Low      | Low      |
| Linear Regression      | ~0.85    | Moderate | Moderate |
| Decision Tree          | ~0.76    | High     | High     |
| Support Vector Regressor | ~0.70  | High     | High     |

✅ **Best Model:** Random Forest Regressor

---

## 📌 Step 4: Feature Importance Analysis

Top 5 important features:
1. `engine size`
2. `curb weight`
3. `horsepower`
4. `highway mpg`
5. `carwidth`

---

## 🛠️ Step 5: Hyperparameter Tuning

- Performed Grid Search on `RandomForestRegressor`:
  - `n_estimators`, `max_depth`, `min_samples_split`, `min_samples_leaf`
- Improved performance:
  - R² Score increased to **0.94+**
  - MSE and MAE further reduced

---

## 📈 Business Impact

- Enables better **pricing strategy** and **design decisions**.
- Identifies key car attributes that influence pricing in the US.
- Useful for **cost optimization** and **targeted feature development**.


---

## 📌 Future Enhancements

- Add external data like fuel prices or safety ratings.
- Create a real-time prediction app using **Streamlit** or **Flask**.
- Deploy model as a REST API or integrate with a dashboard.

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib / Seaborn (optional for visualization)

---



