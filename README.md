# KarmixTech_Financial_Performance_Dashboard
Karmix Tech Data Analytics Internship — Project 3

Business Problem

Finance teams need to know where actual spending is deviating from budget, by region and department, so they can take corrective action before small overspends become large ones. This dashboard analyzes Budget vs Actual performance across regions, departments, and account categories to flag where cost control is needed.

Dataset


Synthetic monthly financial dataset built to reflect realistic corporate budgeting patterns, including festive-season revenue seasonality and lumpy quarter-end CapEx
Size: 1,296 rows — Date, Region (East/North/South/West), Department (Sales/Marketing/Operations/R&D/Admin), Account Category (Revenue/COGS/OpEx/CapEx), Budgeted Amount, Actual Amount
Time period: Jan 2022 – Dec 2024 (3 years, monthly)


Tools Used


Python (Pandas, Seaborn, Matplotlib) — EDA and data quality checks
Power BI — dashboard with DAX measures (Operating Profit, Profit Margin %, Budget Variance %)


Approach


Verified data quality: zero nulls, zero duplicates, no negative amounts
Calculated company-wide KPIs: Total Revenue, Operating Profit, Profit Margin %, Budget Variance %
Built a variance heatmap by Region × Account Category to surface where overspending concentrates
Built a Power BI dashboard with KPI cards, quarterly revenue trend by region, variance comparison chart, drill-down table, and slicers (Year, Region, Department)


Key Insights


Total Revenue: ₹35.4 Cr | Operating Profit: ₹8.78 Cr | Operating Profit Margin: 24.8%
Overall Budget Variance: +7.2% (actual spend running above budget company-wide)
East region is the main problem area — COGS is 17.9% over budget and OpEx is 23.6% over budget, far worse than North, South, or West
The single biggest overspend line item is East Marketing OpEx at +32.2%, tied to Q4 festive campaign spend
Revenue shows consistent Q4 seasonality across all regions (festive season demand spike)


Recommendations


Conduct a cost control review specifically for the East region's COGS and OpEx
Tighten budget approval for Q4 marketing campaign spend before the festive season starts
Use the quarterly seasonality pattern to set more accurate, season-adjusted budgets going forward


Files in this Repository


Financial_Performance_Budget_vs_Actual.csv — dataset
KarmixTech_Financial_Performance.ipynb — Python EDA notebook
KarmixTech_Financial_Performance.pbix — Power BI dashboard
dashboard_screenshot.png — dashboard preview
