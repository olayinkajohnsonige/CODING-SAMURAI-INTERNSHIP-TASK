
# 🐦 Tweet Sentiment Analysis with Logistic Regression & Linear SVC

## 📌 Project Overview

This project predicts **sentiment of tweets** (positive or negative) using **Logistic Regression and Linear SVC**.
The dataset includes features such as **tweet text, length, and word content**.

The goal was to build models that can classify tweet sentiments accurately and understand patterns in textual data.

---

## 📊 Dataset Source

Original Dataset Name: [Sentiment140 Dataset](https://www.kaggle.com/datasets/kazanova/sentiment140)

Source Platform: Kaggle

Original Author: Go, Bing Liu

---

## ⚙️ Steps Followed

1. **Data Exploration**

   * Examined tweet lengths and distributions.
   * Checked for **outliers** using **boxplots and IQR method**.
   * Observed some extremely long or short tweets.

2. **Data Cleaning**

   * Removed unnecessary symbols, URLs, and mentions.
   * Converted all text to **lowercase**.
   .

3. **Feature Engineering**

   * Vectorized tweets using **TF-IDF**.
   * Considered including **tweet length** as an extra feature.

4. **Model Building**

   * Implemented **Logistic Regression** and **Linear SVC**.
   * Performed **train-test split** for evaluation.
   

5. **Model Evaluation**

   * Logistic Regression: **Accuracy ≈ 0.791**, balanced precision and recall.
   * Linear SVC: **Accuracy ≈ 0.790**, similar performance with slightly better recall on positive tweets.
   * Shows that preprocessing and vectorization had a strong impact on model performance.

---

## 📊 Results

* **Accuracy (Logistic Regression):** 0.791
* **Accuracy (Linear SVC):** 0.790
* Both models show balanced performance across positive and negative tweets.
* Slight differences in recall suggest Linear SVC may detect positive sentiments slightly better.

---

## 📘 What Accuracy Means (in simple terms)

* **Accuracy** measures the percentage of correctly classified tweets.
* It ranges from:

  * **1.0 (100%)** → perfect predictions
  * **0.0** → model is no better than guessing
  * **Around 0.79** → the model correctly classifies about **79% of tweets**

---

## 📚 Learnings

* Text preprocessing (cleaning, lowercasing, removing noise) is crucial.
* TF-IDF vectorization helps normalize tweet lengths and emphasize important words.
* Both Logistic Regression and Linear SVC are effective baseline models for text classification.

---

## 🔮 Next Steps

* Experiment with **n-grams and additional features** like sentiment lexicons.
* Try **advanced models** such as Naive Bayes, Random Forest, or deep learning (LSTM/BERT).
* Use **cross-validation and hyperparameter tuning** for more robust evaluation.

---

✍️ Author: Olayinka Johnson Ige

---

