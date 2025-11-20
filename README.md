# customer_behaviour_analysis
A data analysis project showcasing customer behaiour analysis using python,sql and power bi

# 📊 Customer Shopping Behavior Analysis

## 🔍 Overview
This end-to-end data analysis project explores customer shopping behavior using a dataset of **3,900 transactions** across multiple product categories.  
The project covers the full analytics lifecycle: loading the dataset into Python, performing EDA, cleaning data, conducting SQL analysis, building an interactive Power BI dashboard, and presenting insights through a written report and a Gamma presentation.

The goal is to understand customer segments, spending patterns, subscription behavior, and revenue-driving demographics to support data-driven business decisions.  
(Source: Customer Shopping Behavior Analysis PDF) :contentReference[oaicite:0]{index=0}



📂 Dataset
- **Rows:** 3,900  
- **Columns:** 18  
- **Key Features:**  
  - Demographics: age, gender, subscription status, location  
  - Purchase details: item purchased, category, amount, season, size, color  
  - Behavior: discount applied, promo code used, frequency, previous purchases  
  - Ratings & logistics: review rating, shipping type
- **Missing Data:**  
  - 37 missing values in *review_rating* column (handled during cleaning)



 🛠 Tools Used

| Tool / Technology | Purpose |
|------------------|---------|
| **Python (Pandas, NumPy, Matplotlib, Seaborn)** | Data loading, cleaning, EDA, feature engineering |
| **Jupyter Notebook / VS Code** | Development environment |
| **MySQL Server** | SQL analysis for revenue, segmentation, subscriptions, and shipping insights |
| **Power BI** | Interactive dashboard development |
| **Gamma App** | Final presentation |
| **Excel** | Additional checks and manual review |



🧹 Steps Performed

 **1. Data Loading & Cleaning (Python)**
- Imported dataset with pandas  
- Reviewed structure using `.info()` and `.describe()`  
- Imputed missing review ratings using **median rating per category**  
- Renamed columns to **snake_case**  
- Engineered new features:
  - `age_group` (binned ages)
  - `purchase_frequency_days`
- Removed redundant columns (e.g., dropped `promo_code_used`)  


 **2. Exploratory Data Analysis (EDA)**
- Summary statistics  
- Distribution analysis  
- Category-level comparisons  
- Outlier detection  
- Demographic vs. spending behavior explorations  


 **3. SQL Analysis (MySQL Server)**
Performed structured SQL queries to answer business questions:

- **Revenue by Gender**  
- **High-spending discount users**  
- **Top 5 products by review rating** (Gloves, Sandals, Boots, Hat, Skirt) – Page 4  
- **Shipping type comparison**  
  - Express users spend slightly more (60.48 vs 58.46) – Page 4  
- **Subscribers vs non-subscribers**  
  - Non-subscribers generate more total revenue despite lower count – Page 4
  
- Top 3 products per category** – Page 6  
- **Repeat buyers vs subscription likelihood**  
- **Revenue by age group**  
  - Young adults contribute the most revenue (62,143) – Page 7  


4. Power BI Dashboard
Built an interactive Customer Behavior Dashboard showcasing:
- KPIs:  
  - Number of customers: 3.9K  
  - Average purchase amount: $59.76 
  - Average review rating: 3.75
- Visuals:  
  - % of customer ID by subscription status (Yes 27%, No 73%)  
  - Revenue by category  
  - Sales by category  
  - Revenue by age group  
  - Sales by age group  
  - Slicers for subscription status, gender, category, shipping type  



5. Final Report & Gamma Presentation**
- Summarized methodology, key insights, SQL findings, and dashboard results  
- Added visual explanations and business recommendations  
- Created a clean, modern presentation for non-technical audiences



📈 Key Insights & Results

1. Revenue Insights
- Young adults generate the highest revenue(62,143).  
- Middle-aged customers follow closely (59,197).  


2. Subscription Behavior**
- Only **27%** of customers are subscribers  
- Non-subscribers contribute more overall revenue  
- Subscribers spend slightly less on average  


3. Product Performance
- Top-rated products include: Gloves, Sandals, Boots  


4. Shipping Preferences
- Express shipping customers spend more ($60.48) than standard ($58.46).  


5. Customer Segmentation
- Repeat buyers (5+ purchases) are more likely NOT to be subscribers 


6. Business Recommendations
- Boost subscriptions with exclusive perks  
- Strengthen customer loyalty programs  
- Promote high-rated & frequently purchased items  
- Target marketing to high-revenue age groups  




