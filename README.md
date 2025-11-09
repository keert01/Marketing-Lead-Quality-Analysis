# Marketing-Lead-Quality-Analysis

# 🎯 Marketing Lead Quality & Campaign Optimization Analysis

## 🌍 Overview

This project simulates a **real-world marketing campaign analysis** where a data analyst investigates the following business questions:

1️⃣ Are we observing any **lead quality trends over time** — improving or declining?  
2️⃣ What are the **key drivers** that influence lead quality (placement, channel, ad design, or audience)?  
3️⃣ If lead quality improves by 20%, how could that affect **Cost per Lead (CPL)** and revenue performance?

Using **Python** for data preparation and **Power BI** for visualization, this project replicates the workflow of an end-to-end marketing analytics case study — from raw data to actionable insights.

---

## ⚙️ Project Flow

### 🧹 1. Data Cleaning & Preparation (Python)
- Standardized and validated lead-level data (dates, duplicates, nulls).
- Segmented leads into **custom quality buckets**: High → Low.
- Derived new columns from ad creative fields:
  - Widget type, color, design, and size for A/B testing.
- Normalized campaign and referral sources.
- Created audit logs to maintain full **data lineage transparency**.

### 📊 2. Analytical Transformations
- Built **Weekly & Monthly trend tables** with rolling averages.
- Developed **driver-level summary tables** for:
  - Ad Placement & Design  
  - Channel & Campaign  
  - User Intent & Engagement Context
- Calculated KPIs:
  - Weighted Quality Index (WQI)
  - % of High-Quality Leads
  - Lead Quality Elasticity
  - Rolling averages and anomaly tracking

### 🧠 3. Insights & Visualization (Power BI)
Interactive Power BI Dashboard includes:
- 🟦 **KPI Cards:** Total Leads, Avg Quality, % High Quality, and Gap to Target  
- 📈 **Trendline:** Monthly Lead Quality (WQI)  
- 🔍 **Category Analysis:** Avg Quality by key segments — channel, ad design, campaign type, etc.  
- 🧩 **Opportunity Map:** Total Leads vs Lead Quality — identifies “High Volume + Low Quality” focus areas  
- 🌅 **Weekend vs Weekday Comparison:** Detects behavioral impact on lead quality  

---

## 📈 Project Outcomes

✔️ Discovered non-linear fluctuations in lead quality — overall stable but with opportunity areas in Q2 months.  
✔️ Found **Branded Campaigns** outperform Generic by ~7% in average lead quality.  
✔️ Online form leads were more consistent than call-center-acquired leads.  
✔️ Creative elements (e.g., *BlueMeter* and *Head2* designs) correlated with higher conversion quality.  
✔️ Weekend leads showed slightly higher engagement — indicating behavioral variance worth testing.

---

## 💡 Dashboard Preview

### **Power BI Report Overview**
<img width="1277" height="733" alt="image" src="https://github.com/user-attachments/assets/f920f721-970e-4664-a6da-e8e39a8a6fb4" />

*(If viewing locally, refer to `LeadQuality_PowerBIDashboard.pdf` for the full layout.)*

---

## 🧰 Tech Stack & Libraries

| Purpose | Tools / Libraries Used |
|----------|------------------------|
| **Data Wrangling** | Python (`pandas`, `numpy`) |
| **Visualization (EDA)** | `matplotlib`, `seaborn` |
| **Statistical Testing** | `scipy.stats` |
| **Reporting & Dashboarding** | Power BI |
| **Audit & Logs** | `datetime`, custom log tables |

---

## 🧮 Key KPIs & Metrics
- **WQI (Weighted Quality Index)** = Mean Lead Quality Score  
- **% High Quality** = Leads tagged “High” or “Medium-High”  
- **Opportunity Index** = High Quality % ÷ Total Leads  
- **Lead Quality Lift (Target)** = 20% increase scenario modeled

---

## 🚀 Future Enhancements
- Automate pipeline via **Airflow or Prefect**.  
- Integrate **predictive modeling** to estimate CPL uplift under different quality-improvement strategies.  
- Add **real-time connectors** from marketing APIs (Google Ads, Meta Ads).  
- Expand Power BI visuals with region and keyword-level deep dives.

---
## 🗂 Repository Structure
Marketing_Lead_Quality_Analysis/
│
├── cleaned_leads_dataset.xlsx # Processed dataset
├── Driver_Summary_Tables.xlsx # Driver-level aggregations
├── LeadQuality_PowerBIDashboard.pdf # Power BI report snapshot
├── visuals/
│ ├── monthly_trend.png
│ ├── lead_quality_comparison_earlyrecent.png
│ ├── lead_quality_score_dayofweek.png
│ ├── category_impact.png
│ └── opportunity_map.png
└── README.md


---

## ✨ Summary

This project demonstrates how a data analyst can:
- Clean and structure marketing campaign data for lead-quality insights  
- Build trend and segmentation-based KPIs  
- Translate analysis into a **visual storytelling dashboard** that drives business decisions  

> 📌 **End Result:** Actionable insights for optimizing campaign performance and improving CPL through lead quality enhancement.

---


