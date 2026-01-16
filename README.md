# customer_behaviour_data_analysis
data analysis project


# Customer Shopping Behavior Analysis

## Project Overview
This project analyzes customer shopping behavior using transactional data from 3,900 purchases across multiple product categories. The goal is to uncover insights related to spending patterns, customer segments, product preferences, and subscription behavior to support business decision-making.

## Dataset Information
- Total Records: 3,900
- Total Features: 18
- Data Includes:
  - Customer demographics (Age, Gender, Location, Subscription Status)
  - Purchase details (Item Purchased, Category, Purchase Amount, Season, Size, Color)
  - Shopping behavior (Discount Applied, Frequency of Purchases, Review Rating, Shipping Type)
- Missing Values:
  - 37 missing values in the Review Rating column

## Data Cleaning and Preparation
- Checked and handled missing values by imputing median review ratings based on product category
- Renamed columns using snake_case for better readability
- Removed redundant column (promo_code_used)
- Performed feature engineering:
  - Created age_group column
  - Created purchase_frequency_days column
- Loaded the cleaned dataset into PostgreSQL for SQL analysis

## Exploratory Data Analysis (Python)
- Used Pandas and NumPy for data exploration and preprocessing
- Performed descriptive analysis using df.info() and df.describe()
- Analyzed distributions of purchase amounts, ratings, and customer demographics
- Verified data consistency and quality

## SQL Analysis (Business Insights)
The following business questions were answered using PostgreSQL:

1. Revenue comparison by gender
2. Identification of high-spending customers who used discounts
3. Top 5 products based on average review rating
4. Comparison of average purchase amount by shipping type
5. Spending behavior of subscribers vs non-subscribers
6. Products with the highest percentage of discounted purchases
7. Customer segmentation into New, Returning, and Loyal customers
8. Top 3 most purchased products per category
9. Relationship between repeat buyers and subscription status
10. Revenue contribution by different age groups

## Dashboard (Power BI)
- Developed an interactive Power BI dashboard to visualize:
  - Average purchase amount
  - Revenue by category
  - Sales by age group
  - Subscription and shipping behavior

## Key Insights
- Express shipping customers spend slightly more than standard shipping customers
- Loyal customers form the largest customer segment
- Several products are highly dependent on discounts
- Young adults contribute the highest total revenue
- Subscription users show strong long-term business value

## Business Recommendations
- Promote subscription benefits to increase customer retention
- Implement loyalty programs for repeat customers
- Optimize discount strategies to balance revenue and profit
- Highlight top-rated and best-selling products in marketing campaigns
- Focus targeted marketing efforts on high-revenue age groups

## Tools and Technologies
- Python (Pandas, NumPy)
- SQL (PostgreSQL)
- Power BI
- Jupyter Notebook
