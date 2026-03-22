# 📊 Sales Domain Analytics Dashboard — Power BI Project

> A comprehensive end-to-end Business Intelligence solution built on the **Sales Domain**, covering data modeling, cleaning, AI-assisted analysis, KPI tracking, and predictive forecasting.

---

## 🗂️ Project Overview

This project delivers a fully structured Power BI dashboard designed to provide actionable insights across sales performance, profitability, and budget tracking. It integrates modern AI tooling via **MCP Server** to accelerate development and improve accuracy.

---

## 🔄 Workflow & Methodology

### 1. 🏗️ Data Modeling

Defined the core schema using a **Star Schema** approach:

- **Fact Table** — `All_Sales`: Central table holding all transactional records and foreign keys linking to dimension tables.
- **Dimension Tables** — Each with its own Primary Key, referenced as Foreign Keys in the Fact Table.
- **Calendar Date Table** — Created from scratch to ensure clean, deduplicated date values and seamless time-intelligence calculations.
```
Dimension Tables ──FK──▶ Fact Table (All_Sales) ◀──FK── Calendar Date
```

---

### 2. 🧹 Data Cleaning

Restructured and validated raw data to ensure analytical reliability:

- Rebuilt data schemas to enforce consistency and correct data types.
- **Budget Consolidation Challenge**: Budget data was spread across **3 separate tables** (2019, 2020, 2021). These were unified into a single `Budget` table to enable accurate **Total Budget** calculations.

---

### 3. 🤖 AI-Assisted Analysis via MCP Server

Integrated a **Model Context Protocol (MCP) Server** to connect Power BI with an AI Agent — significantly boosting productivity:

| Task | Traditional Approach | With MCP Server |
|---|---|---|
| Relationship Validation | Manual review | AI-confirmed automatically |
| DAX Measure Creation | Written by hand | AI-generated |
| Error Detection | Trial & error | Instant suggestions |

> 💡 The MCP Server acted as a bridge between Power BI and the AI Agent, enabling real-time assistance throughout the modeling and development phases.

---

### 4. 📈 Key Performance Indicators (KPIs)

Calculated and visualized the most critical business metrics:

| KPI | Description |
|---|---|
| 💰 Total Sales | Aggregate revenue across all periods |
| 📦 Total Cost | Full cost of goods and operations |
| 📊 Gross Profit | Revenue minus cost |
| 📅 YoY Sales Growth | Current vs. prior year comparison |
| 📉 YoY Profit Trend | Identifies growth or decline patterns |
| 🧾 Budget vs. Actual | Tracks performance against targets |

> Year-over-Year comparisons enable stakeholders to **identify problems early** and make informed corrective decisions.

---

### 5. 🔮 What-If Analysis (Predictive Forecasting)

Added a dynamic **What-If Analysis** feature to support scenario planning:

- Simulate the impact of sales changes (e.g., *"What if sales increase by 5%?"*)
- Adjustable parameters using Power BI slicers
- Enables **data-driven, forward-looking decision making** without relying on static reports
```
📌 Example Scenario:
  Base Sales: $1,000,000
  What-If Growth: +5%
  Projected Sales: $1,050,000
```

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| ![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black) | Dashboard development & visualization |
| **DAX** | Calculated measures and KPIs |
| **MCP Server** | AI-Power BI integration |
| **Power Query (M)** | Data transformation & cleaning |

---

## 📁 Data Architecture
```
📦 Sales Project
 ┣ 📊 Fact Table
 ┃ ┗ All_Sales (Transactions, FK references)
 ┣ 📋 Dimension Tables
 ┃ ┣ Products
 ┃ ┣ Customers
 ┃ ┣ Regions
 ┃ ┗ Sales Reps
 ┣ 📅 Calendar Date Table
 ┗ 💵 Budget Table (Merged: 2019 + 2020 + 2021)
```

---

## 🚀 Key Highlights

- ✅ Clean star schema with no circular relationships
- ✅ AI-powered DAX generation via MCP Server
- ✅ Consolidated multi-year budget into a unified table
- ✅ YoY trend analysis for Sales, Profit & Cost
- ✅ Dynamic What-If scenario modeling
- ✅ Custom Calendar Date table for time intelligence

---

## 📬 Contact

Feel free to connect or share feedback!

linkedIn : [https://www.linkedin.com/in/mohammed-weal/]
Email : [mohammedweal2003@gmail.com]
