# 🛍️ Customer Segmentation using Clustering Algorithms

This project performs customer segmentation on an **online retail dataset** using **unsupervised machine learning techniques** (KMeans++, Hierarchical Clustering, DBSCAN). The goal is to identify distinct customer groups to enable **targeted marketing**, **better customer service**, and **revenue growth**.

---

## 📌 Business Problem

The retail business faces challenges in identifying high-value customers, resulting in poor marketing ROI and a lack of personalization. To improve customer engagement and optimize marketing efforts, this project segments customers based on their **purchase behavior**.

---

## 🎯 Objective

- Group customers based on:
  - Quantity purchased
  - Total price spent
  - Number of transactions
- Analyze clusters for business insights
- Provide actionable recommendations for each cluster

---

## 🗂️ Dataset

- Source: `Online Retail.xlsx`  
- Attributes used:
  - `Quantity`
  - `TotalPrice` (calculated)
  - `NumTransactions` (aggregated per customer)

---

## 🧠 Techniques Used

- **Data Preprocessing**
  - Null value handling
  - Feature engineering (`TotalPrice`, `NumTransactions`)
  - Scaling and normalization

- **Clustering Algorithms**
  - `KMeans++`
  - `Agglomerative Clustering`
  - `DBSCAN`

- **Evaluation**
  - Silhouette Score
  - Elbow Method
  - Cluster-wise analysis

---

## 📊 Clustering Observations

### 🔹 KMeans++ Clusters

| Cluster | Quantity | TotalPrice | NumTransactions | Interpretation |
|--------|----------|------------|------------------|----------------|
| 0 | Moderate | Moderate | Moderate | Average customers – target with offers |
| 1 | Very High | Very High | High | VIP customers – high retention priority |
| 2 | Low | Low | Very Low | Inactive customers – limited targeting |
| 3 | High | High | Very High | Loyal bulk buyers – personalized upselling |

---

### 🔹 Hierarchical Clustering Clusters

| Cluster | Quantity | TotalPrice | NumTransactions | Interpretation |
|--------|----------|------------|------------------|----------------|
| 0 | High | High | High | High-value customers |
| 1 | Low | Low | Low | Occasional buyers |
| 2 | Very High | Very High | High | Elite customers |
| 3 | Very Low | Very Low | Very Low | Dormant customers |

---

### 🔹 DBSCAN Clusters

| Cluster | Quantity | TotalPrice | NumTransactions | Interpretation |
|--------|----------|------------|------------------|----------------|
| 0 | Low | Low | Low | Small-scale buyers |
| -1 | Outliers | Mixed | Mixed | Noise or non-clustered transactions |

---

## 📌 Key Takeaways

- Different clustering methods help uncover varying levels of customer behavior.
- High-value customers can be identified and targeted for loyalty programs.
- Low-spend customers can be nudged with discounts or re-engagement campaigns.
- Outliers (DBSCAN) highlight potential data noise or unique customer types.

---

## 🛠️ Tech Stack

- Python
- Pandas, NumPy
- Scikit-learn
- Seaborn, Matplotlib
- Jupyter Notebook

---

## 📁 Folder Structure

