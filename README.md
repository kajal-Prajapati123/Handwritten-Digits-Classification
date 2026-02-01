# Handwritten-Digits-Classification

# KNN – Handwritten Digit Classification

## 📌 Task Overview
This project implements a **K-Nearest Neighbors (KNN)** classifier to recognize **handwritten digits (0–9)** using the **Sklearn Digits dataset**.  
The task focuses on understanding **distance-based classification**, **feature scaling**, and **K tuning**.

---

## 📊 Dataset
- **Source:** `sklearn.datasets.load_digits()`
- **Total Samples:** 1797
- **Features:** 64 (8×8 pixel values)
- **Target Classes:** Digits from 0 to 9

Each image is an 8×8 grayscale representation of a handwritten digit.

---

## 🛠 Tools & Libraries Used
- Python
- Scikit-learn
- NumPy
- Matplotlib

---

## Methodology
1. Loaded the Digits dataset and verified feature and target shapes.
2. Visualized sample digit images using `matplotlib.imshow()`.
3. Split data into training and testing sets (80/20).
4. Applied **StandardScaler** for feature scaling (important for KNN).
5. Trained KNN model with different K values (3, 5, 7, 9).
6. Evaluated model performance using accuracy.
7. Plotted **Accuracy vs K** to select the best K.
8. Generated **Confusion Matrix** to analyze misclassifications.
9. Displayed test images with predicted labels.

---

## Results

### Accuracy vs K
The accuracy was evaluated for different K values to identify the optimal number of neighbors.

- Best performance observed at an optimal K value.
- Accuracy decreases if K is too low (overfitting) or too high (underfitting).

---

### Confusion Matrix
- Rows represent **actual labels**
- Columns represent **predicted labels**
- Strong diagonal dominance indicates high accuracy.
- Minor misclassifications occur between visually similar digits (e.g., 5 & 9, 8 & 1).

