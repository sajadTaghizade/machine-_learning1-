# 📊 Clustering Project: Customer Segmentation Analysis

---

### **1. Project Goal**

The objective of this project is to perform a comparative study of three fundamental clustering algorithms to segment customers from a mall dataset. The goal is to identify distinct customer groups based on their annual income and spending score, providing insights for targeted marketing strategies.

---

### **2. Dataset Overview**

This project uses the **Mall Customers dataset** from Kaggle. It's a classic dataset for unsupervised learning tasks.
* **Features Used:** `Annual Income (k$)` and `Spending Score (1-100)`.
* **Goal:** To group the 200 customers into meaningful segments without any prior labels.



---

### **3. Algorithms Implemented & Compared**

This project explores and compares the following three clustering algorithms:

#### **A. K-Means Clustering**
* **Method:** A centroid-based algorithm that partitions data into a pre-specified number of clusters (K).
* **Optimal K:** The "Elbow Method" was used to determine the optimal number of clusters, which was found to be **5**.
* **Result:** Successfully identified 5 distinct, well-separated, and spherical customer segments.

#### **B. Hierarchical Clustering**
* **Method:** An agglomerative (bottom-up) approach that builds a hierarchy of clusters.
* **Optimal K:** The **Dendrogram** was plotted and analyzed to find the optimal cluster count, which was also determined to be **5**.
* **Result:** The clustering result was very similar to K-Means, confirming the strong underlying structure in the data.

#### **C. DBSCAN (Density-Based Spatial Clustering)**
* **Method:** A density-based algorithm that groups together closely packed points and marks outliers as noise.
* **Parameters:** `eps` and `min_samples` were used instead of a predefined K.
* **Result:** DBSCAN identified the dense core groups of customers and correctly labeled a few sparse data points as outliers, showcasing its ability to handle noise.

---

### **4. Comparative Summary**

| Feature | K-Means | Hierarchical Clustering | DBSCAN |
| :--- | :--- | :--- | :--- |
| **Core Idea** | Centroid-based | Hierarchy-based | Density-based |
| **Input Parameters** | Number of clusters (K) | Cutoff for Dendrogram (or K) | Epsilon (`eps`) & Min Samples |
| **Cluster Shape** | Assumes spherical clusters | Can find more complex shapes | Finds arbitrary shapes |
| **Handles Outliers**| No (sensitive to them) | No (sensitive to them) | Yes (its main strength) |
| **Scalability** | High (very fast) | Low (slow for large data) | Medium |

---

### **5. Conclusion**

This project successfully demonstrated and compared the application of three different clustering techniques. While K-Means and Hierarchical Clustering produced similar and easily interpretable segments for this particular dataset, DBSCAN provided the unique ability to isolate noise points. The choice of algorithm depends heavily on the dataset's structure and the specific goals of the analysis.