# Customer-Shopping-Behavior-Analysis-
Customer Shopping Behavior Analysis using Python, SQL, and Power BI. Explores 3,900 transactions to uncover insights into spending patterns, product preferences, customer segments, and subscription behavior for strategic business decisions.

## 📌 Project Overview
This project analyzes **customer shopping behavior** using transactional data from **3,900 purchases across multiple product categories**.  
The goal was to uncover insights into **spending patterns, customer segments, product preferences, and subscription behavior** to guide strategic business decisions.

---

## 📊 Dataset Summary
- **Rows**: 3,900  
- **Columns**: 18  

**Key Features**:  
- **Customer Demographics**: Age, Gender, Location, Subscription Status  
- **Purchase Details**: Item Purchased, Category, Purchase Amount, Season, Size, Color  
- **Shopping Behavior**: Discount Applied, Promo Code Used, Previous Purchases, Frequency of Purchases, Review Rating, Shipping Type  
- **Missing Data**: 37 values in Review Rating column  

---

## 🐍 Exploratory Data Analysis (Python)
- **Data Loading**: Imported dataset using pandas  
- **Initial Exploration**: Used `.info()` and `.describe()` for structure and summary statistics  
- **Missing Data Handling**: Imputed missing review ratings using median per product category  
- **Column Standardization**: Renamed columns to snake_case for readability  
- **Feature Engineering**:  
  - Created `age_group` by binning ages  
  - Created `purchase_frequency_days` from purchase data  
- **Data Consistency Check**: Verified redundancy between `discount_applied` and `promo_code_used`; dropped `promo_code_used`  
- **Database Integration**: Loaded cleaned DataFrame into MySQL Workbench for SQL analysis  

---

## 🗄️ SQL Business Analysis
Key business questions answered using SQL:  
1. Revenue by Gender  
2. High-Spending Discount Users  
3. Top 5 Products by Rating  
4. Shipping Type Comparison (Standard vs. Express)  
5. Subscribers vs. Non-Subscribers (average spend & revenue)  
6. Discount-Dependent Products  
7. Customer Segmentation (New, Returning, Loyal)  
8. Top 3 Products per Category  
9. Repeat Buyers & Subscriptions (>5 purchases)  
10. Revenue by Age Group  

---

## 📈 Power BI Dashboard
An interactive dashboard was built in **Power BI** to visualize:  
- Revenue trends  
- Customer segments  
- Product ratings & preferences  
- Subscription vs. non-subscription behavior  
- Shipping type comparisons  

---

## 💡 Business Recommendations
- **Boost Subscriptions** → Promote exclusive benefits for subscribers  
- **Customer Loyalty Programs** → Reward repeat buyers to move them into the “Loyal” segment  
- **Review Discount Policy** → Balance sales boosts with margin control  
- **Product Positioning** → Highlight top-rated and best-selling products in campaigns  
- **Targeted Marketing** → Focus efforts on high-revenue age groups and express-shipping users  

---

## 🛠️ Tools & Technologies Used
- **Python (pandas, numpy)** → Data cleaning, feature engineering  
- **MySQL Workbench** → Structured business queries  
- **Power BI** → Dashboard development & visualization  

---

## 🚀 How to Use
1. Clone the repository  
2. Run the Python scripts for data cleaning and feature engineering  
3. Explore SQL queries for business insights  
4. Open the Power BI `.pbix` file to interact with dashboards  

