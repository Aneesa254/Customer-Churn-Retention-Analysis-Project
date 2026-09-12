# Telco Customer Churn Analysis

Data analysis project (Task 4) exploring customer churn patterns in a telecom dataset — identifying key churn drivers, validating them statistically, segmenting customers by risk, and translating findings into business recommendations.

## 📌 Overview

Customer churn — the rate at which customers stop using a service — is one of the most expensive problems in subscription-based businesses. This project analyzes 7,043 telecom customer records to answer:

- What factors are most strongly associated with churn?
- Are these associations statistically significant, or could they be due to chance?
- Which customer segments are most at risk, and how much revenue is at stake?
- What actions should the business take to reduce churn?

## 📊 Key Results

| Metric | Value |
|---|---|
| Total Customers | 7,043 |
| Churned Customers | 1,869 |
| Churn Rate | 26.54% |
| Avg. Monthly Charges | $64.76 |
| Revenue at Risk | $139,130.85 / month |

**Highest-risk segment:** *High-Risk* customers (new + expensive plans) — 880 customers churning at **68.07%**, nearly 3x the overall rate.

## 🔬 Methodology

1. **Data Cleaning & EDA** — inspected the dataset, handled missing/invalid values, explored churn distribution across categorical and numerical features.
2. **Statistical Testing**
   - **Chi-Square Test of Independence** — tested whether contract type and churn are associated (χ² = 1184.60, p < 0.001).
   - **Independent Samples T-Test** — tested whether monthly charges differ significantly between churned and retained customers (t = 18.41, p < 0.001).
3. **Rule-Based Customer Segmentation** — grouped customers by tenure and monthly charges (not churn itself) into four segments: High-Risk, New, High-Value, and Loyal, then measured churn rate as an outcome for each.
4. **Dashboard** — built an interactive Power BI dashboard to visualize churn by contract, tenure, payment method, and customer segment.
5. **Reporting** — summarized findings, statistical results, and recommendations into a one-to-two-page executive summary.

## 📁 Repository Contents

| File | Description |
|---|---|
| `Task4_Customer_Churn_Analysis.ipynb` | Jupyter notebook with data cleaning, EDA, statistical tests, and segmentation logic |
| `Task4_Churn_Dashboard.pbix` | Power BI interactive dashboard |
| `Task4_Final_Summary.docx` / `.pdf` | Executive summary: findings, statistical results, segments, revenue at risk, and recommendations |
| `README.md` | This file |

## 🖥️ Dashboard Preview

The Power BI dashboard includes:
- KPI cards (total customers, churn rate, revenue at risk)
- Churn rate by contract type, tenure group, and payment method
- Average monthly charges: churned vs. retained
- Churn rate by customer segment
- Slicers for Contract, Internet Service, and Payment Method

## 💡 Recommendations

1. Incentivize longer-term contracts for Month-to-month customers.
2. Build a structured first-year onboarding/check-in program.
3. Review Fiber optic pricing and add loyalty/bundle perks.
4. Nudge Electronic check users toward automatic payment methods.
5. Proactively offer Tech Support, prioritizing the 880 High-Risk customers.

## 🛠️ Tools Used

- Python (pandas, scipy, matplotlib/seaborn) for data analysis and statistical testing
- Jupyter Notebook
- Power BI for dashboarding
- Microsoft Word for reporting

## 📂 Dataset

Telco Customer Churn dataset (IBM sample dataset), containing 7,043 customer records with demographic, account, and service usage attributes.

---
