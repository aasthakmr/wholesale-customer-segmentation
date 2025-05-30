# Wholesale Customer Segmentation

This repository contains our project for segmenting wholesale customers based on purchasing behavior using K-Means clustering and PCA, conducted as part of an academic group assignment.

## 👥 Team Members
- Aastha  
- Ameer Akhtar  
- Anantha Narayanan Balaji  
- Ko Jen Kang  

## 📌 Objective
To cluster wholesale customers into meaningful segments based on their annual spending across six product categories. These insights are aimed at helping businesses improve inventory planning, customer targeting, and operational efficiency.

## 📊 Dataset
We used the "Wholesale customers data.csv" dataset, which includes the following numerical features:
- Fresh
- Milk
- Grocery
- Frozen
- Detergents_Paper
- Delicatessen

Categorical attributes such as Region and Channel were used for interpretation.

## 🛠️ Methodology

### 1. Data Preprocessing
- Outlier removal using 1.5*IQR to prevent distortion in clustering.
- Standardized numerical data for clustering and PCA.

### 2. Clustering
- Applied K-Means clustering.
- Used Elbow Method and Silhouette Scores to determine the optimal number of clusters (3).

### 3. Evaluation
- Silhouette analysis was conducted to evaluate cluster cohesion and separation.
- Principal Component Analysis (PCA) was used to reduce dimensions for visualization.

### 4. Cluster Summary
- **Cluster 1 ("Tim Horton")**: Large group, low spending power, Horeca channel, prefers Fresh products.
- **Cluster 2 ("Starbucks")**: Fewer clients, high Fresh & Grocery spending, Horeca channel.
- **Cluster 3 ("Walmart")**: Retail-oriented, high spenders on Grocery, Milk, Detergents.
- **Outliers ("Ikea")**: High-revenue clients, mixed channels, dominate Fresh & Grocery purchases.

## 📈 Key Insights
- Channel is a stronger segmentation variable than region.
- Outlier analysis revealed a small set of clients contributing ~45% of revenue.
- Region-based warehouse investment should target "Other" regions, not Lisbon or Oporto.

## 📂 Files
- `customer_clust.csv`: Final clustering result.
- `Technical Document.pdf`: Code and methodology documentation.
- `Managerial document.pdf`: Executive summary and business recommendations.
- `wholesale_customer_segmentation.rmd`: R script.

## 🧠 Future Work
- Consider hierarchical clustering for better granularity.
- Deploy interactive dashboards for ongoing business use.
- Extend the segmentation to temporal purchasing trends.

## 📜 License
This project is for academic use only and is not licensed for commercial redistribution.
