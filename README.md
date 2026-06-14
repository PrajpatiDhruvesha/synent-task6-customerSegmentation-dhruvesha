# Task 6: Customer Segmentation using K-Means Clustering

## Problem Statement

Group customers based on their purchasing behavior using K-Means Clustering. The objective is to identify distinct customer segments based on annual income and spending score, enabling businesses to better understand customer patterns and design targeted marketing strategies.

---

## Dataset Details

### Dataset Name
Mall Customers Dataset (`Mall_Customers.csv`)

### Description
The dataset contains customer information collected from a shopping mall, including demographic details and spending behavior. It is commonly used for customer segmentation and clustering analysis.

### Features

- CustomerID
- Gender
- Age
- Annual Income (k$)
- Spending Score (1-100)

---

## Approach

### 1. Data Loading
- Imported the dataset using Pandas.
- Examined dataset structure using `df.info()`.

### 2. Feature Selection
- Selected the following features for clustering:
  - Annual Income (k$)
  - Spending Score (1-100)

### 3. Data Scaling
- Applied `StandardScaler` to standardize the selected features.
- Ensured both features contributed equally to the clustering process.

### 4. Finding Optimal Number of Clusters
- Used the Elbow Method.
- Calculated WCSS (Within-Cluster Sum of Squares) for cluster values from 1 to 10.
- Visualized the results to determine the optimal number of clusters.

### 5. Applying K-Means Clustering
- Implemented K-Means clustering with 5 clusters.
- Assigned a cluster label to each customer.

### 6. Cluster Visualization
- Created a scatter plot of:
  - Annual Income (k$)
  - Spending Score (1-100)
- Colored customers according to their assigned clusters.

### 7. Cluster Analysis
- Calculated average Annual Income and Spending Score for each cluster.
- Analyzed the characteristics of different customer groups.

### 8. Cluster Size Visualization
- Created a count plot to display the number of customers in each cluster.

---

## Results

### Elbow Method
- Identified the optimal number of clusters for customer segmentation.

### Customer Segmentation
- Successfully divided customers into 5 distinct groups based on spending behavior and income levels.

### Cluster Visualization
- Clearly showed separation between customer groups.
- Revealed different spending patterns among customers.

### Cluster Summary
- Provided average income and spending score for each cluster.
- Helped understand characteristics of each customer segment.

### Cluster Size Analysis
- Displayed the distribution of customers across different clusters.

---

## Tools & Libraries Used

- Python
- Pandas
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook
