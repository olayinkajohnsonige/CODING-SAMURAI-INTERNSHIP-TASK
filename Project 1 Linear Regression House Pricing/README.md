

# 🏠 House Price Prediction with Linear Regression

## 📌 Project Overview

This project predicts **house rental prices** using **Linear Regression**.
The dataset includes features such as **BHK (bedrooms), size, bathrooms, city, furnishing status, tenant type, etc.**

The goal was to build a model that can estimate rental prices and understand the factors that influence them.

---
## 📊 Dataset Source
Original Dataset Name:[House Rent Prediction Dataset](https://www.kaggle.com/datasets/iamsouravbanerjee/house-rent-prediction-dataset)

Source Platform:Kaggle

Original Author:Sourav Banerjee

## ⚙️ Steps Followed

1. **Data Exploration**

   * Used `.describe()` to understand distributions.
   * Checked for **outliers** using **boxplots and IQR method**.
   * Observed that rents above 67,000 were luxury outliers.

2. **Data Cleaning**

   * Removed extreme outliers (to focus on normal houses).
   * Handled missing values.
   * Converted categorical features into numerical form using **OneHotEncoding**.

3. **Feature Engineering**

   * Selected features like:
     `['BHK', 'Size', 'Bathroom', 'Floor', 'Area Type', 'Area Locality', 'City', 'Furnishing Status', 'Tenant Preferred']`

4. **Model Building**

   * Used **Linear Regression** as baseline model.
   * Performed **train-test split** to evaluate.
   * Tried **log-transform** on Rent (but it reduced accuracy).
   * Evaluated with **R² score**.

5. **Model Evaluation**

   * Initial R² ≈ **0.20** (very poor).
   * After cleaning data & removing outliers → R² ≈ **0.60**.
   * Shows that preprocessing has a huge impact on model performance.

---

## 📊 Results

* **R² Score (after cleaning):** \~0.60
* The model explains about **60% of the variance** in rental prices.
* Performance was weaker on luxury houses due to fewer data points.

---

## 📘 What is R² (in simple terms)?

* **R² (R-squared)** measures how well the model’s predictions match the actual data.
* It ranges from:

  * **1.0 (100%)** → perfect predictions 
  * **0.0** → model is no better than just guessing the average
  * **Negative** → model is worse than guessing 

👉 In this project, an **R² of 0.60** means:
The model explains about **60% of the variation** in house rents. It’s not perfect, but it’s a good start considering real estate prices depend on many hidden factors (location, demand, landlord, etc.).


---

## 📚 Learnings

* Data cleaning and **outlier handling** is just as important as the model.
* A simple **Linear Regression** can still give insights if preprocessing is done well.
* Location (`Area Locality`, `City`) and house size are strong predictors of rent.

---

## 🔮 Next Steps

* Try more advanced models (**Random Forest, Gradient Boosting, XGBoost**).
* Use **cross-validation** for more robust evaluation.
* Improve feature engineering (e.g., extracting floor numbers from `"Floor"`, converting `"Posted On"` to recency).

---

✍️ Author: *\[Olayinka Johnson Ige]*

---


