# Insights from Customer Segmentation Analysis  

## Overview  
This document summarizes key insights derived from applying **K-Means, Hierarchical Clustering, and DBSCAN** to segment customers based on their **Recency, Frequency, and Monetary (RFM) values**.  

---

## **1. K-Means Clustering Insights**  
The optimal number of clusters for K-Means was determined using the **Elbow Method**.  

| Cluster | Recency (Mean) | Frequency (Mean) | Monetary (Mean) | Segment Description |
|---------|----------------|------------------|-----------------|----------------------|
| 0       | 4.83           | 1.55             | 3.97            | Low-engagement customers |
| 1       | 4.28           | 4.09             | 6.57            | Moderately active customers |
| 2       | 5.16           | 2.82             | 5.30            | Customers with occasional purchases |
| 3       | 2.12           | 5.09             | 7.54            | **High-value, loyal customers** |
| 4       | 2.75           | 3.18             | 5.61            | Active customers with moderate spending |

### **Key Takeaways from K-Means**
- **Cluster 3 represents the most valuable customers** with frequent and high-spending transactions.  
- **Cluster 0 consists of the least engaged customers**, requiring re-engagement strategies.  
- Clusters 1 and 4 indicate customers with moderate spending patterns and potential for growth.  

---

## **2. Hierarchical Clustering Insights**  
### **Dendrogram Analysis**
- The dendrogram suggested an **optimal cluster count of 5**, aligning with K-Means segmentation.  
- Box plots for **recency** across clusters show clear differentiation in customer behavior.  

### **Key Takeaways from Hierarchical Clustering**
- **Similar clusters emerged as in K-Means**, confirming model stability.  
- Customers with **lower recency (more recent purchases)** tend to have higher frequency and monetary values.  
- The approach effectively highlighted high-value customers.  

---

## **3. DBSCAN Clustering Insights**  
### **Parameter Selection**
- **Epsilon (ε):** 0.4 (selected from the K-distance graph).  
- **Min Samples:** 5 (based on data density).  

### **Results Interpretation**
- **DBSCAN identified multiple small clusters (20+)**, highlighting diverse purchasing behaviors.  
- **Cluster -1 (Noise points):** Represents **outliers or anomalies** in customer spending.  
- **Main Segments:** Similar groups as found in K-Means and Hierarchical Clustering.  

### **Key Takeaways from DBSCAN**
- **Effective for detecting outliers**, which may indicate fraudulent or unique purchasing behaviors.  
- Shows more **granular subgroups**, useful for hyper-personalized marketing.  

---

## **Final Recommendations**  
1. **Target High-Value Customers (Cluster 3, K-Means & Hierarchical)**  
   - Provide exclusive offers and personalized incentives.  
   - Implement loyalty programs to maintain engagement.  

2. **Re-engage Inactive Customers (Cluster 0, K-Means)**  
   - Deploy targeted marketing campaigns.  
   - Offer discounts or promotions to encourage purchases.  

3. **Use DBSCAN for Fraud Detection**  
   - Investigate noise points (Cluster -1) for potential fraudulent activities.  
   - Cross-verify with transaction logs.  

4. **Compare Clustering Models for Business Application**  
   - Use **K-Means for general segmentation** (efficient and interpretable).  
   - Use **Hierarchical for validation and structured insights**.  
   - Use **DBSCAN for outlier detection and niche clusters**.  
