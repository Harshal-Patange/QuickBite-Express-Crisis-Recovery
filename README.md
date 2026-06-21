<div align="center">

# 🍔 QuickBite Express — Crisis Recovery Dashboard

### Providing Insights for a Crisis Recovery to an Online Food Delivery Startup


[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com)
[![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](#)
[![Excel](https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white)](#)
[![Status](https://img.shields.io/badge/Status-Completed-27AE60?style=for-the-badge)](#)
[![Challenge](https://img.shields.io/badge/Codebasics-RPC%2318-E74C3C?style=for-the-badge)](https://codebasics.io)

</div>

---

## 📖 Table of Contents

- [Problem Statement](#-problem-statement)
- [Live Dashboard](#-live-dashboard)
- [Tech Stack](#-tech-stack)
- [Dataset Overview](#-dataset-overview)
- [Dashboard Pages](#-dashboard-pages)
- [Key Insights](#-key-insights)
- [Primary Analysis](#-primary-analysis---10-questions-answered)
- [Secondary Analysis](#-secondary-analysis)
- [Recovery Strategy](#-recovery-strategy---3r-framework)
- [Project Structure](#-project-structure)
- [How to Use](#-how-to-use)
- [Credits](#-credits)

---

## 📌 Problem Statement

**QuickBite Express** is a Bengaluru-based food-tech startup (founded 2020) that
connects customers with nearby restaurants and cloud kitchens across 8 major Indian cities.

### 🚨 The Crisis — June 2025

In June 2025, QuickBite faced a perfect storm of challenges:

| Crisis Factor | Impact |
|--------------|--------|
| 🦠 Viral food safety incident on social media | Massive customer backlash |
| 🌧️ Week-long delivery outage during monsoon | Service completely disrupted |
| ⚔️ Competitors launched aggressive campaigns | Market share loss |
| 📉 Customer trust collapsed overnight | Ratings dropped sharply |

### 🎯 Management Expectations

> As **Peter Pandey** (Data Analyst at QuickBite), I was tasked with analysing the
> crisis impact across 6 key areas and providing actionable recovery insights:

1. **Customer Segments** — Who can be recovered vs needs new strategy
2. **Order Patterns** — Behavioral changes across pre-crisis, crisis, recovery
3. **Delivery Performance** — SLA compliance and operational gaps
4. **Campaign Opportunities** — Targeted trust-rebuilding initiatives
5. **Restaurant Partnerships** — Most valuable partners for long-term retention
6. **Feedback & Sentiment** — Real-time monitoring to guide recovery

---

## 🔴 Live Dashboard

<div align="center">

| Resource | Link |
|----------|------|
| 📊 Power BI File (.pbix) | [https://drive.google.com/drive/folders/1ZGWaQeubpqqyapx6Qfn7gpzB1JX6dAHi]|

</div>

---

## 💻 Tech Stack

```
📊 Power BI    → 5-page interactive dashboard · 100+ visuals · DAX measures
🗄️  SQL        → CTE queries · 10 primary analysis questions answered
📋 Excel       → Data cleaning · pivot analysis · summary tables
```

---

## 🗄️ Dataset Overview

**Data Period:** January 2025 — September 2025
**Phase Labels:**
- 🟢 **Pre-Crisis** → Jan–May 2025 (5 months)
- 🔴 **Crisis** → Jun–Sep 2025 (4 months)

| Table | Rows | Description |
|-------|------|-------------|
| `fact_orders` | 1,49,166 | All orders with status, revenue, timestamps |
| `fact_ratings` | 68,843 | Customer ratings & review text + sentiment |
| `fact_delivery_performance` | 1,49,167 | Actual vs expected delivery times |
| `fact_order_items` | 3,42,995 | Item-level order breakdown |
| `dim_customer` | 1,07,777 | Customer profiles & acquisition channel |
| `dim_restaurant` | 19,996 | Restaurant details & partner type |
| `dim_delivery_partner` | 15,000 | Delivery partner profiles |
| `dim_menu_item` | 3,42,672 | Menu item catalogue |

**8 Cities Covered:**
Bengaluru · Mumbai · Delhi · Hyderabad · Chennai · Pune · Kolkata · Ahmedabad

---

## 📊 Dashboard Pages

### Page 1 — Executive Summary
<img width="485" height="277" alt="{49A09E7A-2BD4-48DB-8225-6DC9DF3A24D7}" src="https://github.com/user-attachments/assets/691f37b8-cc91-4732-be16-29075d8091a9" />

> **Purpose:** First view for leadership — instant snapshot of crisis severity

**Visuals included:**
- 4 KPI Cards with delta labels — Orders · Revenue · Rating · Cancellation
- Monthly Order Trend line chart (crisis months highlighted in red)
- Revenue by Phase waterfall comparison
- Top 5 Cities order decline bar chart
- Customer Loyalty donut chart
- Key Insights summary text box (3 bullet points)
- Avg Order Value stability chart

---

### Page 2 — Orders & City Analysis
<img width="484" height="277" alt="{232743D5-5E9A-4EDC-B69D-976510DE906E}" src="https://github.com/user-attachments/assets/e423bb5f-07a0-4514-972c-8f30ec81124f" />

> **Purpose:** Deep dive into where and how much orders declined

**Visuals included:**
- Orders by City — Pre vs Crisis grouped bar chart
- City Decline % ranked horizontal bar (all 8 cities)
- Cloud Kitchen vs Dine-in comparison
- Order Recovery Funnel (Pre-Crisis → Crisis)
- Order Loss by City map/treemap

---

### Page 3 — Delivery & Operations
<img width="486" height="275" alt="{C4C1D060-2F6E-4561-905A-E0E44061BF90}" src="https://github.com/user-attachments/assets/47463206-7b0d-4119-80da-73fca3e878d9" />

> **Purpose:** Identify operational failures that worsened the crisis

**Visuals included:**
- 4 KPI Cards — Delivery time & SLA compliance (pre vs crisis)
- Actual vs Expected Delivery Time line chart
- Monthly Cancellation Rate trend
- Cancellation Rate by City comparison
- SLA Compliance by City bar chart

---

### Page 4 — Customer & Loyalty Health
<img width="486" height="277" alt="{39451775-431A-445E-AD79-7F7FE24D5063}" src="https://github.com/user-attachments/assets/ff321c7e-0260-4ed3-b89b-213098208866" />


> **Purpose:** Identify which customers churned and who to win back first

**Visuals included:**
- 4 KPI Cards — Loyal · Churned · High-rated churned · Rating drop
- Monthly Avg Rating trend (sharpest drop = June)
- Loyalty Churn Funnel (87K → 73K → 19K)
- Rating Distribution shift (pre vs crisis)
- Churned Customers by City

---

### Page 5 — Sentiment & Recovery
<img width="486" height="274" alt="{F1AF5D2B-BDFA-4E47-A49F-AEF5CA0F1D0F}" src="https://github.com/user-attachments/assets/c795d6a0-486c-4539-b893-59d318b94579" />

> **Purpose:** What are customers saying and what actions to take

**Visuals included:**
- Positive vs Negative Review % by month
- Top Complaint Keywords (Treemap)
- Review Count by Sentiment Type
- Recovery Roadmap — 3R Strategy action cards

---

## 🔑 Key Insights

<table>
<tr>
<td width="50%">

### 📉 Crisis Impact
- Orders dropped **61%** in June 2025
- Revenue fell **₹3.4 Crore** in crisis period
- Avg rating collapsed **4.5 → 2.5** in June
- Cancellation spiked to **14%** (was 4% pre-crisis)
- Delivery time increased **52%** (39min → 60min)

</td>
<td width="50%">

### 👥 Customer Impact
- **87K** loyal customers identified pre-crisis
- **73K** (84%) churned completely in crisis
- **19K** high-rated churned = win-back targets
- Bengaluru and Mumbai most affected cities
- Rating drop was sharpest in **June 2025**

</td>
</tr>
<tr>
<td width="50%">

### 🚚 Operations Impact
- SLA compliance dropped **43.6% → 12.2%**
- All 8 cities saw delivery time worsen
- Bengaluru had worst SLA at **36.67%**
- Cancellation spiked across all cities in June
- Cloud Kitchens hit harder than Dine-in restaurants

</td>
<td width="50%">

### 💬 Sentiment Impact
- Positive reviews dropped **100% → 11%** in June
- Negative reviews spiked **0% → 86%** in June
- Top complaint — **Late delivery (92%)**
- Sentiment collapse aligns perfectly with outage week
- Avg order value remained **stable at ₹350** (frequency not value was issue)

</td>
</tr>
</table>

---

## ✅ Primary Analysis — 10 Questions Answered

| # | Question | Finding | Page |
|---|----------|---------|------|
| 1 | Monthly orders — pre vs crisis severity | **61% drop** — 23K/month → 9K/month | Page 1 |
| 2 | Top 5 cities by % order decline | Bengaluru (70.2%) leads decline | Page 2 |
| 3 | Top 10 restaurants with largest decline (≥50 orders) | All top restaurants lost 85-94% orders | Page 2 |
| 4 | Cancellation rate trend by city | Spiked from **4% → 14%** in all cities | Page 3 |
| 5 | Delivery SLA compliance | Dropped from **43.6% → 12.2%** in crisis | Page 3 |
| 6 | Monthly avg rating fluctuation | Sharpest drop in **June 2025 (4.5→2.5)** | Page 4 |
| 7 | Negative keywords in crisis reviews | Late delivery · Cold food · Cancelled · No refund | Page 5 |
| 8 | Revenue impact pre vs crisis | **₹3.4 Crore lost** — pre ₹38M vs crisis ₹11M | Page 1 |
| 9 | Loyal customers who churned | **73K churned** out of 87K loyal (84%) | Page 4 |
| 10 | High-value customer lifetime decline | Top spenders showed **84% churn rate** | Page 4 |

---

## 🔍 Secondary Analysis

### Q1 — Competitor Comparison (Swiggy / Zomato)

During June–September 2025, while QuickBite suffered a **61% order decline**,
competitors Swiggy and Zomato capitalized aggressively:

- Launched **"Safety Guaranteed"** campaign targeting QuickBite's food safety incident
- Offered **₹0 delivery fee** promotions in Bengaluru and Mumbai
- Onboarded displaced QuickBite restaurant partners with better commission rates
- Ran targeted social media ads to QuickBite's churned customer segments

> **Impact:** Customer acquisition costs at QuickBite tripled as they had to
> compete against funded competitor campaigns while managing reputation damage.

---

### Q2 — External Factors Behind CAC Tripling

| Factor | Impact on CAC |
|--------|--------------|
| 🌧️ Monsoon season | Higher delivery costs → less new sign-ups |
| 📱 Viral social media incident | Paid PR campaigns required to counter negative press |
| ⚔️ Competitor ad spending | Higher bid prices on Google/Meta ads in food delivery |
| 😡 Trust deficit | More touchpoints needed before new customer converts |
| 🔄 Churned user re-acquisition | Win-back campaigns cost 3x more than new acquisition |

---

### Q3 — Trust Rebuild Strategies ✅ (Answered in Dashboard)

Covered in **Page 5 — Recovery Roadmap:**

| Strategy | Action | Expected Impact |
|----------|--------|----------------|
| Food safety audit badges | Display on all restaurant listings | Rebuilds 60% of lost trust |
| SLA delivery guarantee | Refund if delivery exceeds 45 mins | Reduces cancellation rate |
| Partner quality scoring | Public restaurant health scores | Reduces churn risk |
| Customer communication | Proactive email/SMS outreach | Re-engagement rate 25% |

---

### Q4 — Restaurant Type Churn ✅ (Answered in Dashboard)

From **Page 2 — Cloud Kitchen vs Dine-in analysis:**

- **Cloud Kitchens** showed higher churn — no physical presence, harder to trust post safety incident
- **Dine-in Restaurants** retained more customers — brand visibility and walk-in trust factor
- **Small brands** (< 100 monthly orders) churned fastest — no loyal customer base to retain
- **Large branded restaurants** survived better — existing brand equity cushioned the blow

---

### Q5 — Win-Back Probability ✅ (Answered in Dashboard)

From **Page 4 — Loyalty Churn Funnel:**

```
Priority 1 → 19K high-rated churned customers (rating > 4.5 pre-crisis)
             These were SATISFIED before crisis — most likely to return
             Recommended offer: 30% cashback on first 3 comeback orders

Priority 2 → Churned customers from Bengaluru & Mumbai
             Highest volume cities — biggest revenue recovery potential
             Recommended offer: Free delivery for 30 days

Priority 3 → Customers who churned in July (not June)
             Gave QuickBite a second chance after June — higher loyalty signal
             Recommended offer: Loyalty points double for 60 days
```

---

### Extra — Priority Cities for Long-term Demand Loss

Based on **Page 2 City Analysis:**

| City | Decline % | Risk Level | Priority |
|------|-----------|-----------|----------|
| Bengaluru | 70.23% | 🔴 Critical | 1 |
| Mumbai | 70.18% | 🔴 Critical | 2 |
| Ahmedabad | 69.89% | 🟡 High | 3 |
| Pune | 69.81% | 🟡 High | 4 |
| Delhi | 69.81% | 🟡 High | 5 |

---

### Extra — Behavior Shift (Survival Orders)

> **Finding:** Avg Order Value remained **stable at ₹350-353** across ALL months
> including crisis. This proves customers did NOT shift to survival/low-value orders.
> The crisis impact was on **ORDER FREQUENCY** not spending per order.
> Insight: When customers returned, they spent the same — just ordered less often.

---

### Extra — Feedback vs Delivery Outage Alignment

> **Finding:** Page 5 sentiment analysis shows negative reviews spiked from
> near-zero to **86%** exactly in June 2025 — perfectly aligned with the
> delivery outage week. This confirms the outage was the **primary trigger**
> of the sentiment collapse, not the food safety incident alone.

---

## 🎯 Recovery Strategy — 3R Framework

```
╔══════════════════════════════════════════════════════════╗
║                   3R RECOVERY FRAMEWORK                  ║
╠══════════════════════════════════════════════════════════╣
║                                                          ║
║  🔵 RETAIN — Stop the bleeding (immediate)               ║
║     → Cashback offers for active customers               ║
║     → Double loyalty points for 60 days                  ║
║     → Free delivery on next 5 orders                     ║
║                                                          ║
║  🟡 RECOVER — Win back churned customers (30-60 days)    ║
║     → Target 19K high-rated churned customers first      ║
║     → Personalised win-back campaign with 30% discount   ║
║     → Re-engagement email/SMS sequence (7-day drip)      ║
║                                                          ║
║  🟢 REBUILD — Restore brand trust (60-180 days)          ║
║     → Food safety certification badges on all listings   ║
║     → SLA delivery guarantee with auto-refund            ║
║     → Partner quality audits across all 8 cities         ║
║     → Influencer partnerships for social media repair     ║
║                                                          ║
╚══════════════════════════════════════════════════════════╝
```
---

## 🚀 How to Use

### View the Dashboard
1. Download the `.pbix` file from [Google Drive](your-google-drive-link)
2. Open with **Power BI Desktop** (free download from Microsoft)
3. Navigate between 5 pages using the top navigation bar
4. Use **Phase slicer** to filter between Pre-Crisis and Crisis

### Run the SQL Queries
1. Load all 8 CSV files into your SQL database
2. Open `SQL/QuickBite_SQL_Queries.sql`
3. Run queries in order — each query answers one primary analysis question
4. All queries use CTEs for easy readability

### Explore the Dataset
1. All 8 CSV files available in `/Dataset` folder
2. Data covers January 2025 to September 2025
3. Phase column — Pre-Crisis (Month 1-5) · Crisis (Month 6-9)

---

## 📊 Results Summary

```
Before Crisis (Jan-May 2025)    After Crisis (Jun-Sep 2025)
─────────────────────────────   ─────────────────────────────
Orders/month:  ~23,000          Orders/month:  ~9,000  (-61%)
Revenue:       ₹38 Million      Revenue:       ₹11 Million (-71%)
Avg Rating:    4.5 / 5.0        Avg Rating:    2.5 / 5.0  (-2.0)
Cancel Rate:   4.2%             Cancel Rate:   14.0%      (+10%)
Delivery SLA:  43.6%            Delivery SLA:  12.2%      (-31%)
Positive Rev:  ~100%            Positive Rev:  ~11%       (-89%)
```

---

## 🙏 Credits & Acknowledgements

- **Challenge:** [Codebasics.io](https://codebasics.io) — Resume Project Challenge #18
- **Domain:** Food Delivery & Consumer Analytics
- **Function:** Crisis Recovery & Business Strategy
- **Dataset:** Provided by Codebasics team

---

<div align="center">

### 💡 What I Learned

```
Power BI DAX measures · CTE SQL queries · Crisis analytics
Customer churn analysis · Sentiment analysis · Recovery strategy
Data storytelling · Dashboard design · Business insights
```

---

⭐ **If you found this project helpful or insightful, please give it a star!**

https://github.com/Harshal-Patange/QuickBite-Express-Crisis-Recovery

**Made with ❤️ by Harshal Patange**

</div>
