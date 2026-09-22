# AtliQ Hardware Sales & Finance Analytics | Advanced Excel

An end-to-end **Sales & Finance Analytics project** built using Advanced Excel, Power Query, Power Pivot, DAX, and Pivot Tables to analyze AtliQ Hardware's sales performance, market performance, product growth, and gross profitability.

---

## 📌 Project Overview

AtliQ Hardware is a global hardware company that manufactures and sells products such as PCs, laptops, keyboards, mice, printers, and other computer peripherals.

This project analyzes sales and financial data across **customers, markets, products, channels, and fiscal periods** to identify business trends, performance gaps, growth opportunities, and profitability drivers.

---

## 🎯 Business Objectives

The analysis focuses on:

* Evaluating customer sales performance
* Comparing actual sales against 2021 targets
* Identifying high-growth products
* Analyzing top and bottom products by quantity sold
* Identifying products introduced in 2021
* Evaluating country and sub-zone performance
* Analyzing Net Sales, COGS, Gross Margin, and GM%
* Identifying margin and cost pressures
* Understanding seasonal and quarterly trends

---

## 🏢 Business Model

AtliQ Hardware manufactures hardware products and sells them through different channels.

### Products

* PCs
* Laptops
* Keyboards
* Mice
* Printers
* Computer peripherals

### Sales Channels

**Retailers**

* Croma
* Best Buy
* Staples
* Amazon
* Flipkart

**Distributors**

Products are also sold through distributors.

**Direct Channel**

AtliQ also sells products directly to customers.

### Channel Flow

```text
AtliQ Hardware
      ↓
Distributor / Retailer
      ↓
End Customer
```

---

# 🛠 Tools & Technologies

* Microsoft Excel
* Power Query
* Power Pivot
* DAX
* Pivot Tables
* Data Modeling
* ETL
* Data Analysis
* Business Intelligence

---

# 🔄 Data Analytics Workflow

```text
Raw Data
   ↓
Power Query
   ↓
Data Cleaning & Transformation
   ↓
Power Pivot Data Model
   ↓
Table Relationships
   ↓
DAX Measures
   ↓
Pivot Tables
   ↓
Sales & Finance Reports
   ↓
Business Insights
```

---

# 🔧 Data Preparation & ETL

Power Query was used to prepare the raw datasets for analysis.

### Key activities

* Data cleaning
* Data transformation
* Data type standardization
* Removing unnecessary columns
* Creating the date dimension
* Creating fiscal month and quarter fields
* Preparing datasets for the data model

---

# 🧩 Data Model

Power Pivot was used to create relationships between fact and dimension tables.

### Sales Analytics

**Dimensions**

* `dim_customer`
* `dim_market`
* `dim_product`
* `dim_date`

**Facts**

* `fact_sales_monthly`
* `fact_targets_21`

### Finance Analytics

The finance model uses the same dimensional structure with:

* `fact_sales_monthly_with_cost`

The additional cost information enables analysis of:

* Net Sales
* COGS
* Gross Margin
* GM%

---

# 📐 DAX Measures

### Sales Analytics

* Net Sales
* Net Sales 2019
* Net Sales 2020
* Net Sales 2021
* 21 vs 20
* 21 vs Target
* 21 vs Target %
* Target 2021

### Financial Analytics

* Net Sales
* COGS
* Gross Margin
* GM%

### Date Calculations

The `dim_date` table includes:

* Month Name
* Fiscal Month Number
* Fiscal Year
* Quarter

---

# 📈 Sales Analytics

## 1. Customer Performance

### Key Insights

* Net Sales increased from **$87.5M in 2019 to $598.9M in 2021**.
* **Amazon** was the largest customer in 2021, generating **$82.1M** in Net Sales and growing **218.87% YoY**.
* **AtliQ e Store** generated **$53.0M**, growing **223.83% YoY**.
* **AtliQ Executive** generated **$52.8M**, with **338.61% YoY growth**.
* Smaller customers such as **Integration Stores** and **Chiptec** recorded very high percentage growth, although their lower starting bases should be considered when interpreting these percentages.

### Business Observation

Sales growth was broad-based across the customer portfolio, while a relatively small number of large customers contributed significantly to total sales.

---

# 2. Market Performance vs Target

### Overall Sales Growth

