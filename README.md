# Sales & Finance Analytics Report — AtliQ Hardware

**Tools used:** Microsoft Excel · Power Query · Power Pivot · DAX  
**Project type:** Course capstone project — CodeBasics Excel: Mother of Business Intelligence  
**Data period:** FY 2019 · FY 2020 · FY 2021  

---

## About this project

AtliQ Hardware is a company that sells hardware products — PCs, peripherals, and network devices — to customers across global markets. This project uses 3 years of their sales and finance data to build a structured set of business reports that help management answer key performance questions.

All reports were built entirely in Excel using Power Query for data cleaning, Power Pivot for data modelling, and DAX for calculated measures. No macros or VBA were used.

---

## Business questions answered

- Which customers generated the highest net sales — and how did that change year over year?
- Which divisions and product segments are growing fastest?
- How is gross margin (%) performing across quarters and sub-zones?
- Which markets are hitting their targets and which are falling short?
- What does the overall P&L look like across fiscal years?

---

## Reports included in this repository

| Report | Description |
|---|---|
| **[Customer Net Sales Performance](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/Customer%20Net%20Sales%20Performance.pdf)** | Net sales by customer for FY2019, FY2020, FY2021 with year-over-year growth % |
| **[Division Level Report](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/Division%20level%20Report.pdf)** | Net sales and growth % broken down by product division |
| **[GM% by Quarters](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/GM%25%20by%20Quarters%20(sub_zone).pdf) (Sub-zone)** | Gross margin % tracked quarter by quarter across geographic sub-zones |
| **[Market Performance vs Target](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/Market%20Performance%20Vs%20Target.pdf)** | Actual sales vs set targets by market — showing over/under performance |
| **[P&L by Fiscal Year](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/P%20%26%20L%20By%20Fiscal%20Year.pdf)** | Full profit & loss statement across FY2019–2021 — net sales, COGS, gross margin |
| **[P&L by Markets](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/P%20%26%20L%20For%20Markets.pdf)** | P&L broken down by individual market for a single fiscal year |
| **[P&L by Months](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/P%20%26%20L%20By%20Fiscal%20Month.pdf)** | Monthly P&L view showing seasonal patterns in revenue and margin |
| **[Top & Bottom 5 Products](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/Top%20and%20Bottom%205%20Products%20order%20by%20Qty.pdf)** | Ranked by quantity sold — identifying best and worst performing SKUs |
| **[Top 5 Countries](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/Top%205%20Countries%20in%202021.pdf)** | Net sales by country for FY2021 |
| **[Top 10 Products](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/Top%2010%20Products.pdf)** | Products with highest growth in net sales from FY2020 to FY2021 |
| **[New Products — FY2021](https://github.com/1vishalk/Excel-Project-Sales-and-Finance-Analytics/blob/main/New%20Products%202021.pdf)** | Products launched in 2021 and their net sales performance |

---

## How the data model was built

**Step 1 — Extract & Clean (Power Query)**
- Connected to raw CSV files containing sales transactions, product data, customer data, and market data
- Removed blank rows, fixed inconsistent date formats, corrected data types
- Unpivoted monthly sales columns into a proper row-based structure
- Merged dimension tables (customers, products, markets) with the fact table

**Step 2 — Data Model (Power Pivot)**
- Built a star schema: one central fact table (sales transactions) connected to four dimension tables — Customer, Product, Market, and Date
- Created a Date dimension table to support fiscal year calculations (AtliQ's fiscal year runs September to August)

**Step 3 — DAX Measures**
- Net Sales = SUM of net invoice sales amount
- Gross Margin = Net Sales minus Cost of Goods Sold
- Gross Margin % = DIVIDE(Gross Margin, Net Sales)
- Year-over-Year growth % = (Current Year - Previous Year) / Previous Year
- Target variance = Actual Net Sales minus Market Target

**Step 4 — Reports**
- Built each report as a separate PivotTable connected to the Power Pivot data model
- Applied consistent formatting and conditional formatting to highlight performance above/below benchmarks

---

## Key skills demonstrated

- **ETL using Power Query** — data extraction, cleaning, and transformation without manual copy-paste
- **Data modelling** — star schema design with fact and dimension tables
- **DAX** — calculated measures for business KPIs including margin analysis and YoY growth
- **Business reporting** — translating raw transaction data into management-ready reports

---

## About me

I am Vishal Khanduja, an IT professional based in Delhi NCR with 2+ years of experience in IT operations, billing systems, and data reporting. I built this project as part of the CodeBasics Excel course to develop hands-on MIS and reporting skills.

**LinkedIn:** [vishal-khanduja](https://www.linkedin.com/in/vishal-khanduja-6a8a46151/)
