# 🛍️ Customer Segmentation using K-Means Clustering

## 📌 1. Project Overview

Customer segmentation is an unsupervised machine learning technique used to divide customers into groups with similar characteristics. This project applies the K-Means Clustering algorithm to segment customers based on Age, Income, and Total Spending. The identified customer segments help businesses understand customer behavior, improve marketing strategies, and make data-driven decisions.

---

# 🎯 2. Objective

The main objectives of this project are:

-  Segment customers into meaningful groups using K-Means Clustering.
-  Analyze customer purchasing behavior.
-  Identify different customer spending patterns.
-  Support personalized marketing campaigns.
-  Improve customer relationship management.
-  Enable data-driven business decision-making.

---

# 📂 3. Dataset Information

| Column Name | Data Type | Description |
|-------------|-----------|-------------|
| ID | Integer | Unique customer identifier |
| Year_Birth | Integer | Customer's year of birth |
| Education | Categorical | Customer's education level |
| Marital_Status | Categorical | Customer's marital status |
| Income | Numeric | Annual household income |
| Kidhome | Integer | Number of children at home |
| Teenhome | Integer | Number of teenagers at home |
| Dt_Customer | Date | Customer enrollment date |
| Recency | Integer | Number of days since the customer's last purchase |
| MntWines | Numeric | Amount spent on wine products |
| MntFruits | Numeric | Amount spent on fruits |
| MntMeatProducts | Numeric | Amount spent on meat products |
| MntFishProducts | Numeric | Amount spent on fish products |
| MntSweetProducts | Numeric | Amount spent on sweet products |
| MntGoldProds | Numeric | Amount spent on gold products |
| NumDealsPurchases | Integer | Number of purchases made using discounts |
| NumWebPurchases | Integer | Number of website purchases |
| NumCatalogPurchases | Integer | Number of catalog purchases |
| NumStorePurchases | Integer | Number of store purchases |
| NumWebVisitsMonth | Integer | Number of website visits in the last month |
| AcceptedCmp1 | Integer | Accepted Campaign 1 |
| AcceptedCmp2 | Integer | Accepted Campaign 2 |
| AcceptedCmp3 | Integer | Accepted Campaign 3 |
| AcceptedCmp4 | Integer | Accepted Campaign 4 |
| AcceptedCmp5 | Integer | Accepted Campaign 5 |
| Response | Integer | Response to the latest marketing campaign |
| Complain | Integer | Customer complaint status |
| Country | Categorical | Customer's country of residence |
| **Age (Created)** | Numeric | Calculated from **Year_Birth** |
| **TotalSpending (Created)** | Numeric | Total spending across all product categories |

### 🎯 Features Used for Clustering

| Feature | Purpose |
|----------|---------|
| Age | Represents customer age |
| Income | Represents customer's annual income |
| TotalSpending | Represents customer's overall spending |

---

# 🛠️ 4. Tools & Technologies

-  Python
-  Jupyter Notebook
-  Pandas
-  NumPy
-  Matplotlib
-  Seaborn
-  Scikit-learn

---

# 🔄 5. Methodology

### **1️⃣ Data Cleaning**
- Loaded the dataset.
- Checked missing values.
- Handled missing values.
- Removed duplicate records.
- Verified data types.

### **2️⃣ Data Preprocessing**
- Prepared the dataset for analysis.
- Selected relevant variables.
- Organized the dataset for clustering.

### **3️⃣ Data Exploration (EDA)**
Performed Exploratory Data Analysis using:
-  Income Box Plot
-  Total Spending Box Plot
-  Income Histogram
-  Age Histogram
-  Scatter Plot(Income Vs Total Spending)

### **4️⃣ Feature Engineering**
Created two new features:
- **Age = 2026 − Year_Birth**
- **TotalSpending = MntWines + MntFruits + MntMeatProducts + MntFishProducts + MntSweetProducts + MntGoldProds**

### **5️⃣ Feature Selection**
Selected the following features:
-  Age
-  Income
-  TotalSpending

### **6️⃣ Data Scaling**
Applied **StandardScaler** to standardize the selected features before clustering.

### **7️⃣ Optimal Cluster Selection**
Used the **Elbow Method** to determine the optimal number of clusters.
- Calculated Within-Cluster Sum of Squares (WCSS)
- Identified the elbow point
- Selected **K = 4**

### **8️⃣ K-Means Clustering**
Applied the **K-Means Clustering** algorithm to segment customers into **4 distinct customer groups** based on Age, Income, and Total Spending.

### **9️⃣ Visualization & Analysis**
-  Elbow Method
-  Customer Segmentation Scatter Plot
-  Customer Segmentation with Cluster Centroids
-  Spending Distribution Across Clusters

---

# 💡 6. Key Insights

### 💰 Budget Customers
- Low income and low spending customers.
- Respond well to discounts and promotional offers.

### 🌱 Potential Customers
- Moderate income and moderate spending.
- Can be converted into premium customers through targeted marketing and loyalty programs.

### ⭐ Premium Customers
- High income and high spending.
- Frequently purchase premium products and contribute significantly to business revenue.

### 👑 High-Value Customers
- Highest income and highest spending.
- Represent the most profitable customer segment.
- Should be retained through VIP services and personalized experiences.

---

# 🚀 7. Business Impact

This customer segmentation model helps businesses to:

-  Identify high-value customers.
-  Design personalized marketing campaigns.
-  Improve customer retention.
-  Optimize promotional strategies.
-  Increase customer lifetime value.
-  Support data-driven business decisions.

---
# ✅ 8. Conclusion
This project successfully applied the **K-Means Clustering** algorithm to segment customers based on **Age**, **Income**, and **Total Spending**. Four meaningful customer segments were identified, enabling businesses to better understand customer behavior and develop targeted marketing strategies. The insights generated from this analysis support improved customer engagement, stronger retention strategies, and informed business decision-making.
