Ahhh got you now 😎 — you want a **clean, well-structured, portfolio-ready README** with icons, sections, and a story, like your Iris project example. Here’s one for your MNIST Handwritten Digit Recognition project:

---

# ✍️ Handwritten Digit Recognition (MNIST)

## 📌 Project Overview

This project builds a **neural network** to recognize **handwritten digits (0–9)** using the **MNIST dataset**.
It demonstrates how to preprocess image data, train a simple feedforward neural network, evaluate its performance, and save predictions.

---

## 📊 Dataset Source

* **Dataset Name:** [MNIST Handwritten Digits](http://yann.lecun.com/exdb/mnist/)
* **Source:** Keras datasets
* **Features:** 28×28 grayscale images of digits 0–9
* **Target:** The correct digit (0–9)

---

## 🛠 Steps Performed

1. **Data Loading & Exploration:**

   * Loaded MNIST dataset from local `data` folder
   * Visualized sample images with `matplotlib`

2. **Data Preprocessing:**

   * Normalized pixel values to the range \[0,1]
   * Reshaped 28×28 images into 784-length vectors for the neural network

3. **Modeling:**

   * Built a **feedforward neural network** using `TensorFlow/Keras`:

     * Input layer: 784 neurons (flattened image)
     * Hidden layers: 128 and 64 neurons with `ReLU` activation
     * Output layer: 10 neurons with `Softmax` activation

4. **Training & Evaluation:**

   * Compiled model with `Adam` optimizer and `sparse_categorical_crossentropy` loss
   * Trained on 60,000 images for 5 epochs
   * Evaluated accuracy on 10,000 test images

5. **Predictions:**

   * Generated predictions on test images
   * Saved predicted labels to `scripts/predicted_labels.npy`

---

## 📊 Results

* **Test Accuracy:** \~97%
* Visual inspection of predictions confirms the model can accurately classify handwritten digits.

---

## 💡 Notes

* Preprocessing (normalization & reshaping) is essential for neural network performance
* The model is simple and suitable for beginners; convolutional networks (CNNs) can further improve accuracy
* Saved datasets and predictions make the project **self-contained and reproducible**

---

## 📂 Folder Structure

```
handwritten mnist/
│
├── data/        # MNIST dataset saved as mnist_data.npz
├── notebook/    # Jupyter notebook with code and experiments
└── scripts/     # Saved predictions and future scripts
```

---

## 👤 Author

**Olayinka Johnson-Ige**

---


