# Insight BI — Men's T-Shirt Brand Performance Dashboard

An interactive Power BI dashboard that gives merchandising, category, and finance teams a single, consolidated view of brand-level performance across 200+ men's T-shirt brands.

## 📌 Overview

This retail/e-commerce business sources men's T-shirts from 200+ brands (Allen Solly, U.S. Polo Assn., Tommy Hilfiger, GAP, Scotch & Soda, The Bear House, SNITCH, and others). With such a large, fragmented catalog, the merchandising and category teams had no consolidated way to compare brands on discounting, profitability, pricing, and assortment depth — decisions were being made reactively rather than with data.

This project replaces manual, spreadsheet-based brand analysis with a two-page, interactive Power BI report.

## 🎯 Business Problem

The business lacked a single, reliable view of brand-level performance across four dimensions:

- **Discounting behavior** — which brands are discounted most heavily, risking margin erosion
- **Profitability** — which brands generate the highest / lowest average profit %
- **Price positioning** — which brands command the highest average sales price
- **Assortment depth** — which brands offer the widest product variety

Without this visibility, decisions on brand partnerships, discount policy, and inventory/assortment planning risked margin leakage on over-discounted brands and under-investment in high-performing ones.

*(Full details in the [Business Problem Statement](./business_problem_statement.docx).)*

## 👥 Target Audience

Merchandising managers, category managers, and business analysts responsible for brand strategy and pricing decisions.

## ✅ Objectives

- Identify the top 5 brands by average discount % to flag margin risk
- Identify the top 5 and bottom 5 brands by average profit % to guide partnership decisions
- Identify the top 5 brands by average sales price to understand premium positioning
- Identify the top 5 brands by number of product varieties to assess assortment depth
- Allow slicing/filtering by brand for ad-hoc drill-down

## 🛠️ Tools & Technologies

- **Power BI Desktop** — data modeling, DAX measures, report visuals
- **Data source** — Azure
- **DAX** — calculated measures (Average Discount %, Average Profit %, Average Sales Price)

## 🗂️ Data Overview

Brand-level records for men's T-shirts, including fields such as:

- Brand
- Title
- Original Price
- Sale Price

## 🔍 Approach / Methodology

1. **Data import & cleaning** — loaded data into Power BI, handled inconsistent brand naming and duplicates
2. **DAX measures** — built measures for Average Discount %, Average Profit %, and Average Sales Price
3. **Visualization** — built a two-page report: a cover page with a brand slicer, and a Brand Performance page with five key visuals

## 📊 Dashboard Visuals & Key Insights

| Visual | Type | Key Finding |
|---|---|---|
| Top 5 Brands by Avg Discount % | Bar chart | iVOC (89%), WUXI (85%), Mischief Monkey (85%), Voroxy X AG (85%), Red Tape (83%) lead in discounting — potential margin risk zone |
| Top 5 Brands by Avg Profit % | Area chart | LP Jeans and MUJI tie for the highest average profit at 17%, followed closely by a cluster of brands at 16% |
| Top 5 Brands by Highest No. of Varieties | Donut chart | The Indian Garage Co (51 styles, 22.9%) and U.S. Polo Assn. (44 styles, 19.7%) offer the deepest assortment |
| Top 5 Brands by Highest Avg Sales Price | Ribbon chart | Armani Exchange (~6.1K), Brooks Brothers (~5.1K), Terra Luna (~5.0K) command the highest price points |
| Bottom 5 Brands by Avg Profit % | Pie chart | Ramadhani Cloth (3.5%), Gespo and Chimpaaanzee (3% each), Be Active X AG and Aapska (2% each) are the least profitable brands |

**Overall average discount across all brands:** ~82.9%
**Overall average sales price:** ~10K

## 💡 Business Recommendations

- Review discount policy for iVOC, WUXI, Mischief Monkey, Voroxy X AG, and Red Tape — heavy discounting at 83–89% may be compressing margins disproportionately
- Double down on high-margin brands like LP Jeans and MUJI through better shelf placement or marketing spend
- Reassess partnerships with bottom-profit brands (Ramadhani Cloth, Gespo, Chimpaaanzee, Be Active X AG, Aapska) — renegotiate terms or reduce inventory exposure
- Leverage premium brands (Armani Exchange, Brooks Brothers) for higher-margin bundling or premium collection campaigns
- Expand assortment for high-variety, well-performing brands (Indian Garage Co, U.S. Polo Assn.) if sales data supports demand

## ⚠️ Limitations

- Report built from a static extract; profit %/discount % figures reflect a point-in-time snapshot
- Sample sizes vary by brand (some "bottom 5" brands may have very few SKUs, e.g. only 2), which can skew average % metrics
- No time-series/trend view included in this version

## 🚀 Future Scope

- Add a time trend page (monthly/quarterly profit and discount trends)
- Add category/sub-category breakdown (beyond just T-shirts)
- Automate data refresh from a live source (SQL/API) instead of manual load
- Add a brand scorecard combining all four metrics into a single ranking

## 📁 Project Files

- `Mens_Tshirt_Analysis_Project_Report.docx` — full project report
- `business_problem_statement.docx` — business problem statement
- Power BI report (`.pbix`) — dashboard file *(add link/path if included in repo)*

## ✍️ Author

**Sonal Undekar**
QA Engineer / Test Data Engineer
