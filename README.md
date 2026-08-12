# Image Classification with TensorFlow & MNIST

This repository contains a Jupyter Notebook demonstrating a basic Deep Learning workflow for classifying handwritten digits (0–9) using the **MNIST dataset** and **TensorFlow / Keras**.

---

## 📌 Project Overview
The goal of this project is to build and train a Feedforward Neural Network (Multi-Layer Perceptron) to recognize handwritten digits from 28x28 pixel grayscale images.

---

## 🛠️ Tech Stack & Libraries
* **Python 3**
* **TensorFlow / Keras** (Sequential API)
* **NumPy** (Data Manipulation & Reshaping)
* **Matplotlib** (Data Visualization)

---

## 🚀 Workflow & Pipeline

1. **Data Loading & Exploration:**
   * Loaded the MNIST dataset containing 60,000 training examples and 10,000 test examples.
   * Visualized digit samples using `matplotlib`.

2. **Data Preprocessing:**
   * **One-Hot Encoding:** Converted integer labels into 10-dimensional categorical vectors using `to_categorical`.
   * **Vector Unrolling:** Flattened 28x28 images into 784-element 1D vectors.
   * **Normalization:** Standardized pixel values using mean and standard deviation.

3. **Model Architecture:**
   * **Input Layer:** Flattened 784 features.
   * **Hidden Layer 1:** Dense layer with 128 units and `ReLU` activation.
   * **Hidden Layer 2:** Dense layer with 128 units and `ReLU` activation.
   * **Output Layer:** Dense layer with 10 units and `Softmax` activation for multi-class classification.

4. **Model Compilation & Training:**
   * **Optimizer:** Stochastic Gradient Descent (`SGD`).
   * **Loss Function:** `categorical_crossentropy`.
   * **Epochs:** 3

5. **Evaluation & Prediction:**
   * Evaluated model accuracy on unseen test data (~96.4% test accuracy).
   * Generated class probability predictions for test samples.

---

## 📊 Results
* **Training Accuracy:** ~96.0%
* **Test Set Accuracy:** ~96.4%
* 
