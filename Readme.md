 Retail Supply Chain Dashboard – Power BI Project

 Project Overview

This Power BI dashboard provides a comprehensive analysis of retail supply chain data, helping stakeholders understand sales, profits, and performance trends across segments, regions, and products. This project highlights insights into sales performance and profit margins using visuals like bar charts, donut charts, and KPIs.



  Files Used

- Excel Dataset: `Retail-Supply-Chain-Sales-Dataset.xlsx`
- Power BI File: `Retail Supply Chain Dashboard.pbix`
- Dashboard Screenshot: `RetailDashboardScreenshot.png` (used for GitHub preview)
- README.md: Project description and setup guide



  How We Built the Report

 1. Data Import & Cleaning
- Imported Excel dataset into Power BI.
- Cleaned column headers (renamed where necessary).
- Loaded into Power Query and performed basic transformations.

 2. Created a Calendar Table
- Generated a calendar table using `CALENDARAUTO()` DAX.
- Created relationships between `Order Date` and the calendar table for time-based analysis.

 3. Data Modeling
- Established one-to-many relationships between fact and dimension tables.
- Ensured proper relationship between the Calendar and Sales data.

 4. Created DAX Measures
- Total Sales: `SUM(Sales)`
- Total Profit: `SUM(Profit)`
- Orders Count: `DISTINCTCOUNT(Order ID)`
- Profit Margin %: `DIVIDE(SUM(Profit), SUM(Sales), 0)`
- Additional measures used for chart slicing/grouping.

 5. Created Visualizations
- Line Chart – Sales Trend Over Time (X: Year, Y: Total Sales, Legend: Segment)
- Stacked Bar Chart – Total Profit by Region & Segment
- Donut Chart – Total Sales by Segment
- Stacked Bar Chart – Top 10 Products by Sales
- Card Visuals (KPI Panel) – Total Sales, Total Profit, Orders Count, Profit Margin %
- Product Slicer – Product Names for visual interactivity

 6. Added Slicer Visual
- Added slicers for Segment, Product Name, and Date for easier filtering.

 7. Set Interactions
- Adjusted visual interactions so slicers only affect selected visuals.

 8. Insights & Recommendations

  Key Insights
  
- Consumer segment leads with the highest total sales.
- Corporate segment has higher profit margins in some regions.
- Top 10 products contribute a large portion of total revenue.
- Sales trend is increasing year by year.

  Recommendations
  
- Promote high-performing products (like Canon and Fellowes).
- Investigate underperforming products to revise pricing or marketing.
- Focus more on the Consumer and Corporate segments for future campaigns.
- Explore new sales strategies for Home Office segment with low sales but potential.



  How to Use This Project

1. Clone or download this repository.
2. Open `Retail Supply Chain Dashboard.pbix` in Power BI Desktop.
3. Explore visuals, slicers, and filters.
4. Adjust or extend the report for deeper analysis.



  Credits

Dataset source: Provided internally  
Dashboard & Analysis by: G Lokesh  
