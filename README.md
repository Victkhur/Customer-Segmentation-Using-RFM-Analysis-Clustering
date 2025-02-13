# **Customer Segmentation Using RFM Analysis & Clustering**  

## **Overview**  
This project applies **RFM (Recency, Frequency, Monetary) analysis** and clustering techniques to segment customers based on their purchasing behavior. It leverages **K-Means, Hierarchical Clustering, and DBSCAN** to identify distinct customer groups and provide actionable insights for marketing strategies.

## **Objectives**  
- **Segment customers** based on RFM analysis.  
- **Compare different clustering algorithms** (K-Means, Hierarchical Clustering, DBSCAN).  
- **Visualize customer clusters** for better interpretation.  
- **Provide business insights** and marketing recommendations.

## **Dataset**  
The dataset consists of transactional data, including:  
- **Recency:** Days since the last purchase.  
- **Frequency:** Number of purchases.  
- **Monetary Value:** Total amount spent.  

## **Technologies Used**  
- **Python** (Pandas, NumPy, Scikit-learn)  
- **Matplotlib & Seaborn** (Data Visualization)  
- **SciPy** (Hierarchical Clustering)  
- **DBSCAN** (Density-Based Clustering)  

## **Project Structure**  
```
📂 Customer-Segmentation  
│── 📂 data                # Dataset  
│── 📂 notebooks           # Jupyter Notebooks  
│── 📂 reports             # Analysis & Visualizations  
│── 📂 models              # Saved Models  
│── 📜 README.md           # Project Overview  
│── 📜 requirements.txt    # Required Libraries  
│── 📜 clustering.py       # Clustering Implementation  
│── 📜 visualization.py    # Data Visualization  
│── 📜 insights.md         # Business Insights  
```

## **Implementation Steps**  
1. **Data Preprocessing**  
   - Handle missing values & outliers.  
   - Log transformation of skewed RFM distributions.  

2. **Feature Engineering**  
   - Compute RFM scores.  
   - Normalize features for clustering.  

3. **Clustering Models**  
   - **K-Means Clustering** (Elbow Method for optimal k).  
   - **Hierarchical Clustering** (Dendrogram to decide cluster count).  
   - **DBSCAN** (K-distance graph to find epsilon).  

4. **Cluster Interpretation & Business Insights**  
   - Identify VIP customers, potential churn, and engagement strategies.  
   - Visualize clusters using scatter plots and box plots.  

## **Results & Insights**  
| Cluster | Recency (Mean) | Frequency (Mean) | Monetary (Mean) | Customer Type | Marketing Strategy |  
|---------|----------------|------------------|-----------------|----------------------|-----------------------------|  
| **0** | 4.83 | 1.55 | 3.97 | Inactive Customers | Win-back campaigns |  
| **1** | 4.28 | 4.09 | 6.57 | Moderate Buyers | Loyalty programs |  
| **2** | 5.16 | 2.82 | 5.30 | Low Engagement | Regular promotions |  
| **3** | 2.12 | 5.09 | 7.54 | VIP Customers | Exclusive perks |  
| **4** | 2.75 | 3.18 | 5.61 | Potential Loyalists | Upselling strategies |  

## **Key Visualizations**  
- **Dendrogram** (Hierarchical clustering analysis)  
- **K-Distance Graph** (DBSCAN Epsilon selection)  
- **Cluster Distributions** (Box plots for RFM features)  

## **How to Run the Project**  
1. Clone the repository:  
   ```sh
   git clone https://github.com/yourusername/Customer-Segmentation.git
   cd Customer-Segmentation
   ```  
2. Install dependencies:  
   ```sh
   pip install -r requirements.txt
   ```  
3. Run clustering script:  
   ```sh
   python clustering.py
   ```  
4. Explore results in Jupyter Notebook.  

## **Future Enhancements**  
- **Automate feature selection for clustering**.  
- **Integrate predictive modeling for customer churn**.  
- **Deploy as a web-based dashboard (Flask/Streamlit)**.  

## **Contributors**  
- **John Victor** (Data Analysis & Machine Learning)  
- Contributions welcome! Feel free to submit a PR.  
