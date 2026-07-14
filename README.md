# 🏦 Power BI – Bank Credit & Risk Overview Dashboard

An interactive, 8-page Power BI dashboard built for commercial banking teams to monitor loan portfolio health, credit risk exposure, and branch-level performance — turning raw loan and transaction data into a single, decision-ready view for executives and risk officers.

---

## 📌 Project Overview

Banks generate enormous volumes of loan, repayment, and branch data — but raw transaction tables don't tell a story on their own. This dashboard consolidates that data into a guided, executive-ready report that answers the questions credit and risk teams ask daily: *How healthy is the portfolio? Where is risk concentrated? Which branches are performing, and which need attention?*

Built entirely in **Power BI Desktop**, the report reflects real banking domain knowledge — combining credit risk analysis experience with hands-on Power BI development, from data modeling through to executive-level visual storytelling.

---

## 🧭 Report Pages

The `.pbix` file contains eight connected pages, each built around a specific banking use case:

### 1. Landing Page
Entry point with navigation and a high-level snapshot of the portfolio before drilling into detail.

### 2. Portfolio Overview
Executive summary of the lending book — total disbursed amount, active portfolio outstanding, and overall portfolio composition.

### 3. Credit Risk & Quality Analysis
Tracks Non-Performing Loans (NPL), Portfolio at Risk (PAR %), and past-due buckets (30/60/90+ days) to flag deteriorating asset quality early.

### 4. Regional & Branch Performance
Compares branches and regions side by side to identify high-performing locations versus areas with rising default risk.

### 5. Active Portfolio by Loan Status
Breaks the live portfolio down by loan status, showing exactly where outstanding balances currently sit.

### 6. Total Portfolio Drill Down
Lets users move from summary numbers down to granular, transaction-level detail without leaving the report.

### 7. Bookmark & Selection (Tables & Visuals)
Regional loan distribution and occupation-wise NPL ratio, with **Tables** and **Visuals** bookmark buttons that instantly toggle the same data between chart view and table view — no page reload needed.

### 8. Data Quality & Findings
A dedicated audit page surfacing data gaps, outliers, and anomalies — built to catch issues before internal or regulatory review does.

---

## ✨ Key Features

- **Star schema data model** — clean separation between fact tables (loans, balances) and dimension tables (branches, customers, calendar, products) for fast, reliable performance.
- **Time intelligence** — a dedicated Date table powering accurate Month-over-Month (MoM) and Year-to-Date (YTD) trend calculations.
- **Custom DAX measures** — purpose-built calculations for NPL ratio, PAR %, provision coverage, and average loan size.
- **Bookmarks & interactive navigation** — one-click switching between high-level charts and detailed tables.
- **Built-in data quality checks** — a dedicated page that treats data integrity as part of the reporting process, not an afterthought.

---

## 🗂️ Repository Contents

| File | Description |
|---|---|
| `Bank Credit Overview.pbix` | The full Power BI report — open in Power BI Desktop to explore live. |
| `1.Landing Page.png` | Screenshot of the report's home/overview page. |
| `2.Portfolio Overview.png` | Screenshot of the executive portfolio summary page. |
| `3.Credit Risk & Quality Analysis.png` | Screenshot of the risk and NPL tracking page. |
| `4.Regional & Branch Performance.png` | Screenshot of the branch comparison page. |
| `5.Active Portfolio by Loans Status.png` | Screenshot of the loan status breakdown page. |
| `6.Total Portfolio Drill Down.png` | Screenshot of the drill-down detail page. |
| `7.Bookmark & selection (Tables & Visuals).png` | Screenshot showing bookmark/toggle navigation in action. |
| `8.Data Quality & Findings.png` | Screenshot of the data quality audit page. |

---

## 🛠️ Tools & Techniques Used

- **Power BI Desktop** — report design and visualization
- **Power Query** — data cleaning and transformation
- **DAX (Data Analysis Expressions)** — custom KPI and risk-ratio measures
- **Star schema data modeling** — fact/dimension table design for performance
- **Bookmarks & drill-through** — guided, interactive report navigation

---

## 🎯 Why It Matters

- **Protects capital** — early PAR % warnings let risk teams tighten lending criteria before losses build up.
- **Optimizes resources** — highlights which branches are over-performing versus accumulating bad debt.
- **Supports compliance** — the Data Quality page catches gaps before an audit does.
- **Bridges domain and tool** — built by someone with real credit and risk analysis background, not just Power BI training, so the metrics reflect what banking teams actually track.

---

## ▶️ How to Use

1. Clone or download this repository.
2. Open `Bank Credit Overview.pbix` in **Power BI Desktop** (free download from Microsoft).
3. Use the slicers and bookmark buttons on each page to explore the portfolio by branch, region, or loan status.
4. Right-click any visual to drill through to the underlying detail.

---

## 👤 Author

Built by **Dileepa Rathnayake** — a banking and finance professional with 13+ years of experience in credit and risk analysis, combined with Power BI and data analytics skills. This project applies that domain expertise to a real-world credit risk reporting scenario.

---

## 📄 License

No license specified yet — add one (e.g., MIT) if you'd like others to freely reuse or build on this report.
