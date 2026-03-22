# FP&A Budget vs Actual Dashboard — Power BI

![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?logo=powerbi)
![Excel](https://img.shields.io/badge/Excel-Data%20Source-green?logo=microsoftexcel)
![Status](https://img.shields.io/badge/Status-Complete-brightgreen)
![Finance](https://img.shields.io/badge/Domain-FP%26A%20Finance-blue)

> End-to-end FP&A dashboard tracking a **£27M annual budget** across 6 departments for a mock UK financial services firm — Meridian Financial Group UK Ltd. Built to demonstrate financial analysis, variance reporting, and management reporting skills.

---

## Dashboard Preview

![FP&A Dashboard](FPA_Dashboard_Hardik.png)

---

## Business Problem

Finance teams spend hours each month manually comparing budget vs actual spend in Excel — copying data, checking figures, and reformatting reports for leadership. This dashboard automates that entire process and delivers:

- Instant RAG (Red/Amber/Green) status per department
- Monthly budget vs actual trend with variance line
- Waterfall chart showing which departments drove over/underspend
- Year-end forecast projection
- Quarterly and monthly dynamic filtering

---

## Key Findings

| Department | Budget | Actual | Variance | Status |
|---|---|---|---|---|
| Operations | £9,600K | £9,750K | +£150K | AMBER |
| Technology | £5,800K | £5,960K | +£160K | RED |
| Risk & Compliance | £3,600K | £3,485K | -£115K | GREEN |
| Finance | £3,200K | £3,130K | -£70K | GREEN |
| HR | £2,400K | £2,350K | -£50K | GREEN |
| Sales | £2,600K | £2,640K | +£40K | AMBER |
| **TOTAL** | **£27,200K** | **£27,335K** | **+£115K** | |

**Key insight:** Technology is the only RED department — overspent by £160K (+2.76%). HR delivered the strongest underspend at -£50K. Year-end forecast projects £27,630K — £430K above original budget.

---

## Dashboard Features

- **4 KPI Cards** — Total Budget, Total Actual, Variance, YE Forecast
- **Line & Clustered Column Chart** — Monthly Budget vs Actual with Variance line overlay
- **Donut Chart** — Annual actual spend split by department
- **RAG Status Table** — Conditional formatting (Green/Amber/Red) with variance % per department
- **Waterfall Chart** — Variance drivers by department (red = over, green = under)
- **Quarterly Slicer** — Q1/Q2/Q3/Q4 dynamic filtering
- **Month Slicer** — Filter by individual month

---

## Tools Used

| Tool | Purpose |
|---|---|
| Power BI Desktop | Dashboard design and visualisation |
| Excel | Data source — flat table structure |
| DAX | Calculated measures and formatting |
| Power Query | Data transformation and column typing |

---

## Data Structure

The data is structured in **flat/long format** — the correct format for Power BI:

**Monthly_Actuals table** (72 rows — one per month per department)

| Month | Month_Num | Department | Budget_GBP | Actual_GBP | Variance_GBP |
|---|---|---|---|---|---|
| Jan | 1 | Operations | 800 | 780 | -20 |
| Jan | 1 | Technology | 483 | 510 | +27 |
| ... | | | | | |

**Dept_Summary table** (6 rows — one per department)

| Department | Annual_Budget | Annual_Actual | Variance_GBP | Variance_Pct | RAG_Status | YE_Forecast |
|---|---|---|---|---|---|---|

---

## How to Run

1. Download `FPA_PowerBI_CLEAN_Hardik.xlsx` from this repo
2. Open **Power BI Desktop** (free at powerbi.microsoft.com)
3. Get Data → Excel → select the file → load all 3 tables
4. Open `FPA_Dashboard_HardikSolanki.pbix` to view the finished dashboard

---

## Skills Demonstrated

- Financial Planning & Analysis (FP&A)
- Budget vs Actual variance reporting
- RAG status reporting for management packs
- Year-end forecasting
- Power BI dashboard design (DAX, Power Query, conditional formatting)
- Data modelling — flat table structure for BI tools
- Management reporting for senior stakeholders

---

## About

Built by **Hardik Solanki** — Finance & Data Analyst with 3+ years experience in financial reporting, FP&A, and data visualisation.

- LinkedIn: [linkedin.com/in/hardiksolanki](https://linkedin.com/in/hardiksolanki)
- GitHub: [github.com/shardik-solanki](https://github.com/shardik-solanki)
- Email: hardiksolanki.uk@gmail.com

*Part of a finance project portfolio targeting FP&A Analyst and Financial Analyst roles in UK financial services.*
