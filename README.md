# Customer Trends Data Analysis Project Using SQL,Python,PowerBI
# Customer Shopping Behavior Analysis

## 📌 Project Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions.


<img width="4872" height="2656" alt="image" src="https://github.com/user-attachments/assets/37aaea47-7862-4419-a117-8a03c26dd41f" />
<img width="1082" height="604" alt="image" src="https://github.com/user-attachments/assets/7ececd0b-7a21-4b97-999f-07d2674617e5" />


## 📂 Dataset Summary
* **Total Records:** 3,900 Rows
* **Total Features:** 18 Columns
* **Key Attributes:**
    * **Demographics:** Age, Gender, Location, Subscription Status
    * **Purchase Details:** Item Purchased, Category, Purchase Amount, Season, Size, Color
    * **Behavior:** Discount Applied, Frequency of Purchases, Review Rating, Shipping Type
* **Data Quality:** Identified and handled 37 missing values in the `Review Rating` column.

## 🛠️ Tech Stack
* **Python (Pandas):** Data cleaning, preprocessing, and exploratory data analysis (EDA).
* **SQL (PostgreSQL):** Structured query analysis for business insights.
* **Power BI:** Interactive dashboard for data visualization.

## ⚙️ Methodology

### 1. Data Preparation (Python)
* **Data Loading:** Imported dataset using Pandas and performed initial exploration using `df.info()` and `describe()`.
* **Missing Data Handling:** Imputed null values in `Review Rating` using the median rating of each product category.
* **Standardization:** Renamed columns to snake case for better readability.
* **Feature Engineering:**
    * Created `age_group` column by binning customer ages.
    * Derived `purchase_frequency_days` column.
* **Data Validation:** Verified redundancy between discount and promo code columns; dropped `promo_code_used`.

### 2. SQL Analysis
Loaded the cleaned data into PostgreSQL to answer key questions:
* Revenue analysis by Gender and Age Group.
* Identification of high-spending discount users.
* Product performance based on rating and discount frequency.
* Customer segmentation (Loyal vs. New).

### 3. Visualization (Power BI)
Built a comprehensive dashboard to track:
* **KPIs:** Average Purchase Amount ($59.76), Average Rating (3.75).
* **Sales Metrics:** Revenue by Category and Age Group.
* **Demographics:** Subscription status distribution.

## 📊 Key Insights

### 💰 Revenue & Demographics
* **Gender Disparity:** Male customers generated significantly higher revenue ($157,890) compared to Female customers ($75,191).
* **Top Spenders:** The **Young Adult** age group contributed the highest revenue ($62,143).

### 🛍️ Product Trends
* **Highest Rated:** "Gloves" have the highest average rating at 3.86.
* **Most Discounted:** "Hats" and "Sneakers" are the most frequently discounted items, with ~50% discount rates.
* **Category Leaders:** "Jewelry" (Accessories) and "Blouse" (Clothing) are the top-selling items by volume.

### 👥 Customer Segmentation
* **Loyalty:** The majority of customers are in the **"Loyal"** segment (3,116), with very few categorized as "New" (83).
* **Subscriptions:** 73% of customers are Non-Subscribers, highlighting a massive opportunity for growth.
* **Shipping:** Express shipping users spend an average of $60.48, marginally higher than Standard shipping users ($58.46).

## 🚀 Business Recommendations
1.  **Boost Subscriptions:** Promote exclusive benefits to the 73% of non-subscribers to increase recurring revenue.
2.  **Loyalty Programs:** Focus on moving "Returning" customers into the "Loyal" segment through rewards.
3.  **Inventory Strategy:** Highlight top-rated products (Gloves, Sandals) in marketing campaigns.
4.  **Discount Optimization:** Review margins on high-discount items like Hats to ensure profitability.


