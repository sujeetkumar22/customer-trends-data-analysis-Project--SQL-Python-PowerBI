# Customer trends Data Analysis Project Using SQL,Python,PowerBI
Customer Shopping Behavior Analysis
📌 Project Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across various product categories. The primary goal is to uncover insights into spending patterns, customer segments, product preferences, and subscription behavior to guide strategic business decisions.
<img width="4872" height="2656" alt="image" src="https://github.com/user-attachments/assets/37aaea47-7862-4419-a117-8a03c26dd41f" />
<img width="1082" height="604" alt="image" src="https://github.com/user-attachments/assets/7ececd0b-7a21-4b97-999f-07d2674617e5" />
📂 Dataset Summary
The analysis utilizes a dataset containing 3,900 rows and 18 columns.


Customer Demographics: Age, Gender, Location, Subscription Status.


Purchase Details: Item Purchased, Category, Purchase Amount, Season, Size, Color.


Shopping Behavior: Discount Applied, Promo Code Used, Previous Purchases, Frequency, Review Rating, Shipping Type.


Data Quality: Identified 37 missing values in the Review Rating column.

🛠️ Tools & Technologies Used

Python (Pandas): Data cleaning, preprocessing, and exploratory data analysis (EDA).



SQL (PostgreSQL): Structured query analysis to answer key business questions.



Power BI: Creation of an interactive dashboard for visual insights.

⚙️ Methodology
1. Data Preparation (Python)

Data Loading & Exploration: Imported dataset and inspected structure/summary statistics.


Handling Missing Data: Imputed missing values in Review Rating using the median rating of each product category.

Feature Engineering:

Created an age_group column by binning customer ages.

Derived purchase_frequency_days from purchase data.


Standardization: Renamed columns to snake case and dropped redundant columns like promo_code_used.



Database Integration: Loaded the cleaned DataFrame into PostgreSQL.

2. Strategic Analysis (SQL)
Key business questions were addressed through SQL queries, including:

Revenue comparison by gender.

Identification of high-spending discount users.

Top products by review rating and discount rates.


Analysis of shipping types and subscription impact.


Customer segmentation (New, Returning, Loyal).

3. Visualization (Power BI)
Built a "Customer Behavior Dashboard" to visualize metrics such as average purchase amount ($59.76), average rating (3.75), and revenue by category.




📊 Key Insights
💰 Revenue & Demographics

Gender Gap: Male customers generated significantly higher total revenue ($157,890) compared to Female customers ($75,191).



Age Groups: The "Young Adult" group contributed the highest revenue ($62,143), followed closely by "Middle-aged" ($59,197).

🛍️ Product Performance

Top Rated Items: "Gloves" (3.86) and "Sandals" (3.84) hold the highest average product ratings.


Heavily Discounted: "Hat" and "Sneakers" are the products with the highest percentage of discounted purchases, at approximately 50%.


Category Leaders: "Jewelry" is the top accessory, while "Blouse" and "Pants" lead the clothing category with 171 orders each.

👥 Customer Behavior & Segmentation

Subscriptions: Only 27% of customers are subscribers, while 73% are non-subscribers.




Loyalty: The vast majority of customers fall into the "Loyal" segment (3,116 customers), compared to only 83 "New" customers.


Shipping: There is a negligible difference in average spend between "Express" ($60.48) and "Standard" ($58.46) shipping users.

🚀 Business Recommendations
Based on the analysis, the following actions are recommended:


Boost Subscriptions: Promote exclusive benefits to convert the 73% non-subscriber base.



Enhance Loyalty Programs: Continue rewarding repeat buyers to maintain the strong "Loyal" customer segment.


Targeted Marketing: Focus marketing efforts on high-revenue age groups (Young Adults) and highlight top-rated products in campaigns.


Review Discount Policy: Analyze the high discount rates on products like Hats and Sneakers to balance sales boosts with margin control.
<img width="4872" height="2656" alt="image" src="https://github.com/user-attachments/assets/37aaea47-7862-4419-a117-8a03c26dd41f" />


