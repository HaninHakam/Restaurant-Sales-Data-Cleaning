# 🍽️ Restaurant Sales — Excel Data Cleaning & Reporting

This project demonstrates **Excel Power Query cleaning**, **QA validation**, and an **interactive reporting dashboard** built on a messy restaurant sales dataset.  
It is part of my professional portfolio to showcase skills in **Excel, Power Query, and data analysis**.

📄 [Read the Full Case Study](Docs/case_study.md)  
🖼 [See Dashboard & QA Screenshots](Docs/screenshots/)
---

## 📊 Project Overview
A restaurant provided sales transaction data in CSV format.  
The raw data had issues such as:
- Text fields with extra spaces
- Dates stored as text (`DD-MM-YYYY`)
- Quantities stored with decimals (should be integers)
- Manager names stored in a single messy string
- No column for **Total Sales**

The goal was to:
1. **Clean & normalize the data** (Power Query pipeline).
2. **Perform QA checks** to ensure data quality.
3. **Build an interactive Excel dashboard** with KPIs and slicers.

## 📂 Repository Structure
-**Raw Data**
-**Clean Data**
-**Docs**
  -screenshots
---

## 🛠️ Tools & Skills Used
- **Excel Power Query (M)** – automated data cleaning
- **Excel formulas** – QA validation & KPIs
- **Pivot Tables & Pivot Charts** – interactive reports
- **Slicers & Timelines** – filtering and time analysis
- **VBA macro** (optional) – refresh & export cleaned data

---

## ⚡ Data Cleaning Steps
- Trimmed and cleaned text fields (`Purchase Type`, `Manager`, `City`)
- Parsed `Date` column correctly (`DD-MM-YYYY`)
- Converted numeric fields to correct types
- Rounded `Quantity` to integers
- Added calculated column: `Total Sales = Price * Quantity`
- Split `Manager` into **First Name** & **Last Name**
- Removed duplicate `Order ID`s
- Reordered columns for readability

---

## ✅ QA Checks
Implemented a `QA` sheet with formulas:
- Row counts (raw vs cleaned)
- Missing values check for `Date` & `Manager`
- Duplicate `Order ID` detection
- Negative/zero `Quantity` detection
- Sanity check: `SUM(Price * Quantity) = SUM(Total Sales)`

---

## 📈 Dashboard Highlights
- **KPIs**:
  - Total Sales
  - Total Orders
  - Average Order Value
  - % Online vs In-store Sales
- **Charts**:
  - Sales by Product (bar chart)
  - Sales by City (column chart)
  - Sales trend over time (line chart)
- **Filters**:
  - Slicers for Purchase Type, Payment Method, City
  - Timeline for Date

---

### Key Insights
- Fries and Burgers drive the highest sales.
- Online orders make up ~40% of total revenue.
- New York contributes the largest city-level sales.

---

**Tools & Skills Used:** Excel, Power Query (M), Pivot Tables, Charts, Dashboard Design, Data QA

---
“Future improvements: Automate refresh with VBA, build Power BI version, or migrate dataset to SQL Server for advanced querying.”
→ Shows growth mindset.

