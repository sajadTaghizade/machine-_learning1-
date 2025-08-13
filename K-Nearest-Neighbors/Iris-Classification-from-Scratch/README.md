# Neighbors (KNN): Iris Flower Classification

---

### **1. Project Goal**

The objective of this project is to implement the K-Nearest Neighbors (KNN) algorithm from scratch for a multi-class classification task. The model is built to classify species of the Iris flower based on its sepal and petal measurements. The project also includes a comparison with the scikit-learn library and a method for hyperparameter tuning.

---

### **2. Dataset Overview**

This project uses the classic **Iris dataset**, available in the `scikit-learn` library. It is an ideal dataset for demonstrating KNN due to its clean, numeric features and clear class separation.
* **Total Samples:** 150
* **Features:** 4 (Sepal Length, Sepal Width, Petal Length, Petal Width)
* **Number of Classes:** 3 (Setosa, Versicolor, Virginica)



---

### **3. Implementation Methods**

The project was implemented using two distinct approaches:

* **1. From Scratch Implementation:**
    * The entire algorithm was built using only the `NumPy` library and encapsulated in a `KNN` class.
    * **Distance Metric:** The **Euclidean Distance** was implemented to measure the "closeness" between data points.
    * **Prediction Logic:** The model finds the 'K' nearest training samples for each test point and predicts the class based on a **majority vote**.
    * **Lazy Learning:** The `fit` method simply stores the training data, demonstrating the instance-based or "lazy" nature of the algorithm.

* **2. Using the Scikit-learn Library:**
    * The `KNeighborsClassifier` class was used to build a standard model. This served as a baseline to validate the correctness of the from-scratch implementation, with both models achieving identical results.

---

### **4. Hyperparameter Tuning: Finding the Optimal K**

A key part of this project was finding the best value for the `K` hyperparameter. The "Elbow Method" was used to achieve this:
1.  The model was trained and evaluated for a range of `K` values (from 1 to 25).
2.  The accuracy for each `K` was plotted.
3.  The value of `K` that resulted in the highest accuracy was identified as the optimal choice for this dataset.

<div align="center">
  <img src="./assets/k_accuracy_plot.png" alt="Accuracy vs. K Value Plot" width="600"/>
  <p><i>Plot showing the model's accuracy for different values of K.</i></p>
</div>

---

### **5. Final Result**

The from-scratch KNN model was successfully implemented and validated against the scikit-learn version. Through hyperparameter tuning, the optimal value for `K` was determined, resulting in a highly accurate classifier for the Iris dataset. This project demonstrates a complete workflow from algorithmic implementation to model tuning.