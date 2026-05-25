# 🏨 Hotel Bookings — Excel Data Analysis Project

A complete, hands-on Excel data analysis project using a real-world hotel bookings dataset.  


---

## 📌 Project Overview

This project applies from basic formulas through to Power Query, Power Pivot, and DAX on a real hotel industry dataset with 119,390 booking records.

The goal is to answer 20 business questions a hotel revenue manager or operations analyst would genuinely ask, and to build a fully interactive performance dashboard as the capstone.

---

## 🗂️ Repository Structure

```
hotel-bookings-excel-analysis/
│
├── README.md                      
│
├── questions/
│   └── business_questions.md        ← All 20 business questions
│
├── solutions/
│   ├── 01_beginner_formulas.md      ← Q1–Q5  : Formulas & Functions
│   ├── 02_intermediate_pivots.md    ← Q6–Q12 : PivotTables & Charts
│   ├── 03_power_query_cleaning.md   ← Q13–Q15: Power Query
│   └── 04_power_pivot_dax.md        ← Q16–Q20: Power Pivot, DAX & Dashboard
│
└── assets/
    └── dashboard_preview.png        ← Dashboard screenshot 
```

---

## 📊 Dataset

**Source:** [Hotel Booking Demand — Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)  
**Original paper:** Antonio, Almeida & Nunes (2019), *Hotel booking demand datasets*, Data in Brief

| Property | Value |
|---|---|
| Rows | 119,390 bookings |
| Columns | 32 original + 4 engineered |
| Period | July 2015 – August 2017 |
| Hotels | City Hotel & Resort Hotel |
| File format | CSV (semicolon-delimited) → converted to `.xlsx` |


## 🛠️ Tools & Skills Used

| Tool | Skills Applied |
|---|---|
| **Excel Formulas** | `COUNTIF`, `AVERAGEIF`, `SUMIF`, `IFS`, `LARGE`, `INDEX/MATCH` |
| **PivotTables** | Grouping, calculated fields, top N filters, % of total |
| **PivotCharts** | Line, bar, column, combo charts with slicers |
| **Power Query** | Import, clean nulls, build date column, append, merge |
| **Power Pivot** | Data Model, relationships, DAX measures |
| **DAX** | `COUNTROWS`, `CALCULATE`, `FILTER`, `SUMX`, `DIVIDE`, `AVERAGE`, `TOTALYTD` |
| **What-If Analysis** | Two-variable Data Table |
| **Dashboard Design** | Slicers, `GETPIVOTDATA`, linked cells, layout |

---

## 📋 Business Questions Summary

> Full questions with hints: [`questions/business_questions.md`](questions/business_questions.md)  
> Step-by-step solutions: [`solutions/`](solutions/)

### 🟢 Beginner — Formulas & Functions (Q1–Q5)
1. What is the overall cancellation rate across all bookings?
2. Which hotel type has a higher average daily rate?
3. Add a `total_guests` calculated column to the data.
4. Classify each booking's lead time as Last Minute / Short / Medium / Long.
5. How many bookings had a room upgrade?

### 🟡 Intermediate — PivotTables & Charts (Q6–Q12)
6. Which month has the highest number of arrivals?
7. What is the cancellation rate by market segment?
8. Build a chart: average ADR by month for each hotel type.
9. Which top 10 countries do most guests come from?
10. What is the average length of stay by customer type?
11. Do guests who make more special requests cancel less?
12. What is the cancellation rate of repeated vs new guests?

### 🟠 Advanced — Power Query (Q13–Q15)
13. Build a proper `arrival_date` column from three separate columns.
14. Replace "NULL" text values in `agent` and `company` with proper blanks.
15. Split the dataset by hotel type, then Append back into one master table.

### 🔴 Advanced — Power Pivot & DAX (Q16–Q20)
16. DAX measure: `Est Revenue = adr × total_nights`. Revenue by hotel and year?
17. DAX measure: Cancellation Rate. Does deposit type affect cancellations?
18. DAX measure: Average waiting list days for canceled vs. completed bookings.
19. **Capstone:** Full interactive Hotel Performance Dashboard with slicers.
20. What-If Analysis: How does revenue change if ADR increases by 5/10/15%?

---

## 📈 Key Findings

| Metric | Value |
|---|---|
| Total bookings | 119,390 |
| Overall cancellation rate | 37.0% |
| Average ADR | €101.83 |
| Average length of stay | 3.4 nights |
| Total estimated revenue | €42,723,498 |
| Top guest country | Portugal (48,590 bookings) |
| Highest cancellation segment | Groups (61%) |
| Lowest cancellation segment | Complementary (6%) |
| Best revenue year | 2016 (€18,870,601) |
| City Hotel total revenue | €25,279,470 (59% of total) |
| Resort Hotel total revenue | €17,444,028 (41% of total) |
