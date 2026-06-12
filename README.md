# OIBSIP_DataAnalytics_taskno2
#  Customer Segmentation Analysis Using K-Means Clustering

##  Project Overview

Customer segmentation is a powerful analytical technique used to group customers based on similar characteristics and purchasing behaviors. This project applies Exploratory Data Analysis (EDA) and K-Means Clustering to identify distinct customer groups using demographic information, income levels, spending patterns, purchase behavior, and marketing campaign responses.

The goal of this project is to help businesses better understand their customers, improve marketing effectiveness, and develop personalized customer engagement strategies.

---

##  Objectives

- Analyze customer demographic and purchasing data.
- Perform data cleaning and preprocessing.
- Create meaningful customer-related features.
- Identify spending and purchasing patterns.
- Explore relationships between customer attributes.
- Apply K-Means Clustering for customer segmentation.
- Evaluate cluster quality using Silhouette Score.
- Generate actionable business insights and recommendations.

---

##  Dataset Description

The dataset contains customer information including demographics, purchasing activity, and campaign interactions.

### Customer Information

| Feature | Description |
|----------|------------|
| ID | Customer Identifier |
| Year_Birth | Birth Year |
| Education | Education Level |
| Marital_Status | Marital Status |
| Income | Annual Income |

### Family Information

| Feature | Description |
|----------|------------|
| Kidhome | Number of Children |
| Teenhome | Number of Teenagers |

### Customer Activity

| Feature | Description |
|----------|------------|
| Dt_Customer | Customer Enrollment Date |
| Recency | Days Since Last Purchase |

### Product Spending

| Feature | Description |
|----------|------------|
| MntWines | Amount Spent on Wine |
| MntFruits | Amount Spent on Fruits |
| MntMeatProducts | Amount Spent on Meat Products |
| MntFishProducts | Amount Spent on Fish Products |
| MntSweetProducts | Amount Spent on Sweet Products |
| MntGoldProds | Amount Spent on Gold Products |

### Purchase Channels

| Feature | Description |
|----------|------------|
| NumWebPurchases | Purchases Made Online |
| NumCatalogPurchases | Purchases Made via Catalog |
| NumStorePurchases | Purchases Made in Store |
| NumDealsPurchases | Purchases Made Using Deals |
| NumWebVisitsMonth | Website Visits per Month |

### Campaign Information

| Feature | Description |
|----------|------------|
| AcceptedCmp1-5 | Campaign Acceptance Indicators |
| Response | Response to Latest Campaign |
| Complain | Customer Complaint Status |

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- SciPy
- Jupyter Notebook

---

##  Data Cleaning

The following preprocessing steps were performed:

- Handled missing values in the Income column using median imputation.
- Removed duplicate records.
- Converted date columns into appropriate formats.
- Verified data consistency and quality.

### Missing Values

Only the Income column contained missing values, which were replaced using the median income value.

---

##  Feature Engineering

Several new features were created to improve customer analysis.

### Age

```python
Age = Current Year - Year_Birth
```

### Total Spending (MntTotal)

```python
MntWines +
MntFruits +
MntMeatProducts +
MntFishProducts +
MntSweetProducts +
MntGoldProds
```

### Total Purchases

```python
NumWebPurchases +
NumCatalogPurchases +
NumStorePurchases
```

### Children

```python
Kidhome + Teenhome
```

### In Relationship

Binary feature indicating whether the customer is currently in a relationship.
-0 single 
-1 married

---

##  Exploratory Data Analysis

The following analyses were performed:

### Income Analysis

- Income Distribution Histogram
- Income Box Plot
- Outlier Detection

### Customer Demographics

- Age Distribution
- Marital Status Analysis
- Relationship Status Analysis

### Spending Analysis

- Total Spending Distribution
- Product Category Spending
- Spending Patterns by Customer Segment

### Correlation Analysis

- Correlation Matrix
- Correlation Heatmap
- Point-Biserial Correlation Analysis

### Campaign Analysis

- Campaign Acceptance Rates
- Response Analysis
- Customer Engagement Patterns

---

## 🤖 Customer Segmentation Using K-Means

### Feature Selection

The following features were used for clustering:

- Income
- Age
- MntTotal
- Total_Purchases
- Recency
- Children
- In_relationship

### Data Scaling

StandardScaler was used to normalize feature values before clustering.

### Elbow Method

The Elbow Method was applied to determine the optimal number of clusters.

### K-Means Clustering

K-Means was implemented to divide customers into meaningful groups based on purchasing behavior and demographic characteristics.

### Cluster Evaluation

Silhouette Score was used to evaluate cluster quality and separation.

---

## 📈 Cluster Profiling

Each customer segment was analyzed using:

- Average Income
- Total Spending
- Purchase Frequency
- Family Composition
- Recency
- Campaign Responses

The cluster profiles help identify different customer types and their behavioral characteristics.

---

##  Key Insights

1. Income has a strong influence on customer spending behavior.

2. Customers can be grouped into distinct segments with unique purchasing patterns.

3. High-income customers generally contribute more revenue.

4. Customer spending varies significantly across segments.

5. Product preferences differ among customer groups.

6. Marketing campaign responses vary by customer segment.

7. Relationship status and family composition influence purchasing decisions.

8. Recency plays an important role in customer engagement and activity levels.

9. Certain customer groups exhibit strong loyalty and repeat purchasing behavior.

10. Customer segmentation provides more meaningful insights than analyzing the customer base as a single group.

---

##  Business Recommendations

### High-Value Customers

- Offer loyalty rewards.
- Provide premium product recommendations.
- Create exclusive membership programs.

### Regular Customers

- Encourage repeat purchases through personalized promotions.
- Improve engagement through targeted campaigns.

### Budget Customers

- Offer discounts and bundle deals.
- Promote value-oriented products.

### At-Risk Customers

- Launch reactivation campaigns.
- Provide special offers and incentives.
- Improve customer communication.

---

##  Project Outputs

The project includes:

- Income Distribution Analysis
- Age Analysis
- Spending Analysis
- Correlation Heatmaps
- Product Preference Analysis
- Campaign Analysis
- Customer Segmentation
- Cluster Profiling
- Silhouette Score Evaluation
- PCA Cluster Visualization

---




##  Conclusion

This project successfully applied Exploratory Data Analysis and K-Means Clustering to identify meaningful customer segments based on demographic characteristics and purchasing behavior.

The segmentation results provide valuable insights into customer preferences, spending habits, and engagement patterns. These findings can help businesses design personalized marketing campaigns, improve customer retention, and optimize marketing strategies through data-driven decision-making.

---

##  Author

**RamCharan S**

Data Analytics Internship Project

2026
