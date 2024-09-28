# 🎯 Customer Segmentation Using K-Means Clustering

Welcome to the **Customer Segmentation** project repository! 🚀 This project involves clustering customers into distinct groups based on their characteristics, such as age, income, and spending habits, using K-Means clustering. The goal is to help businesses better understand their customer base for more targeted marketing strategies and improved service delivery. 

---

## 📂 Project Overview

In this project, we implemented **K-Means Clustering** to group customers based on their demographics and spending behavior. We used customer data to create insightful clusters that can assist in customer segmentation, resulting in improved business strategies and personalized services.

---

## 📊 Dataset

The dataset contains customer data with the following columns:

- `Gender` - Male or Female
- `Age` - Customer age
- `Income` - Annual income of the customer
- `Spending` - Spending score, a measure of how much the customer spends

---

## 🛠️ Methodology

1. **Data Preprocessing**
   - One-Hot Encoding (OHE) was applied to the `Gender` column to convert it into numerical format.
   - Feature scaling was done to normalize the `age`, `income`, and `spending` columns.

2. **K-Means Clustering**
   - We determined the optimal number of clusters using the **Elbow Method** by plotting the Sum of Squared Errors (SSE) against different cluster numbers.
   - Once the optimal number of clusters was found, we applied K-Means to group the customers.
   
3. **Evaluation**
   - The performance of the clustering model was evaluated using **Silhouette Score** and **Davies-Bouldin Index**.

---

## 🔍 Results

- **Optimal Number of Clusters**: Based on the elbow plot, we decided to use **4 clusters**.
- **Cluster Descriptions**:
  - **Cluster 0**: This cluster appears to be characterized by older individuals with higher incomes and spending habits.They might be retirees or individuals with established careers and financial stability.

   - **Cluster 1**:  This cluster seems to be a mix of age groups with a slightly lower average income and spending compared to Cluster 0. This could represent a diverse group of individuals, including young professionals, students, or individuals with moderate incomes.

  - **Cluster 2**: This cluster primarily consists of younger individuals with lower incomes and spending levels. They might be students, entry-level professionals, or individuals with limited financial resources.

  - **Cluster 3**: This cluster exhibits a relatively balanced distribution of age, income, and spending, suggesting a diverse group of individuals with varying demographics and financial situations.
 

  
---

## 📈 Performance Evaluation

- **Silhouette Score**: 0.3048 (Moderate clustering quality)
- **Davies-Bouldin Index**: 1.088 (Lower value indicates better clustering)

Both metrics indicate that the K-Means clustering model does a reasonably good job of segmenting the customers, but there might still be some overlap between clusters, as the silhouette score is not very high.

---

## 📊 Visualizations

The following visualizations were created:
1. **Elbow Method Plot** - To determine the optimal number of clusters.
2. **Cluster Distributions** - Subplots displaying the distribution of customers in each cluster for `age`, `income`, and `spending`.
3. **2D Scatter Plot** - A scatter plot showing customer segmentation in two dimensions (age and spending) for visualizing the clusters.

---

## 🛠️ How to Run the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/Dawood-Imran/customers-clustering.git
