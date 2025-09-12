
# 🌸 Iris Flower Classification

## 📌Project Overview
This project classifies **Iris flowers** into three species: **Iris-setosa**, **Iris-versicolor**, and **Iris-virginica** using machine learning. It’s a classic ML project for practicing **classification** tasks with a small dataset.


## 📊 Dataset Source
* **Original Dataset Name:**[Iris Species](https://www.kaggle.com/datasets/uciml/iris)
* **Source:** Kaggle
* **Features:**

  * 🌿 SepalLengthCm
  * 🌿 SepalWidthCm
  * 🌸 PetalLengthCm
  * 🌸 PetalWidthCm
* **Target:** Species of the flower


## 🛠 Steps Performed

1. **Data Exploration:**

   * Checked for missing values and duplicates
   * Visualized distributions with `countplot` & relationships with `pairplot`

2. **Data Preprocessing:**

   * Removed duplicates for unbiased results
   * Encoded species labels using `LabelEncoder`
   * Split data into training & test sets

3. **Modeling:**

   * Tested ML models:

     * 🌳 Decision Tree Classifier
     * 👥 K-Nearest Neighbors (KNN)

4. **Evaluation:**

   * Measured performance using `accuracy_score` & `confusion_matrix`
   * Compared models in a table and saved results to CSV

## 📊 Results

* **Decision Tree Accuracy:** 93%
* **KNN Accuracy:** 93%

Confusion matrices show most predictions are correct with minimal misclassifications.


## 💡 Notes

* Removing duplicates gives more realistic results
* Visualizations help understand feature relationships
* Can extend with hyperparameter tuning or more models

## 👤 Author

**Olayinka Johnson-Ige** 

---















