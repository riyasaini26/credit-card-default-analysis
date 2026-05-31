# Credit Card Default Risk Analysis

## Problem Statement
Credit card default is a major financial risk for banks and fintech companies.
The goal of this project is to identify key factors that contribute to credit 
card bill non-payment, and use these insights to determine whether a customer 
should be targeted for a new credit card offer.

## Dataset
- **Source:** UCI Machine Learning Repository / Kaggle
- **Dataset:** Default of Credit Card Clients 
🔗 [Default of Credit Card Clients - Kaggle]([https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset?resource=download))
- **Size:** 30,000 customer records
- **Features:** Demographics, credit limit, payment history (6 months), bill amounts

## Tools Used
- **Google BigQuery** — data storage and SQL analysis
- **SQL** — querying and deriving insights
- **Power BI** — dashboard and visualization

## Key Insights

### 1. Overall Default Rate
- 22.12% of customers defaulted on their next payment
- 77.88% of customers were reliable payers

### 2. Payment Delay is the Strongest Risk Signal
- Customers with **More than 2 month payment delay** had a **69.6% default rate**
- Customers with **1 month payment delay** had a **33.9% default rate**
- Customers who paid on time had only a **16.8% default rate**

### 3. Credit Limit Bucket Analysis
- Low credit limit customers (<50K) showed higher default rates
- High credit limit customers are generally lower risk

### 4. Age Group Analysis
- Age doesn't show much effecct on the default rate

### 5. Education Level
- High school educated customers had higher default rates
- Graduate school customers were the most reliable segment

## Business Recommendation
> Customers showing even a single month of payment delay should be 
> flagged immediately as high risk. A two month delay is a strong 
> predictor of default with 69% probability.

**For credit card targeting:**
- ✅ Target: High credit limit + on-time payment history + graduate/university educated
- ❌ Avoid: Payment delay ≥ 1 month + low credit limit + young age group

## SQL Queries
All queries used in this analysis are available in the `/queries` folder.

## Dashboard
Power BI dashboard screenshot available in the `/dashboard` folder.

## Author
**Riya**
[LinkedIn Profile](https://www.linkedin.com/in/riya-saini-05a4ab215/)
