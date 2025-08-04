<div align="center">
  <img src="https://www.ionos.com/digitalguide/fileadmin/DigitalGuide/Teaser/machine-learning-t.jpg" alt="Project Banner" width="800"/>
  <h1>Linear Regression: Predicting Student Scores</h1>
  <p>
    An in-depth exploration of Linear Regression by implementing the algorithm from scratch in multiple ways and comparing it with the industry-standard Scikit-learn library.
  </p>
  
  <p>
    <img src="https://img.shields.io/badge/Python-3.10%2B-blue.svg" alt="Python Version">
    <img src="https://img.shields.io/badge/Library-Scikit_Learn-orange.svg" alt="Scikit-Learn">
    <img src="https://img.shields.io/badge/Library-NumPy-blue.svg" alt="NumPy">
    <img src="https://img.shields.io/badge/Library-Pandas-lightgrey.svg" alt="Pandas">
    <img src="https://img.shields.io/badge/Library-Matplotlib-green.svg" alt="Matplotlib">
  </p>
</div>

---

## 📋 Project Overview

This project serves as a comprehensive case study on **Simple Linear Regression**. The primary goal is to predict a student's final score based on the number of hours they studied. The project goes beyond a simple implementation by building the regression model using four distinct methods to provide a deep understanding of the underlying mechanics.

---

## ✨ Key Features & Implementations

The core of this project is the comparison of different approaches to solve a linear regression problem. The model was built using:

1.  **Ordinary Least Squares (OLS) from Scratch:** Manually implementing the statistical formulas to calculate the optimal coefficients.
2.  **Gradient Descent from Scratch:** An iterative optimization algorithm to find the model parameters by minimizing the cost function.
3.  **The Normal Equation:** A direct, analytical solution using linear algebra to find the optimal parameters.
4.  **Scikit-Learn Library:** Utilizing the industry-standard `LinearRegression` model for a quick and optimized implementation.

---

## 📊 Dataset

The dataset used is a simple CSV file containing two columns:
* `Hours`: The number of hours a student studied.
* `Scores`: The final score achieved by the student.

| Hours | Scores |
|-------|--------|
| 2.5   | 21     |
| 5.1   | 47     |
| 3.2   | 27     |
| 8.5   | 75     |
| ...   | ...    |


---

## 📈 Visualization of Results

All implementation methods produced nearly identical results, confirming the validity of our manual calculations. The final regression line effectively models the relationship between hours studied and scores.

<div align="center">
  <img src="./assets/regression_plot.png" alt="Regression Plot" width="600"/>
  <p><i>Best-fit line plotted against the test data.</i></p>
</div>

---

## 🧠 Mathematical Concepts Explored

<details>
<summary><b>Click to expand: Mathematical Foundations</b></summary>
<br>
  
### Ordinary Least Squares (OLS)
OLS finds the optimal parameters by minimizing the sum of the squared differences between observed and predicted values. It provides a direct formula for the coefficients:
- $\theta_1 = \frac{\sum (x_i - \bar{x})(y_i - \bar{y})}{\sum (x_i - \bar{x})^2}$
- $\theta_0 = \bar{y} - \theta_1\bar{x}$

### Gradient Descent
An iterative approach that adjusts parameters in the opposite direction of the cost function's gradient. The update rules are:
- $\theta_0 := \theta_0 - \alpha \frac{1}{m} \sum (h_\theta(x_i) - y_i)$
- $\theta_1 := \theta_1 - \alpha \frac{1}{m} \sum (h_\theta(x_i) - y_i)x_i$

### The Normal Equation
A closed-form solution using linear algebra that computes the optimal parameters analytically in a single step:
- $\theta = (X^T X)^{-1} X^T y$

</details>

---

## 🚀 How to Run This Project

Follow these steps to set up and run the project on your local machine.

### Prerequisites
Make sure you have Python 3.8+ installed. You will also need the libraries listed in `requirements.txt`.

### Installation
1.  Clone the main repository:
    ```sh
    git clone [https://github.com/your-username/Machine-Learning.git](https://github.com/your-username/Machine-Learning.git)
    ```
2.  Navigate to the project directory:
    ```sh
    cd Machine-Learning/Linear-Regression/Student-Scores-Prediction
    ```
3.  Install the required packages:
    ```sh
    pip install -r requirements.txt
    ```
    *(Note: You may need to create a `requirements.txt` file with NumPy, Pandas, Scikit-learn, and Matplotlib).*

### Usage
You can run the project by executing the main script or Jupyter Notebook:
```sh
# If you are using a Python script
python your_script_name.py

# Or, if you are using a Jupyter Notebook
jupyter notebook your_notebook_name.ipynb
```

---

## 🏁 Results Comparison

The following table summarizes the final parameters and Mean Squared Error (MSE) obtained from each implementation method on the test set.

| Method                  | Intercept ($\theta_0$) | Slope ($\theta_1$) | MSE on Test Set |
|-------------------------|------------------------|--------------------|-----------------|
| OLS from Scratch        | `2.44`                 | `9.83`             | `17.00`         |
| Gradient Descent        | `2.38`                 | `9.84`             | `16.95`         |
| Normal Equation         | `2.44`                 | `9.83`             | `17.00`         |
| **Scikit-Learn** | **`2.44`** | **`9.83`** | **`17.00`** |

<br>

<div align="center">
  <p>Developed with ❤️ by [Your Name Here]</p>
  <a href="https://github.com/your-username">GitHub Profile</a>
</div>