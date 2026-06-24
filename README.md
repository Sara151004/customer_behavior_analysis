# Customer Shopping Behavior Analysis
End-to-end customer shopping behavior analysis using Python, PostgreSQL, and Power BI with data cleaning, customer segmentation, and interactive dashboards.

# Overview

Analyzes customer shopping behavior to uncover spending patterns, customer segments, product preferences, and subscription trends — simulating a real-world business analytics workflow from raw data to stakeholder-ready insights.

# Dataset

- **3,900 rows · 18 columns**
- Demographics (Age, Gender, Location, Subscription Status), purchase details (Item, Category, Amount, Season, Size, Color), and behavior (Discount/Promo Use, Frequency, Review Rating, Shipping Type)
- 37 missing `Review Rating` values, imputed using category-level medians

# Tools

`Python (Pandas)` · `PostgreSQL` · `Power BI` · `Gamma` (presentation)

# Workflow

1. **Clean & engineer (Python)** — handled missing values, standardized column names, engineered `age_group` and `purchase_frequency_days`, removed redundant `promo_code_used` column
2. **Analyze (SQL)** — 10 queries covering revenue by gender/age, discount behavior, top products by rating and discount-dependency, subscriber vs. non-subscriber spend, customer segmentation, and repeat-buyer subscription patterns
3. **Visualize (Power BI)** — interactive dashboard with KPI cards and filters by category, gender, subscription, and shipping type
4. **Communicate** — written report and Gamma-generated slide deck for non-technical stakeholders

# Key Insights

- 3,116 of 3,900 customers are "Loyal" vs. just 83 "New" — strong retention, weak acquisition
- Subscribers and non-subscribers spend similarly per order (~$59–60); non-subscribers drive more total revenue purely on volume
- 839 customers spent above average *despite* using a discount
- Most repeat buyers (>5 purchases) are still unsubscribed (2,518 vs. 958) — a clear upsell opportunity
- Accessories and Clothing lead in both sales volume and revenue

# Recommendations

- Promote subscriptions to high-frequency repeat buyers
- Reward loyal customers to drive retention further
- Balance discount strategy against margin impact
- Spotlight top-rated, best-selling products in marketing
- Target high-revenue age groups and Express-shipping users