Net Sales increased from:

**$87.5M → $196.7M → $598.9M**

from FY2019 to FY2021.

However, FY2021 sales were **$54.9M below the target**, representing an **8.4% shortfall**.

### Leading Markets

| Market         | FY2021 Sales |
| -------------- | -----------: |
| India          |      $161.3M |
| USA            |       $87.8M |
| South Korea    |       $49.0M |
| Canada         |       $35.1M |
| United Kingdom |       $34.2M |

India was the largest market, increasing from **$30.8M in 2019 to $161.3M in 2021**.

However, FY2021 India sales were **$9.6M below target**, a **5.6% shortfall**.

### Target Gaps

The USA recorded the largest absolute target gap at **$10.2M**, followed by:

* India: $9.6M
* Canada: $5.1M
* South Korea: $4.4M

By percentage shortfall:

* Poland: 15.3%
* Canada: 12.6%
* Spain: 12.4%
* Indonesia: 11.5%

### Business Observation

Strong YoY growth did not necessarily translate into target achievement. This suggests the business should investigate the drivers behind the target gaps at the **customer, product, channel, and market levels**.

---

# 3. Top Products by Growth

### Key Insights

* Analyzed products increased from **$6.4M in FY2020 to $52.0M in FY2021**, representing **808.04% growth**.
* **AQ Electron 4 3600 Desktop Processor** generated the highest FY2021 sales among the analyzed products at **$19.4M**, growing **641.26%**.
* **AQ Smash 2** increased from **$0.4M to $11.2M**, representing **2,589.49% growth**.
* **AQ Home Allin1** increased from **$0.7M to $5.2M**, representing **768.99% growth**.
* AQ GT 21 and AQ Pen Drive DRC also recorded substantial YoY growth.

### Business Observation

Some products combine **high absolute sales with high growth**, while other products show very high percentage growth because of a low FY2020 starting base.

---

# 4. Product Quantity Analysis

### Key Insights

* The top 5 products sold approximately **19.0M units**.
* The bottom 5 products sold only **174.9K units**.
* **AQ Master Wired x1 Ms** was the highest-volume product at approximately **4.2M units**.
* Three of the top five products belonged to the **AQ Master** product family.
* AQ Gamers products also appeared among the highest-volume products.

### Business Observation

The large difference between high- and low-volume products suggests an opportunity to investigate **product demand, pricing, promotion, product positioning, and portfolio rationalization**.

---

# 5. New Products Introduced in 2021

### Key Insights

AtliQ introduced **16 new products in 2021**, generating approximately **176.2M units**.

The highest-volume launches included:

* AQ Qwerty — 22.0M
* AQ Trigger — 20.7M
* AQ Gen Y — 19.5M
* AQ Trigger Ms
* AQ Qwerty Ms

The top five launches contributed approximately **54% of new-product volume**.

### Business Observation

New-product performance was concentrated among a few launches, particularly the **AQ Qwerty and AQ Trigger families**.

---

# 6. Top Markets by FY2021 Sales

India, USA, South Korea, Canada, and the United Kingdom were the largest markets by FY2021 sales.

India and USA together contributed approximately **67.8% of the sales volume among these five markets**, highlighting the importance of these markets to overall performance.

---

# 💰 Finance Analytics

## 1. Profit & Loss by Fiscal Year

### Key Insights

* Net Sales increased significantly from **$87.5M in FY2019 to $598.9M in FY2021**.
* COGS increased substantially alongside sales, indicating increasing direct cost pressure.
* GM% declined from **41.43% in FY2019 to 37.28% in FY2020 and 36.43% in FY2021**.
* The decline in GM% indicates that COGS increased faster than sales over the period.

### Business Observation

AtliQ achieved strong revenue growth, but the declining GM% indicates that maintaining sales growth while controlling direct costs became increasingly important.

> **Note:** GM% represents gross profitability and does not include operating expenses, depreciation, interest, taxes, or other indirect costs.

---

# 2. Monthly Profit & Loss Analysis

### Key Insights

* FY2019 recorded strong sales growth toward **October–December**, accompanied by higher COGS.
* November and December recorded some of the highest sales and COGS, indicating a seasonal demand pattern.
* GM% remained relatively stable around **41%–42% during FY2019**.
* Overall GM% subsequently declined to **37.28% in FY2020 and 36.43% in FY2021**.

