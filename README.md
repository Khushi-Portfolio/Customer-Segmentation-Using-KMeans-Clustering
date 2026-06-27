🛍️ Customer Segmentation using K-Means Clustering
📌 1. Project Overview

Customer segmentation is an unsupervised machine learning technique used to divide customers into groups with similar characteristics. In this project, the K-Means Clustering algorithm is applied to segment customers based on Age, Income, and Total Spending. The identified customer segments provide valuable insights that help businesses understand customer behavior and support personalized marketing strategies.

🎯 2. Objective

The objectives of this project are:

📊 Segment customers into meaningful groups using K-Means Clustering.
👥 Analyze customer purchasing behavior.
💰 Identify high-value and low-value customer segments.
🎯 Support personalized marketing campaigns.
📈 Improve customer relationship management.
📊 Enable data-driven business decision-making.
📂 3. Dataset Information
📄 Dataset Name

Customer Personality Analysis

🌐 Dataset Source

Kaggle

📝 Dataset Description

The dataset contains customer demographic information, annual income, purchase behavior, and marketing campaign responses. It is widely used for customer analytics and customer segmentation.

📋 Dataset Features
Column Name	Data Type	Description
ID	Integer	Unique customer identifier
Year_Birth	Integer	Customer's year of birth
Education	Categorical	Customer's education level
Marital_Status	Categorical	Customer's marital status
Income	Numeric	Annual household income
Kidhome	Integer	Number of children at home
Teenhome	Integer	Number of teenagers at home
Dt_Customer	Date	Customer enrollment date
Recency	Integer	Days since the last purchase
MntWines	Numeric	Amount spent on wine products
MntFruits	Numeric	Amount spent on fruits
MntMeatProducts	Numeric	Amount spent on meat products
MntFishProducts	Numeric	Amount spent on fish products
MntSweetProducts	Numeric	Amount spent on sweet products
MntGoldProds	Numeric	Amount spent on gold products
NumDealsPurchases	Integer	Number of purchases made using discounts
NumWebPurchases	Integer	Number of purchases made through the website
NumCatalogPurchases	Integer	Number of purchases made through catalogs
NumStorePurchases	Integer	Number of purchases made in physical stores
NumWebVisitsMonth	Integer	Number of website visits in the last month
AcceptedCmp1	Integer	Accepted Campaign 1
AcceptedCmp2	Integer	Accepted Campaign 2
AcceptedCmp3	Integer	Accepted Campaign 3
AcceptedCmp4	Integer	Accepted Campaign 4
AcceptedCmp5	Integer	Accepted Campaign 5
Response	Integer	Response to the latest marketing campaign
Complain	Integer	Customer complaint status
Country	Categorical	Customer's country of residence
Age (Created)	Numeric	Calculated from Year_Birth
TotalSpending (Created)	Numeric	Sum of spending across all product categories
🎯 Features Used for Clustering
Feature	Purpose
Age	Represents customer age
Income	Represents annual customer income
TotalSpending	Represents total customer spending
🛠️ 4. Tools & Technologies
🐍 Python
📓 Jupyter Notebook
🐼 Pandas
🔢 NumPy
📊 Matplotlib
📈 Seaborn
🤖 Scikit-learn
🔄 5. Methodology
1️⃣ Data Cleaning
Loaded the dataset.
Checked missing values.
Handled missing values.
Removed duplicate records.
Verified data types.
2️⃣ Data Preprocessing
Prepared the dataset for analysis.
Selected relevant variables.
Organized the dataset for clustering.
3️⃣ Data Exploration (EDA)

Performed Exploratory Data Analysis using:

📦 Income Box Plot
📦 Total Spending Box Plot
📊 Income Histogram
📊 Age Histogram
🔥 Correlation Heatmap
📈 Scatter Plot
4️⃣ Feature Engineering

Created two new features:

Age = 2026 − Year_Birth
TotalSpending = Sum of all product spending columns
5️⃣ Feature Selection

Selected the following features:

✅ Age
✅ Income
✅ TotalSpending
6️⃣ Data Scaling

Applied StandardScaler to standardize the selected features before clustering.

7️⃣ Optimal Cluster Selection

Used the Elbow Method to determine the optimal number of clusters.

Calculated WCSS (Within-Cluster Sum of Squares)
Identified the elbow point
Selected K = 4
8️⃣ K-Means Clustering

Applied the K-Means Clustering algorithm to group customers into 4 distinct customer segments based on Age, Income, and Total Spending.

9️⃣ Visualization & Analysis

Generated the following visualizations:

📦 Income Box Plot
📦 Total Spending Box Plot
📊 Income Histogram
📊 Age Histogram
🔥 Correlation Heatmap
📈 Income vs Total Spending Scatter Plot
📉 Elbow Method
🎯 Customer Segmentation Scatter Plot
⭐ Customer Segmentation with Cluster Centroids
📦 Spending Distribution Across Clusters
💡 6. Key Insights
💰 Budget Customers
Low income and low spending customers.
Price-sensitive and responsive to discounts and promotional offers.
🌱 Potential Customers
Moderate income and moderate spending.
Can be converted into high-value customers through personalized marketing and loyalty programs.
⭐ Premium Customers
High income and high spending.
Frequently purchase premium products and contribute significantly to business revenue.
👑 High-Value Customers
Highest income and highest spending.
Represent the most profitable customer segment and should be retained through VIP services and personalized experiences.
🚀 7. Business Impact

This customer segmentation model helps businesses:

🎯 Identify high-value customers.
💌 Design personalized marketing campaigns.
🤝 Improve customer retention strategies.
💵 Optimize promotional offers.
📈 Increase customer lifetime value.
📊 Support data-driven business decisions.
📷 8. Visualizations

The project includes:

📦 Income Box Plot
📦 Total Spending Box Plot
📊 Income Histogram
📊 Age Histogram
🔥 Correlation Heatmap
📈 Income vs Total Spending Scatter Plot
📉 Elbow Method
🎯 Customer Segmentation Scatter Plot
⭐ Customer Segmentation with Cluster Centroids
📦 Spending Distribution Across Clusters
✅ 9. Conclusion

This project successfully applied the K-Means Clustering algorithm to segment customers based on Age, Income, and Total Spending. Four meaningful customer segments were identified, providing valuable insights into customer purchasing behavior. These insights can help businesses implement personalized marketing strategies, improve customer retention, and make informed business decisions through data-driven analytics.
