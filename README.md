# 🌸 Clustering Comparison: K-Means vs. Fuzzy C-Means (C-Means)

> A clean and educational comparison of two unsupervised learning techniques — **K-Means** and **Fuzzy C-Means** — applied on the classic **Iris dataset**.  
> This notebook is designed for research, learning, and demonstration purposes, with a focus on clustering accuracy, performance visualization, and label alignment.

---

## 🔍 Overview

In this notebook, we:

- Load and standardize the Iris dataset 🌱
- Apply both **K-Means** and **Fuzzy C-Means (C-Means)** algorithms
- Automatically align predicted cluster labels to true labels using the **Hungarian Algorithm**
- Visualize cluster assignments and performance
- Evaluate clustering accuracy in a clean and structured way

---

## 📊 Algorithms Compared

| Algorithm        | Type          | Description |
|------------------|---------------|-------------|
| **K-Means**       | Hard Clustering | Each data point belongs to one and only one cluster |
| **Fuzzy C-Means** | Soft Clustering | Each data point has a probability (membership score) of belonging to each cluster |

---

## 📈 Dataset

- **Name:** Iris
- **Features Used:** All 4 (sepal length, sepal width, petal length, petal width)
- **Samples:** 150
- **Classes:** Setosa, Versicolor, Virginica

---

## ✅ Evaluation Method

Since clustering is **unsupervised**, predicted labels do not match ground truth by default.  
To resolve this, we apply the **Hungarian Algorithm** (a.k.a. optimal label alignment) to map clusters to true labels and measure the accuracy.

```python
from scipy.optimize import linear_sum_assignment
from sklearn.metrics import confusion_matrix, accuracy_score

| Algorithm         | Accuracy (Aligned) |
| ----------------- | ------------------ |
| **K-Means**       | \~48–55%           |
| **Fuzzy C-Means** | \~62–65%           |



📁 Project Structure
📦 clustering-comparison-kmeans-vs-cmeans/
├── 📄 README.md
├── 📓 clustering_comparison.ipynb
├── 📊 images/ (optional - for cluster plots)


📬 Contact
Feel free to reach out if you'd like to collaborate, discuss clustering methods, or need help extending this project:

Your Name
📧 Amiroo.azm81@gmail.com
🌐 https://www.linkedin.com/in/amirali-azimi2002/


