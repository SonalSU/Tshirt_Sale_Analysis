# 👔 Men's T-Shirt Brand Analysis using Azure SQL & Power BI

## 📌 Project Overview

This project demonstrates an end-to-end Business Intelligence solution built using **Azure SQL Database** and **Microsoft Power BI** to analyze men's t-shirt product data from multiple brands.

The project transforms raw CSV data into interactive dashboards that help analyze pricing strategies, discounts, profitability, product variety, and brand performance.

The solution follows a complete BI pipeline, starting from data ingestion into Azure SQL Database, data cleaning using SQL and Power Query, business metric creation using DAX, and finally designing and publishing interactive Power BI dashboards.

---

# 🎯 Business Problem

A fashion retail company offers men's t-shirts from hundreds of brands through an online marketplace. Although the company collects extensive product information, pricing details, and customer-related data, the information is stored in raw CSV files, making analysis difficult and time-consuming.

Business users need answers to questions such as:

- Which brands offer the highest discounts?
- Which brands generate the highest profits?
- Which brands have the largest product variety?
- Which premium brands have the highest average selling prices?
- Which brands are underperforming?

To support better business decisions, an interactive reporting solution is required that consolidates the data, calculates important business metrics, and presents insights through dynamic dashboards.

---

# 🎯 Project Objectives

- Import raw CSV data into Azure SQL Database.
- Clean and prepare data using SQL.
- Connect Azure SQL Database with Power BI.
- Perform data transformation using Power Query.
- Create calculated business metrics using DAX.
- Develop interactive dashboards for brand analysis.
- Publish reports using Power BI Service.
- Enable data-driven business decision making.

---

# 🛠️ Tech Stack

- Microsoft Azure SQL Database
- SQL
- Microsoft Power BI Desktop
- Power Query Editor
- DAX (Data Analysis Expressions)
- Power BI Service
- CSV Dataset

---

# 📂 Dataset

**Source:** CSV File

The dataset contains information related to men's t-shirts, including:

- Brand Name
- Product Name
- Original Price
- Sale Price
- Product Rating
- Product Reviews
- Product Variety
- Product Details

---

# 🔄 Project Workflow

## Step 1 – Data Loading

- Imported the raw CSV dataset into Azure SQL Database.
- Created a centralized database for analysis.

---

## Step 2 – Data Cleaning in Azure SQL

Performed preprocessing before connecting Power BI.

### Changes Performed

- Converted **Original Price** from Text to Numeric.
- Converted **Sale Price** from Text to Numeric.

This ensured accurate mathematical calculations and improved data quality.

---

## Step 3 – Power BI Connection

Connected Azure SQL Database with Power BI Desktop to import the cleaned dataset.

---

## Step 4 – Data Transformation using Power Query

Performed additional transformations including:

- Verified data types
- Removed unnecessary columns
- Checked null values
- Renamed columns
- Applied formatting
- Prepared clean data for visualization

---

## Step 5 – DAX Calculations

Created calculated columns using DAX.

### ✅ Cost Price

Calculated the estimated **Cost Price** for every product.

**Purpose**

- Estimate product cost.
- Support profitability calculations.
- Enable profit analysis.

---

### ✅ Discount Percentage

Calculated the percentage discount offered on every product.

**Purpose**

- Compare pricing strategies.
- Identify brands offering the highest discounts.

---

### ✅ Profit Percentage

Calculated product profit percentage using Cost Price and Sale Price.

**Purpose**

- Measure profitability.
- Compare brands based on profit margins.

---

# 📊 Dashboard Pages

## 🏠 Home Page

The landing page provides an attractive navigation interface with a brand selector and links to the detailed analysis pages.

**Features**

- Professional landing page
- Brand slicer
- Navigation buttons
- Custom background and branding

---

## 📈 Brand Performance Dashboard

The Brand Dashboard provides an overview of brand performance using multiple interactive visualizations.

### Top 5 Brands by Average Discount %

**Visual:** Bar Chart

**Purpose**

Displays brands offering the highest average discounts.

---

### Top 5 Brands by Highest Average Profit %

**Visual:** Area Chart

**Purpose**

Identifies brands generating the highest average profit percentages.

---

### Top 5 Brands by Product Variety

**Visual:** Donut Chart

**Purpose**

Shows brands with the highest number of available products.

---

### Top 5 Brands by Average Sales Price

**Visual:** Ribbon Chart

**Purpose**

Compares premium brands based on their average selling prices.

---

### Bottom 5 Brands by Average Profit %

**Visual:** Pie Chart

**Purpose**

Highlights brands with the lowest profit margins.

---

# 📊 Key Business Insights

The dashboard enables business users to:

- Compare discount strategies across brands.
- Identify premium brands based on average selling price.
- Analyze profitability using calculated profit percentages.
- Understand product variety offered by each brand.
- Detect underperforming brands for pricing optimization.
- Support data-driven pricing and inventory decisions.

---

# 🚀 Skills Demonstrated

- Azure SQL Database
- SQL Data Cleaning
- ETL Process
- Data Transformation
- Power Query
- DAX
- Data Modeling
- Power BI Dashboard Development
- Business Intelligence
- Data Visualization
- Dashboard Design
- Report Publishing

---

# 📷 Dashboard Preview

## Home Page

<img width="1775" height="805" alt="image" src="https://github.com/user-attachments/assets/23d51d6e-dd36-4a27-967c-db716d154f53" />


## Brand Analysis Dashboard

<img width="1772" height="807" alt="image" src="https://github.com/user-attachments/assets/7225ad2b-45b1-408a-b26f-063032f928e8" />



---

# 📁 Project Structure

```
Mens-Tshirt-Analysis
│
├── Dataset
│   └── Mens_Tshirt_Data.csv
│
├── SQL
│   └── Data_Cleaning.sql
│
├── PowerBI
│   └── Mens_Tshirt_Analysis.pbix
│
├── Images
│   ├── Home_Page.png
│   ├── Brand_Dashboard.png
│
└── README.md
```

---

# 📚 Learning Outcomes

Through this project, I gained hands-on experience in:

- Azure SQL Database
- SQL Data Cleaning
- Power Query Transformations
- DAX Calculations
- Power BI Data Modeling
- Dashboard Development
- Business Intelligence Reporting
- Power BI Service Publishing

---

# 🔮 Future Enhancements

- Add KPI Cards
- Dynamic Top N Filtering
- Drill-through Pages
- Tooltip Pages
- Row-Level Security (RLS)
- Incremental Refresh
- Executive Dashboard
- Real-Time Azure SQL Integration

---

# ⭐ Conclusion

This project demonstrates a complete Business Intelligence workflow, beginning with importing raw CSV data into Azure SQL Database and performing SQL-based data cleaning. The cleaned data was transformed using Power Query, while DAX calculated columns were developed to derive **Cost Price**, **Discount Percentage**, and **Profit Percentage**. Finally, interactive Power BI dashboards were created to analyze brand performance, pricing strategies, product variety, and profitability. The published solution enables stakeholders to explore business performance through dynamic visualizations and make informed, data-driven decisions.
