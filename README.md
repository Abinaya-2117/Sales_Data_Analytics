# Sales Data Analytics

## Project Overview
This repository contains an end-to-end operational and financial analytics dashboard developed in **Microsoft Excel**. The project integrates and analyzes over 750 cross-functional records spanning customer support operations, order fulfillment, pricing structures, and regional sales performance. 

The goal of this project is to provide cross-functional leadership (Clinical, Operations, Coaching, Member Care, and Finance) with actionable insights into service quality, revenue drivers, agent efficiency, and discounting impacts.

---

## Key Dashboards & Features

### 1. Customer Service & Support Operations
- **CSAT Analysis:** Tracks average Customer Satisfaction (CSAT) scores across support agents.
- **Support Workload:** Monitors interaction volume grouped by contact types (**Query**, **Request**, **Complaint**).
- **Ticket Resolution Tracking:** Evaluates service performance and identifies support bottlenecks.
- 

### 2. Order Fulfillment & Pricing Metrics
- **Channel Performance:** Analyzes revenue distribution between **Online** orders and **Physical Visits**.
- **Discount & Revenue Impact:** Reconciles gross revenue against net revenue after applied discounts to identify margin erosion.
- **Product Demand:** Highlights top-performing products and sales volume trends.

### 3. Financial & Regional Sales Performance
- **Regional Breakdown:** Evaluates sales performance across key geographical territories (**North**, **South**, **East**, **West**).
- **Daily Sales Trends:** Tracks daily overall and average sales metrics to detect seasonal or operational fluctuations.
- **Rounding & Price Realization:** Compares actual sales values against nearest-unit rounded price thresholds.

---

## Data Architecture & Schema

The underlying data model consists of three core relational entities:

| Sheet Name | Key Metrics / Fields Included | Primary Key / Foreign Keys |
| :--- | :--- | :--- |
| **`Customer`** | Customer ID, Order ID, Contact Date, Contact Type, Ticket ID, Agent Handled, CSAT Rating | `Ticket ID`, `Order ID` |
| **`Order`** | Order ID, Product ID, Product Name, Order Type, Product Price, Agent, Quantity, Discounts, Revenue | `Order ID`, `Product ID` |
| **`Finance`** | Order ID, Product ID, Sale Date, Sales Amount, Discounted Value, Region, Rounded Sales Value | `Order ID`, `Product ID` |

---

## Tools & Techniques Used
- **Microsoft Excel / Google Sheets:** Data aggregation, Pivot Tables, conditional formatting, dynamic charts, timeline slicers.
- **Data Analysis Methods:** Data cleaning, metric reconciliation, KPI formulation, cross-tabulation.
- **SQL / Python (Pandas & Seaborn):** Extracted, validated, and programmatically visualized dataset distributions and trends.

---

## How to View
**Interactive Excel Dashboard:** Download `Dashboard.xlsx` and open locally in Microsoft Excel (2013 or newer) to interact with pivot slicers and dynamic charts.
