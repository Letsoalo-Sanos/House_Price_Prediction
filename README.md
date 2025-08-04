# Housing Price Prediction Project

This project focuses on predicting house prices based on various property features using machine learning techniques. Two regression models—**Linear Regression** and **Random Forest Regressor**—were applied to evaluate and compare performance.

---

## Objective

The objective of this project is to build predictive models that estimate the price of residential properties using structured housing data. The predictions are based on property characteristics such as area, number of rooms, presence of amenities, and furnishing status.

---

## Dataset Overview

The dataset (`Housing.csv`) includes 13 features:

| Feature             | Type         | Description                                  |
|---------------------|--------------|----------------------------------------------|
| `price`             | Target       | Selling price of the house                   |
| `area`              | Numerical    | Total area of the property in square feet    |
| `bedrooms`          | Numerical    | Number of bedrooms                           |
| `bathrooms`         | Numerical    | Number of bathrooms                          |
| `stories`           | Numerical    | Number of floors                             |
| `mainroad`          | Binary       | Located on a main road (yes/no)              |
| `guestroom`         | Binary       | Guest room availability (yes/no)             |
| `basement`          | Binary       | Basement present (yes/no)                    |
| `hotwaterheating`   | Binary       | Hot water system present (yes/no)            |
| `airconditioning`   | Binary       | AC available (yes/no)                        |
| `parking`           | Numerical    | Number of parking spaces                     |
| `prefarea`          | Binary       | Located in preferred area (yes/no)           |
| `furnishingstatus`  | Categorical  | Furnishing level (furnished, semi, unfurnished)|

---

## Data Preprocessing

- Converted binary categorical features (`yes`/`no`) to `1` and `0`
- Applied One-Hot Encoding to `furnishingstatus` to handle multi-class data
- Standardized numerical features (optional, depending on model)
- Checked for duplicates and missing values
- Performed an 80/20 train-test split using `train_test_split()`

---

##  Models Used

###  Linear Regression
- A baseline model for comparison
- Assumes linear relationships between features and target variable

###  Random Forest Regressor
- Tree-based ensemble model
- Captures non-linear interactions between variables
- Robust to outliers and does not require feature scaling

---

## Evaluation Metrics

The models were evaluated using:

- **R² Score** – Measures how well the model explains the variability of the target
- **MAE (Mean Absolute Error)** – Average of the absolute differences between predicted and actual values
- **RMSE (Root Mean Squared Error)** – Penalizes large errors more than MAE

---

## Results & Insights

- **Random Forest Regressor** outperformed **Linear Regression** in all metrics.
- Important features influencing price:
  - `area`
  - `airconditioning`
  - `prefarea`
  - `bathrooms`
- Random Forest effectively captured both linear and non-linear patterns.

---

## Key Learnings

- Categorical features must be encoded properly for model compatibility
- Linear Regression offers simplicity and interpretability
- Random Forest provides higher accuracy and handles mixed data types well
- Evaluation metrics are critical to measure and compare performance

---

## 🛠️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

---

