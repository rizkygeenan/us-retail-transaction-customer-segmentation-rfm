# 🛒 US Retail Transaction & Customer Segmentation Analysis (RFM)

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Manipulation-orange.svg)
![Power BI](https://img.shields.io/badge/Power_BI-Dashboard-yellow.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)

## 📌 Project Overview
This Final Project is part of the Data Analytics & Business Intelligence Bootcamp (dibimbing.id Batch 23) program. This project focuses on an in-depth analysis of retail transaction behavior in the United States (US) market and the implementation of the RFM (Recency, Frequency, Monetary) model for customer segmentation. The objective is to identify the root causes of low customer retention (one-time buyers) and formulate data-driven promotional and business optimization strategies.

- **Analysis Period:** March 1, 2023 – February 29, 2024 (1 Year)
- **Market Scope:** United States (USA)
- **Dataset:** Retail Analysis on Large Dataset (Kaggle) — ~302,482 rows of raw data
- **Main Tools:** Python (Pandas, NumPy, SciPy for Statistical Testing), Power BI (Interactive Dashboard)

---

## 🎯 Objectives
1. Analyze general business metrics overview (Total Sales, Total Orders, Total Customers, AOV, and UPT).
2. Group customers into strategic segments using the RFM Segmentation method.
3. Analyze loyalty levels, shopping frequency, and segment trend dynamics over time.
4. Perform statistical tests (Mann-Whitney U Test & Chi-Square Test) to evaluate the relationship between customer satisfaction (ratings & feedback) and churn rates.
5. Formulate actionable recommendations for marketing strategies and service recovery.

---

## 📊 Key Findings & Insights

### 1. Key Performance Indicators (US Market)
- **Total Sales:** $129.98M driven by an Average Order Value (AOV) of $1.39K from 93.71K total orders, indicating a dominance of high-ticket products.
- **Units Per Transaction (UPT):** Stands at 1.32, indicating that most transactions contain only a single product and cross-selling strategies are not yet optimal.
- **Customer Retention Risk:** Average shopping frequency is only 1.62x across 57.96K customers, highlighting a high dominance of one-time buyers and a risk of burning customer acquisition costs (CAC).

### 2. RFM Customer Segmentation
- **Champions & Potential Customers (62% Revenue / $81.7M):** Champions contribute the highest revenue with the highest AOV ($3.01K), while Potential Customers hold the highest UPT (1.43), making them prime targets for upselling.
- **At Risk ($30.4M):** High-value customers who have started transacting less frequently and require immediate win-back intervention.
- **Hibernating (58% / ~34K Customers):** The largest group yet inactive; excluded from mass paid campaigns to maintain ROI efficiency.

### 3. Impact of Customer Experience (Statistical Validation)
- Based on statistical tests (Mann-Whitney U & Chi-Square with a p-value < 0.05), it is statistically proven that dissatisfaction at the start of a transaction directly impacts a customer's decision to churn.
- One-Time Buyers recorded a low average rating of 2.66 with 39.42% leaving 'Poor' feedback, whereas Repeat Buyers consistently gave ratings > 4.

---

## 🖥️ Dashboard Overview
These interactive dashboards were built using Power BI to monitor sales performance, core metrics, and RFM segmentation insights in depth.

### 1. Customer Segmentation Dashboard
* **Main Function:** Displays customer segment proportion distributions, revenue contribution comparisons (Total Sales) across segments, and average shopping frequencies (Avg Frequency).
* **Visual Components:** 
  * Pie Chart illustrating customer count percentages per segment (Champions, Potential Customers, At Risk, Hibernating).
  * Bar Chart showing total revenue (Total Sales) by customer segment.
  * KPI Cards highlighting order metrics and transaction value averages (AOV, UPT).
<img width="861" height="491" alt="customer-segmentation-dashboard" src="https://github.com/user-attachments/assets/f366f9db-ef42-4603-923d-4c98dcaecae8" />


### 2. Customer Behavior Dashboard
* **Main Function:** Analyzes segment trend dynamics over time, correlations between ratings/feedback and retention rates, and product category performance.
* **Visual Components:**
  * Line Chart tracking monthly customer count movements across each segment.
  * Stacked Bar Chart comparing initial feedback between One-Time Buyers and Repeat Buyers.
  * Retention Rate by Rating to visualize the impact of poor reviews on churn risks.
<img width="849" height="492" alt="customer-behavior-dashboard" src="https://github.com/user-attachments/assets/03691bfd-1e3f-4506-a811-32ea2ba331f8" />


---

## 💡 Actionable Business Recommendations

1. **VIP Loyalty & Personalization (Champions):** Provide early access, priority customer service, and non-discount perks such as birthday gifts to stabilize their lifetime value (LTV).
2. **Targeted Cross-Sell & Upsell (Potential Customers):** Drive shopping frequency growth from an average of 2.3x to higher tiers using conditional threshold vouchers and personalized product recommendations.
3. **Automated Win-Back Campaign (At Risk):** Rescue potential revenue of $30.4M by deploying automated, time-sensitive "We Miss You" email campaigns alongside NPS surveys to map out pain points.
4. **Service Recovery System (Low Ratings):** Implement proactive handling within 24 hours for poor reviews (Ratings 1–3), particularly within the Grocery and Electronics categories, to prevent permanent churn.

---

## 📂 Deliverables & Repository Structure

```text
├── dataset/
│   └── US_retail_cleaned_data.csv          # Cleaned dataset used for RFM and analysis
├── notebooks/
│   └── data_preprocessing_and_rfm.ipynb    # Python notebook for cleaning, EDA, RFM, & stats test
├── dashboard/
│   └── Retail_RFM_Dashboard.pbix           # Power BI Interactive Dashboard file
├── reports/
│   └── Final_Project_Presentation.pdf      # Complete presentation slides submitted to LMS
└── README.md                               # Project documentation
