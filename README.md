# 📉 Telco Customer Retention & Churn Analysis

An end-to-end data analytics project analyzing telecom customer behavior to identify churn patterns, retention drivers, and high-risk customer segments using **Python** and **Power BI**.

---

## 📌 Overview

This project analyzes a real-world telecom dataset to help a subscription-based business understand why customers leave, which segments are most at risk, and what actions can improve retention. The analysis mirrors actual work done by data analysts in product, growth, and retention teams.

---

## 🎯 Business Questions Answered

- Why are customers leaving the platform?
- Which customer segments are most likely to churn?
- How long do customers typically stay active?
- What contract types and payment methods drive churn?
- Which customers are at high risk of churning?
- What actions can improve customer retention?

---

## 📁 Dataset

- **Source:** [Kaggle — Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)
- **Size:** 7,043 customers | 21 features
- **Coverage:** Telecom subscription data including contract type, tenure, charges, and services

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Python (Pandas) | Data cleaning, feature engineering, risk segmentation |
| Power BI | Dashboard design, DAX measures, interactive visuals |

---

## 📊 Dashboard Preview

### Page 1 — Churn Overview
![Churn Overview](screenshots/page1_churn_overview.png)

### Page 2 — Retention & Risk Analysis
![Retention Analysis](screenshots/page2_retention_risk.png)

---

## 🔑 Key Findings

| Metric | Value |
|---|---|
| Total Customers | 7,043 |
| Overall Churn Rate | 26.54% |
| Average Tenure | 32.37 months |
| Average Monthly Charges | $64.76 |
| High Risk Customers | 1,994 |
| Senior Citizen Churn Rate | 41.68% |
| Retention Rate | 73.46% |

- **Month-to-month contracts** have the highest churn rate (~42%) vs only ~3% for two-year contracts
- Customers in the **0-12 month** tenure group churn at ~48% — the most critical retention window
- **Electronic check** payment method has the highest churn at 57.3% of all churned customers
- **Fiber optic** internet service customers churn at 42% vs 19% for DSL
- Churned customers pay on average **~$20 more per month** than retained customers at every tenure stage
- **Senior citizens** churn at 41.68% — nearly double the non-senior rate of ~23%

---

## 💡 Recommendations

1. **Target month-to-month customers** with incentives to switch to annual contracts — this alone could cut churn significantly
2. **Focus retention efforts on 0-12 month customers** — nearly half churn in the first year; onboarding improvements are critical
3. **Investigate Fiber optic pricing** — 42% churn rate suggests dissatisfaction with value vs cost
4. **Offer payment method alternatives** to electronic check users — they show the highest churn
5. **Create a Senior citizen retention program** — tailored support and simpler plans could reduce their 41.68% churn rate
6. **Flag high-risk customers early** — 1,994 customers are classified as high risk; proactive outreach could save significant revenue

---

## 🔧 Feature Engineering (Python)

| New Column | Description |
|---|---|
| `Churn_Flag` | Binary 1/0 instead of Yes/No |
| `SeniorCitizen_Label` | "Senior" / "Non-Senior" readable label |
| `Tenure_Group` | 6 groups: 0-12, 13-24, 25-36, 37-48, 49-60, 61+ Months |
| `Charge_Segment` | Low / Medium / High / Very High based on monthly charges |
| `Num_Services` | Count of active services per customer |
| `Risk_Segment` | High / Medium / Low / Very Low Risk based on contract and tenure |

---

## 🛠️ Skills Demonstrated

- Data cleaning and transformation with **Pandas**
- Feature engineering and customer segmentation
- **DAX measures** in Power BI
- Multi-page dashboard design with navigation
- Business storytelling through data visualization
- Domain knowledge in **SaaS/Subscription churn analytics**

