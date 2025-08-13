<div align="center">
  <img src="https://user-images.githubusercontent.com/74038190/212284113-f42a762b-9e19-424a-9129-2b3f790c64c7.gif" alt="Project Banner" width="800"/>
  <h1>Machine Learning Algorithms Collection</h1>
  <p>
    This repository is a personal collection of machine learning algorithms, implemented from scratch and with standard libraries to build a deep, practical understanding of the concepts.
  </p>
  
  <p>
    <img src="https://img.shields.io/badge/Python-3.10%2B-blue.svg" alt="Python Version">
    <img src="https://img.shields.io/badge/Focus-Implementation-brightgreen.svg" alt="Focus">
    <img src="https://img.shields.io/badge/Status-In_Progress-yellow.svg" alt="Status">
  </p>
</div>

---

## 📖 About This Repository

Welcome to my machine learning portfolio! The primary goal of this repository is to serve as a learning journal and a practical showcase of key ML algorithms. Each section is dedicated to a specific algorithm, featuring hands-on projects with detailed explanations and clean, well-documented code.

---

## 📂 Repository Structure

This collection is organized modularly. Each core algorithm resides in its own top-level directory. Inside each directory, you will find one or more projects demonstrating its application with different datasets.

```
/Machine-Learning
├── /Linear-Regression
│   ├── /Project-1
│   └── /Project-2
├── /Logistic-Regression
│   └── ...
└── README.md (You are here)
```

---

## 🚀 Implemented Algorithms & Projects

Here is the current status of the algorithms implemented in this repository.

### ✅ Linear Regression
* **Description:** A fundamental algorithm for modeling a linear relationship between a dependent variable and one or more independent variables.
* **Projects:**
    * **[Student Scores Prediction](./Linear-Regression/Student-Scores-Prediction):** An in-depth project implementing Linear Regression from scratch in 3 ways (OLS, Gradient Descent, Normal Equation) and comparing them to Scikit-learn.

### ✅ Logistic Regression
* **Description:** A classification algorithm used to predict a binary outcome, typically using the Sigmoid function.
* **Projects:**
    * **[Breast Cancer Diagnosis](./Logistic-Regression/Breast-Cancer-Diagnosis):** An implementation from scratch with Gradient Descent, compared against the Scikit-learn library.


### ✅ Neural Networks (MLP)
* **Description:** An implementation of a Multi-Layer Perceptron, a foundational deep learning model, for classification tasks.
* **Projects:**
    * **[Digits Classification from Scratch](./Neural-Networks-MLP/Digits-Classification-from-Scratch):** A detailed implementation of Feedforward and Backpropagation using only NumPy, compared with its Scikit-learn equivalent.


### ✅ Decision Trees
* **Description:** A from-scratch implementation of a CART-like classification tree using Gini Impurity and pre-pruning techniques.
* **Projects:**
    * **[Wine Classification from Scratch](./Decision-Trees/Wine-Classification-from-Scratch):** Building a complete Decision Tree class with `fit` and `predict` methods.


### ✅ K-Nearest Neighbors (KNN)
* **Description:** A from-scratch implementation of the KNN algorithm, a simple instance-based classifier, including hyperparameter tuning.
* **Projects:**
    * **[Iris Classification from Scratch](./K-Nearest-Neighbors/Iris-Classification-from-Scratch):** Building a complete KNN class and finding the optimal K value.


### ✅ Clustering Algorithms
* **Description:** A comparative study of unsupervised clustering techniques to find natural groupings in data.
* **Projects:**
    * **[Customer Segmentation Analysis](./Clustering/Customer-Segmentation-Analysis):** Comparing K-Means, Hierarchical Clustering, and DBSCAN on a mall customer dataset.


---

## ✨ Featured Project: Student Score Prediction

The most complete project in this repository so far. It's a perfect starting point to see the level of detail and implementation in this collection.

➡️ **[View the Project README](./Linear-Regression/Student-Scores-Prediction/README.md)**

This project covers:
-   In-depth mathematical explanations of 4 different implementation methods.
-   Full Python code for each method.
-   A final comparison of the results, showing how all valid methods converge to the same solution.

---

## 🛠️ Tech Stack

The following technologies and libraries are used across the projects in this repository:

* **Python**
* **NumPy** for numerical operations and linear algebra.
* **Pandas** for data manipulation and analysis.
* **Matplotlib** & **Seaborn** for data visualization.
* **Scikit-learn** for industry-standard model implementations and evaluation metrics.
* **Jupyter Notebook** for interactive development and documentation.
