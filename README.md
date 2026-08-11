# AdventureWorks Sales Analysis - Power BI Dashboard 
## Project Overview 
This project is an end-to-end Power BI business intelligence dashboard designed for 
**AdventureWorks**, a fictional manufacturer of bicycles and cycling accessories. The report 
transforms raw sales, product, and customer data into an interactive, two-page dashboard. It is 
built to help stakeholders track high-level financial performance, analyze product profitability, 
and understand customer purchasing behavior. 
## Dashboard Pages & Features 
### 1. Executive Dashboard Summary 
The first page serves as the financial anchor, designed for C-suite executives to grasp company 
performance at a glance. 
*   **Key Performance Indicators (KPIs):** Total Revenue ($24.91M), Total Profit ($10.46M), 
Profit Margin % (41.97%), and Revenue YoY Growth % (58.40%). 
*   **Performance Trends:** A line chart plotting Total Revenue by Year (2015–2017). 
*   **Product Profitability:** Bar charts breaking down Total Revenue, Total Cost, and Profit 
Margin % by Product Category.  
*   *Insight:* While "Bikes" generate the vast majority of total revenue, "Accessories" yield 
the highest profit margins. 
<!-- PLACEHOLDER FOR PAGE 1 IMAGE --> 
![Executive Dashboard Summary](INSERT_IMAGE_LINK_HERE) 
*Caption: Executive Overview page showing revenue trends, product profitability, and year
over-year growth.* --- 
### 2. Detailed Insights 
The second page drills down into operational volume, time intelligence, and customer 
demographics, designed for sales and marketing managers. 
*   **Volume KPIs:** Total Quantity Sold (84,174) and Total Orders (56,046). 
*   **Order & Quantity Tracking:** A dual-line chart comparing Total Orders and Total Quantity 
Sold over time. 
*   **Category Distribution:** A donut chart showing the share of Total Quantity Sold by 
Category Name (Accessories lead by volume at 68.68%). 
*   **Time Intelligence:** A clustered column chart comparing Total Revenue vs. Revenue 
Previous Year across all months, clearly highlighting seasonal growth. 
*   **Customer Demographics:** A detailed matrix breaking down Total Revenue, Orders, 
Quantity, and Profit Margin % by Customer Education Level (e.g., Bachelors, Graduate Degree, 
Partial College). 
<!-- PLACEHOLDER FOR PAGE 2 IMAGE --> 
![Detailed Insights Dashboard](INSERT_IMAGE_LINK_HERE) 
*Caption: Detailed Insights page showing operational volume, seasonal trends, and customer 
demographics.* 
## Interactive Elements & Navigation 
The report features a custom-built, unified navigation pane on the left side of every page: 
*   **Page Navigation Buttons:** Allows users to seamlessly toggle between the "Overview" and 
"Detailed Insights" pages. 
*   **Global Slicers:** Tile-based slicers for **Year** (2015, 2016, 2017) and **Product 
Category**, allowing users to instantly filter the entire canvas contextually. 
## Data Model & DAX 
The backend relies on a robust Star Schema data model featuring: 
*   **Centralized Measures:** All DAX calculations are organized within a dedicated 
`_Measures` table. 
*   **Time Intelligence:** Utilizes a custom `Dim_Date` table to accurately calculate Year-over
Year (YoY) growth and Previous Year metrics. 
*   **Measure Branching:** Foundational measures (Total Cost, Total Revenue) are branched 
into advanced analytics (Profit Margin %, YoY Growth). 
<!-- PLACEHOLDER FOR DATA MODEL IMAGE --> 
![Data Model Schema](INSERT_IMAGE_LINK_HERE) 
*Caption: Star Schema data model featuring active/inactive relationships and the central fact 
tables.* 
## How to Use This Report 
1.  Download the `.pbix` file from this repository. 
2.  Open the file using **Power BI Desktop**. 
3.  Use the buttons on the left navigation bar to switch between pages. 
4.  Click on any of the Year or Product Category slicers on the left panel to filter the dashboard. 
You can also click directly on any chart element (like the "Bikes" bar) to cross-filter the rest of 
the page. 
