# 🧠 Handwritten Digits Classification with an MLP Neural Network

---

### **1. Project Goal**

The primary objective of this project is to build, train, and evaluate a Multi-Layer Perceptron (MLP) neural network to classify small (8x8 pixel) images of handwritten digits (0-9). This project serves as a foundational step in understanding the core concepts of deep learning.

---

### **2. Dataset Overview**

This project uses the **Digits dataset**, which is built into the `scikit-learn` library. Key features of this dataset include:
* **Total Samples:** 1,797
* **Features per Sample:** 64 (each 8x8 pixel image is flattened into a 64-element vector)
* **Number of Classes:** 10 (representing the digits 0 through 9)
* **Data Type:** The dataset is preprocessed and ready for modeling.

---

### **3. Implementation Methods**

This project was implemented using two distinct approaches to provide a comprehensive and comparative understanding.

#### **A. Using the Scikit-learn Library**
The first approach utilized the standard, optimized `MLPClassifier` class from `scikit-learn`. This serves as a baseline and represents the standard industry practice for applying MLP models quickly and effectively.

#### **B. From Scratch Implementation**
The second, more in-depth approach involved building the entire neural network from the ground up using only the `NumPy` library. This method provides deep insight into the internal mechanics of a neural network. The process is broken down into the following key steps:

**1. Parameter Initialization**
* The network's parameters (weights and biases) for a one-hidden-layer architecture were initialized.
* **Weights (`W1`, `W2`)** were initialized with small random numbers. This is crucial to "break symmetry" and ensure that neurons in the same layer learn different features.
* **Biases (`b1`, `b2`)** were initialized to zero.

**2. The Feedforward Pass**
* This is the process of passing input data through the network to generate a prediction.
* The sequence of operations is:
    1.  **Hidden Layer Input:** $Z_1 = X \cdot W_1 + b_1$
    2.  **Hidden Layer Output:** $A_1 = \text{ReLU}(Z_1)$
    3.  **Output Layer Input:** $Z_2 = A_1 \cdot W_2 + b_2$
    4.  **Final Probabilities:** $A_2 = \text{Softmax}(Z_2)$
* Intermediate values are stored in a `cache` for use during backpropagation.

**3. The Backpropagation Algorithm**
* This is the core of the learning process. The algorithm works backward from the final output to determine how much each parameter contributed to the overall error by calculating the **gradient** of the cost function with respect to each parameter.

**4. The Parameter Update**
* The parameters are updated using Gradient Descent, nudging them in the opposite direction of the calculated gradient to minimize the cost function.
    > $parameter = parameter - \text{learning\_rate} \times \text{gradient}$

---

### **4. Key Concepts Covered**
* Multi-Layer Perceptron (MLP) Architecture
* Feedforward Propagation & Backpropagation
* Activation Functions (ReLU & Softmax)
* Cost Function (Categorical Cross-Entropy)
* Gradient Descent Optimization
* Feature Scaling & One-Hot Encoding

---

### **5. Final Result**
Both the from-scratch implementation and the Scikit-learn model successfully learned to classify the handwritten digits, achieving a high accuracy of over **97%** on the unseen test data. This result validates the correctness of the manual implementation.