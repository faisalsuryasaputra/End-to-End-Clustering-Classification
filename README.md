# 🚀 End-to-End Customer Segmentation & Prediction Engine

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)
![Status](https://img.shields.io/badge/Status-Completed-green)

## 📌 Project Overview
This project delivers a comprehensive **Machine Learning** solution for customer segmentation. Starting from raw data, I performed **Clustering** to group customers based on their behavioral patterns, analyzed the characteristics of each group (*profiling*), and built a **Classification** model to automatically predict segments for new customers.

This project demonstrates the integration of **Unsupervised Learning** (K-Means, PCA) with **Supervised Learning** (Random Forest, Decision Tree) to solve real-world business problems.

## 🛠️ Workflow (Pipeline)

### 1. Data Preprocessing & Cleaning
- Handling missing values and duplicates.
- Numerical data standardization (*Scaling*).
- Categorical data encoding (*One-Hot Encoding*).

### 2. Clustering (Unsupervised Learning)
- Implementing **K-Means Clustering**.
- Determining the optimal number of clusters ($k$) using the **Elbow Method** and **Silhouette Score** evaluation.
- Dimensionality reduction using **PCA (Principal Component Analysis)** for 2D visualization.

### 3. Cluster Profiling & Interpretation
- Performing *inverse transformation* to return data to its original readable scale.
- Analyzing the characteristics of each cluster (e.g., identifying "High Spenders", "Loyal Customers", etc.) based on statistical means and modes.

### 4. Classification (Supervised Learning)
- Using the generated clusters as "Labels" (Targets).
- Training **Decision Tree** and **Random Forest** models to predict customer segments.
- Performing **Hyperparameter Tuning** using `GridSearchCV` to optimize model accuracy.
