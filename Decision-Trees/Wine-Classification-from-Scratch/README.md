# 🌳 Decision Tree Project: Classification of Wine Types

---

### **1. Project Goal**

The objective of this project is to implement a Decision Tree classification algorithm from scratch. A complete model was built using the `NumPy` library to gain a practical understanding of core concepts such as the **Gini Impurity** splitting criterion and **recursive** tree building.

---

### **2. Dataset Overview**

This project uses the classic **Wine dataset**, available in the `scikit-learn` library. This dataset is ideal for focusing on the algorithm's logic due to its clean, numeric features.
* **Total Samples:** 178
* **Features:** 13 (including chemical properties like alcohol, malic acid, etc.)
* **Number of Classes:** 3 (representing three different types of wine)

---

### **3. Implementation Methods**

The project was implemented using two different approaches:

* **1. From Scratch Implementation:**
    * The entire logic was encapsulated in a `DecisionTree` class.
    * **Splitting Criterion:** **Gini Impurity** was used to evaluate the quality of each split.
    * **Recursive Structure:** The main `_grow_tree` function recursively builds the tree until a stopping condition is met.
    * **Pre-pruning:** To prevent overfitting, hyperparameters like `max_depth` and `min_samples_split` were implemented.
    * **Prediction:** A separate recursive function, `_traverse_tree`, was implemented to traverse the tree and predict labels for new samples.

* **2. Using the Scikit-learn Library:**
    * The `DecisionTreeClassifier` class was used to build a standard model for comparison and to validate the results of the from-scratch implementation.

---

### **4. Visualizations & Analysis 📊**

To better understand the data and the model's performance, several visualizations were created:
* **Correlation Matrix:** To examine the relationships between different features.
* **Confusion Matrix:** To accurately evaluate the model's errors for each class.
* **Feature Importance:** To identify the most influential features in the wine classification process.
* **Tree Structure:** To visually represent the rules and decisions the model learned.

---

### **5. Final Result**

The from-scratch implementation successfully achieved an accuracy level very close to the standard `scikit-learn` model. This result validates the correct implementation of the algorithm and demonstrates a solid understanding of the key concepts behind decision trees, including the Gini splitting criterion and the recursive building process.