### Business Observation

The combination of strong sales growth and declining GM% suggests that AtliQ should monitor **product costs, pricing, freight, manufacturing costs, and product mix**.

---

# 3. Market-Level Financial Performance

## High-Revenue Markets

### India

India generated approximately **$241.85M Net Sales**, with **$161.16M COGS** and a **33.4% GM%**.

Net Sales increased from **$30.82M in FY2019 to $161.26M in FY2021**, while GM% declined from approximately **42% to 32%**.

### USA

USA generated **$131.23M Net Sales**, **$82.54M COGS**, and **$48.69M Gross Margin**, resulting in a **37.1% GM%**.

### South Korea

South Korea generated **$79.05M Net Sales**, **$50.22M COGS**, and **$28.83M Gross Margin**, resulting in a **36.5% GM%**.

---

## Higher-Margin Growth Markets

Japan, Netherlands, New Zealand, and France recorded GM% between approximately **43.3% and 45.0%**.

New Zealand recorded the highest GM% among these markets at **45.0%**, followed by Japan at **44.7%**.

---

## Markets with Margin Pressure

Austria, Germany, Italy, and Norway recorded relatively lower GM%, ranging from **29.9% to 32.6%**.

Germany recorded a **29.9% GM%** despite $19.26M in Net Sales.

### Suggested Analysis

Further investigation could focus on:

* Product mix
* Pricing
* Freight costs
* Supplier costs
* Manufacturing costs
* Customer/channel mix

This can help identify the underlying drivers of lower gross margins.

---

# 4. Gross Margin % by Sub-Zone

## FY2019

* **ROA:** 44.4%
* **SE:** 44.2%
* **ANZ:** 42.6%
* **India:** 42.4%
* **NE:** 36.7%
* **NA:** 35.4%

GM% remained relatively stable across quarters, with limited variation within most sub-zones.

## FY2020

* **ANZ:** 42.8%
* **NA:** 39.8%
* **NE:** 37.8%
* **SE:** 37.9%
* **ROA:** 38.2%
* **India:** 32.2%

India recorded the lowest GM%, while ANZ maintained the highest.

## FY2021

* **SE:** 38.5%
* **ROA:** 38.3%
* **ANZ:** 38.3%
* **NE:** 38.3%
* **NA:** 37.3%
* **India:** 32.0%

India remained the lowest-margin sub-zone, while SE recorded the highest GM%.

### Key Business Observation

India's GM% declined from **42.4% in FY2019 to 32.0% in FY2021**, while ANZ declined from **42.6% to 38.3%**. These changes indicate areas where product mix, pricing, and cost structure could be investigated further.

---

# 📊 Reports

## Sales Report

![Sales Report](excel/screenshots/sales_report.png)

## Finance Report

![Finance Report](excel/screenshots/finance_report.png)

---

# 💡 Key Business Takeaways

The analysis highlights several important business themes:

* Strong overall sales growth from FY2019 to FY2021
* Significant growth across customers and markets
* Large FY2021 target gaps despite strong YoY growth
* High concentration of sales among major markets and customers
* Strong growth from selected products and new launches
* Significant differences in product volumes
* Declining overall GM% despite substantial revenue growth
* Regional differences in gross-margin performance
* Potential cost pressure in lower-margin markets

---

# ⚠️ Data Privacy Disclaimer

The datasets used in this project are based on the **Codebasics learning/project environment**.

Due to privacy and data-sharing restrictions, the original sensitive datasets are **not included in this repository**.

The repository contains the project structure, analysis methodology, reports, and relevant documentation without exposing restricted business data.

---

# 📁 Project Structure

```text
sales-finance-analytics-excel/
│
├── README.md
│
├── data/
│
├── excel/
│   └── screenshots/
│       ├── sales_report.png
│       └── finance_report.png
│
├── power_query/
│
├── power_pivot/
│
├── reports/
│
└── insights/
```

---

# 🙏 Acknowledgement

This project was completed as part of the **Codebasics learning/project ecosystem** and helped me practice end-to-end business analysis using Excel, Power Query, Power Pivot, and DAX.

Special thanks to **Dhaval Patel and the Codebasics team** for providing practical business-oriented analytics challenges.
