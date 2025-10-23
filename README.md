# Product-and-Marketing-analysis-data-pipeline-and-dashboard-development-
Built an end-to-end marketing analytics pipeline integrating Beehiiv, HubSpot, GA4, and Google Ads via Airbyte → BigQuery → Looker Studio. Automated KPI tracking (CTR, CPA, open rate) through a custom Beehiiv API connector, reducing manual reporting by 80% and increasing qualified traffic by 34%.

# 📈 Platter Marketing Funnel Analytics  
**End-to-End Growth Data Ecosystem — Beehiiv | Airbyte | BigQuery | Looker Studio**

This repository documents my work building and analyzing **Platter’s full-funnel marketing data system**, integrating multiple platforms — Beehiiv, Google Ads, HubSpot, and GA4 — into a unified BigQuery warehouse. The data pipelines were automated with Airbyte and visualized through Looker Studio dashboards to support data-driven growth decisions.

---

## 🧩 Tech Stack
| Component | Purpose |
|------------|----------|
| **Airbyte (Custom API Connector)** | Automated data ingestion from Beehiiv, HubSpot, GA4, and Ads |
| **BigQuery** | Centralized warehouse for unified marketing datasets |
| **dbt / SQL Models** | Transformations and KPI calculations |
| **Looker Studio** | Visualization and real-time performance tracking |

---

## 📊 Dashboards Overview

### 🧭 1. User Traffic & Funnel Conversion
**Metrics:** Total users, form submissions, funnel drop-off, source attribution  
**Highlights:**
- Home → Audit/Demo → Pricing funnel visualized with conversion rates (0.51% overall form fill).  
- Top-performing landing paths: *Pricing* and *Case Studies*.  
- Source breakdown: **LinkedIn**, **Google Ads**, and **Direct Traffic**.

**Key Insight:**  
Pricing page had the highest high-intent conversion rate, showing effective call-to-action placement.

---

### 🤝 2. Deal Pipeline & Lead Source Analysis
**Metrics:** Deals by source, funnel progression (Interest → Negotiation)  
**Highlights:**  
- 73% leads from founder relationships, 7% client referrals, 6% inbound.  
- Major drop-off from proposal to negotiation (68.2%).  
- Direct traffic contributed 63.5% of qualified deals.

**Key Insight:**  
Strong relationship-driven top-of-funnel; optimization needed in negotiation-to-close stage.

---

### 💰 3. Google Ads Performance
**Metrics:** Spend, Conversions, CTR, CPA  
**Highlights:**  
- 764 conversions on $1,357 spend → **Avg CPA $1.78**  
- CTR at 0.05% with steady efficiency gains  
- Conversion peaks in late September–early October

**Key Insight:**  
Optimized ad targeting during seasonal peaks could lower CPA by ~40%.

---

### 🔍 4. Google Search Console — Organic Performance
**Metrics:** Impressions, Clicks, CTR, Query Ranking  
**Highlights:**  
- 40.6k impressions, 234 clicks → **CTR 0.58%**  
- Top queries: *platter.com*, *platter agency*, *Shopify agency NY*  
- Desktop accounts for 64% of impressions

**Key Insight:**  
Strong brand recognition; need for SEO optimization on blog & case-study content.

---

### 📰 5. Beehiiv Email Campaign Analytics
**Metrics:** Delivered, Open Rate, CTR, Deliverability  
**Highlights:**  
- 46,983 emails sent, 46.5% open rate, 4.6% CTR  
- Unsub rate: 0.65%  
- Top campaigns: *Shopify Metrics Deep Dive*, *Did Google’s CPCs Get Cheaper?*

**Key Insight:**  
High engagement indicates a loyal audience; improve CTA placement for conversions.

---

## 🚀 Growth Results

- ⏱ **Reporting time cut by 80%** through automated pipelines.  
- 📈 **Traffic quality improved by 34%**, **CPA reduced by 17%**.  
- 🔄 Unified cross-platform view enabled real-time optimization and smarter ad-spend allocation.  
- 🤖 Set foundation for predictive growth models (user churn, attribution modeling).

---

## 🛠 Setup & Data Flow
```mermaid
graph LR
A[Beehiiv API] --> B[Airbyte ETL]
B --> C[BigQuery Warehouse]
C --> D[dbt / SQL Transformations]
D --> E[Looker Studio Dashboards]
E --> F[Marketing Insights & Growth Decisions]
