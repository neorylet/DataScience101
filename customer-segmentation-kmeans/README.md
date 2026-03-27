# Customer Segmentation Using K-Means Clustering and Behavioral Analysis

## Overview
This project applies K-Means clustering to segment retail customers based on income and spending behavior. The objective is to identify distinct customer groups and provide actionable insights that can support targeted marketing and business strategy.

---

## Business Problem
Retail businesses often lack clear segmentation of their customers, resulting in generic marketing strategies and inefficient resource allocation. Without understanding different customer groups, it becomes difficult to:
- Identify high-value customers
- Personalize marketing efforts
- Improve customer retention and engagement

---

## Objectives
- Segment customers using behavioral and financial data
- Identify meaningful customer groups
- Analyze patterns in income, spending, and purchasing behavior
- Provide data-driven business recommendations

---

## Tools and Technologies
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib

---

## Dataset
The dataset contains retail customer information, including:
- Annual Income
- Spending Score
- Purchase Frequency
- Transaction Amount
- Age (used optionally for analysis)

---

## Data Preprocessing
The dataset required cleaning before analysis:
- Missing values in Age and Transaction Amount were handled using median imputation
- Customer ID was removed as it is not relevant for clustering
- Numerical features were standardized using StandardScaler to ensure balanced clustering

---

## Methodology

### Feature Selection
The following features were selected for clustering:
- Annual Income
- Spending Score
- Purchase Frequency
- Transaction Amount

These variables represent both financial capacity and purchasing behavior.

---

### Feature Scaling
All selected features were scaled to normalize their ranges and prevent bias in distance-based clustering.

---

### K-Means Clustering
- The Elbow Method was used to determine the optimal number of clusters
- K-Means clustering was applied to group customers into distinct segments

---

### Evaluation
Clustering performance was evaluated using the Silhouette Score to measure how well-defined the clusters are.

---

## Visualization

### Elbow Method
The Elbow Method helps determine the optimal number of clusters by analyzing inertia across different values of K.

![Elbow Method](images/elbow_method.png)

---

### Customer Segments (Income vs Spending Score)
This plot shows how customers are grouped based on income and spending behavior.

![Customer Segments](images/cluster_income_spending.png)

---

### Purchase Behavior (Frequency vs Transaction Amount)
This visualization highlights differences in purchasing behavior among customer segments.

![Purchase Behavior](images/cluster_frequency_transaction.png)

---

### Cluster Distribution
This chart shows the number of customers in each segment.

![Cluster Distribution](images/cluster_distribution.png)

---

## Results
The model successfully identified distinct customer segments with clear behavioral differences. These segments reveal patterns in spending habits, purchasing frequency, and income levels.

---

## Business Insights

### High-Value Customers
Customers with high income and high spending behavior  
Recommendation: Focus on retention through loyalty programs and premium services

---

### Budget Customers
Customers with lower income and spending levels  
Recommendation: Offer discounts and promotions to increase engagement

---

### Potential Customers
Customers with high income but lower spending  
Recommendation: Target with personalized marketing and upselling strategies

---

### Frequent Low Spenders
Customers who purchase often but spend small amounts  
Recommendation: Introduce bundle offers to increase transaction value

---

## Conclusion
This project demonstrates how clustering techniques can be used to better understand customer behavior and support data-driven decision-making. Customer segmentation enables businesses to tailor strategies for different groups, improving both efficiency and profitability.

---

## Future Improvements
- Experiment with alternative clustering algorithms such as DBSCAN or Hierarchical Clustering
- Incorporate customer lifetime value analysis
- Develop an interactive dashboard for business users

---

## Project Structure

```
customer-segmentation-kmeans/
│
├── data/
│   └── unclean_customer_data.csv
│
├── notebooks/
│   └── segmentation.ipynb
│
├── images/
│   ├── elbow_method.png
│   ├── cluster_income_spending.png
│   ├── cluster_frequency_transaction.png
│   └── cluster_distribution.png
│
└── README.md
```

## Author
Neo Ryle Tubera
