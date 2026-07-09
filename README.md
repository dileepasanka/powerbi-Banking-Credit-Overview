# Bank Credit Review & Risk Analysis Dashboard

## 📌 Project Overview
An interactive 8-page Power BI dashboard designed for commercial banking executives and risk managers. It transforms raw loan transaction data into actionable insights to monitor portfolio health, track credit risk exposure, and evaluate regional branch performance.

---

## 📊 Dashboard Previews
Below are the individual pages tracking different aspects of the lending portfolio:

### 1. Landing Page

### 2. Portfolio Overview

### 3. Credit Risk & Quality Analysis

### 4. Regional & Branch Performance

### 5. Active Portfolio by Loans Status

### 6. Total Portfolio Drill Down

### 7. Bookmark & Selection (Tables & Visuals)

### 8. Data Quality & Findings

---

## 🔍 Key Capabilities
* **Portfolio Health Tracking:** Immediate breakdown of active vs. distressed loan values.
* **Risk Evaluation:** Real-time monitoring of non-performing loans (NPLs) and provisions to catch asset degradation early.
* **Regional Analytics:** Deep dive into branch efficiency to identify high-revenue regions vs. high-default zones.
* **Data Integrity Audit:** A dedicated page tracking data quality gaps, outliers, and system anomalies to ensure reporting accuracy.

---

## 📈 Core KPIs Monitored
* **Asset Quality:** Total Active Portfolio Outstanding, Total Disbursed Amount, and Portfolio at Risk (PAR %).
* **Risk Concentrations:** Non-Performing Loans (NPL) Ratio, Provision Coverages, and Past-Due buckets (30/60/90+ days).
* **Operational Performance:** Average Loan Size, Interest Yield Spreads, and Branch Tiers.

---

## 🎯 Business Value
1. **Protects Capital:** Early warnings on worsening PAR % allow risk officers to adjust lending criteria before losses occur.
2. **Optimizes Resources:** Pinpoints which branches are over-performing or accumulating toxic debt.
3. **Ensures Compliance:** The Data Quality section highlights data gaps before internal or regulatory audits find them.
4. **Enhanced UX:** Uses Power BI bookmarks and custom toggles to let users switch seamlessly between executive charts and granular data grids.

---

## 🛠️ Tech Stack & Methodology

### 1. Data Modeling
* **Star Schema Architecture:** Enforces clean separation between central Fact tables (Loans, Balances) and Dimension tables (Branches, Customers, Calendar, Products).
* **Performance Optimization:** Built with strict single-direction filters to maximize DAX storage engine efficiency.
* **Time Intelligence:** Integrated a dedicated Date table to calculate flawless Month-over-Month (MoM) and Year-to-Date (YTD) metrics.

### 2. Core DAX Measures
* **Active Portfolio Value:**
  ```dax
  Total Active Portfolio = 
  CALCULATE(
      SUM('Fact_Loans'[Outstanding_Balance]),
      'Dim_Loan_Status'[Status_Group] = "Active"
  )
