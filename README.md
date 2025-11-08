# Customer Segmentation using RFM Analysis

## 📖 Overview  
This project performs **customer segmentation** using **RFM (Recency, Frequency, Monetary)** analysis to identify customer groups based on purchasing behavior.  
By combining **feature engineering**, **unsupervised learning (K-Means)**, and **data visualization**, this analysis helps businesses design targeted marketing strategies and improve customer retention.

---

## 🧩 Workflow Summary

### 1. Data Preprocessing  
- Load transaction dataset (customer ID, date, and purchase amount)  
- Handle missing values and duplicates  
- Convert date columns to datetime format  
- Filter valid transactions (e.g., non-negative amounts)  

### 2. RFM Feature Engineering  
- **Recency**: Days since the customer’s last purchase  
- **Frequency**: Number of transactions per customer  
- **Monetary**: Total spending by each customer  
- Compute RFM metrics for each customer ID  

### 3. RFM Scoring  
- Assign scores (1–5) for each metric:
  - Higher Recency score = more recent purchases  
  - Higher Frequency score = more active customers  
  - Higher Monetary score = more valuable customers  
- Combine RFM scores into a single **RFM Segment**  

### 4. Clustering (K-Means)  
- Apply **K-Means Clustering** on standardized RFM features  
- Determine optimal number of clusters using the **Elbow Method** and **Silhouette Score**  
- Assign cluster labels to each customer  

### 5. Visualization  
- Visualize RFM distributions and cluster separations  
- Plot:
  - Recency vs. Frequency  
  - Frequency vs. Monetary  
  - Cluster heatmap and summary table  

---

## 🛠️ Technologies Used  
- **Python 3**  
- **Pandas**, **NumPy** – data processing  
- **Matplotlib**, **Seaborn** – visualization  
- **Scikit-learn** – clustering (K-Means, scaling, silhouette score)  
- **Jupyter Notebook** – analysis documentation  

---
