# Global Superstore Analytics Dashboard

[![Tableau](https://img.shields.io/badge/Tableau-Workbook-blue)](https://www.tableau.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**An interactive Tableau dashboard suite that transforms raw superstore sales data into actionable insights about profit, delays, discounts, and operational performance across markets, managers, and product categories.**

![Dashboard Preview]([<img width="1838" height="739" alt="Home Page" src="https://github.com/user-attachments/assets/2e111233-7fa4-4931-8174-aa9ebfb16e08" />](https://github.com/j019/Global-Superstore-Analytics-Dashboard/blob/main/Home%20Page.png)
)  

🔗 Dashboard link : (https://public.tableau.com/app/profile/jatin.valecha/viz/Superstore_project_17802904775670/HomePage)

---

## 📊 Overview

This project presents a complete business intelligence solution built on the **Global Superstore** dataset. It contains 25+ worksheets, 11 dashboards, and numerous calculated fields that enable stakeholders to:

- Monitor KPIs (revenue, profit, quantity, delays)
- Analyze profit ratios and discount effectiveness
- Identify loss-making segments and delayed orders
- Drill down by region, manager, category, or country
- Compare annual profit trends (2019–2022)

All dashboards are interactive – filters, highlight actions, and URL actions (e.g., Wikipedia lookup for countries) provide an intuitive exploration experience.

---

## 🚀 Features

### Core Dashboards
| Dashboard | Purpose |
|-----------|---------|
| **Home Page** | Central navigation hub |
| **Profit Analysis Dashboard** | Profit ratio, profit status, and category breakdown |
| **Sales Analysis Dashboard** | Sales over time, by category, city, and state |
| **Category Analysis** | Sales and net sales per product category |
| **KPI Analysis by Country / Sub‑category** | Country‑level and sub‑category performance metrics |
| **Monthly Loss Analysis by Market** | Track loss counts and total quantity lost per market |
| **Average Discount Analysis By Region** | Discount distribution and its impact |
| **Analysis By Manager Dashboard** | Profit and discount performance per manager |

### Key Metrics (Calculated Fields)
- **Profit Status** – labels each row as `Profit`, `Loss`, or `No Loss No Profit`
- **Profit Ratio** – `SUM(Profit) / SUM(Revenue)`
- **Delay Days** – difference between expected and actual ship dates
- **No. of Delayed Orders** – count of orders with `Delay Days > 0`
- **Annual Profit** – separate fields for 2019, 2020, 2021, 2022
- **Profit Ratio Category** – classifies profit ratio into tiers (C1, C2, …)

### Interactive Actions
- **Filters** – by Segment, Order Priority, Market, Region, Sub‑Category, Country, Manager
- **Highlight Action** – dynamically highlight selected marks
- **URL Action** – opens Wikipedia page for a selected country

### Visual Design
- Custom color palette: `#1170aa` (blue), `#fc7d0b` (orange), `#a3acb9` (grey)

---

## 📁 Data Source

- **Name:** `Orders+ (Global Superstore)`
- **Format:** Excel / CSV (standard Superstore dataset)
- **Key tables:** Orders, Returns, People (managers), Shipping costs
- **Preprocessing:** No external ETL – all transformations (calculated fields, aliases) are embedded in the `.twb` file.

> ⚠️ **Note:** The original data file is **not** included in this repository. You can obtain a similar dataset from [Tableau Community](https://community.tableau.com/s/question/0D54T00000CWeX8SAL/sample-superstore-sales-excelxls) or use your own superstore data with matching column names.

---

## 🛠️ How to Use

### Prerequisites
- **Tableau Desktop** (version 2020.2 or later – the `.twb` file is XML‑based and should be compatible)
- (Optional) **Tableau Public** – to publish online
  
