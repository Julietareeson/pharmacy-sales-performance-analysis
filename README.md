# Pharmacy Sales & Profit Performance Analysis

> An interactive Power BI dashboard analyzing pharmacy sales, revenue, profitability, product performance, promotional activities, and pharmacy branch performance.
>
> ## Project Overview

A pharmacy chain was experiencing inconsistent sales and profit performance across its branches. The goal of this project was to analyze sales data to understand revenue and profitability across pharmacies and products, evaluate promotional performance, identify periods of strong and weak performance, and highlight areas that may require operational improvement.

## Business Questions

- Which pharmacies generate the highest revenue and profit?
- Which products contribute the most to total sales?
- Do promotional campaigns increase sales and profit?
- Which months have the strongest and weakest performance?
- Which products have high sales but low profit margins?
- Which pharmacies need operational improvement?

 ## Tools Used

- Power BI
- Power Query
- DAX
- Microsoft Excel

 ## Data Cleaning & Preparation

The dataset was reviewed and prepared in Power Query before building the data model.

- Checked FactSales for errors and missing values.
- FactSales columns had 0% errors and 0% empty values.
- Checked for duplicate records; no duplicates were found.
- Verified fields with Yes/No values for consistency.
- Reviewed the DimDate and DimPharmacy tables.
- Reviewed the DiscontinuedDate field, where most values were empty because the products had no recorded discontinuation date.
- Ensured the data was ready for modeling and analysis in Power BI.

 ## Data Modeling

A star-schema data model was created in Power BI to organize the sales data and support efficient analysis.

- FactSales was used as the central fact table containing the sales transactions.
- DimDate was used to analyze performance over time.
- DimPharmacy was used to analyze revenue and profit across pharmacy branches.
- DimProduct was used to analyze product performance.
- A separate Measures table was created to organize the DAX measures used in the analysis.
- Relationships were established between the dimension tables and FactSales to allow the dashboard visuals to interact correctly.

 ## DAX Measures & Analysis

DAX measures were created to calculate key performance indicators and support the dashboard analysis.

The analysis focused on:

- Total Revenue
- Total Profit
- Total Cost
- Total Units Sold
- Profit Margin %
- Revenue and profit by pharmacy
- Revenue and profit by product
- Revenue and profit by promotional activity
- Monthly revenue and profit performance

## Key Insights

- The pharmacy chain generated 8.63M in total revenue and 2.42M in total profit, with an overall profit margin of 28%.
- Vienna HealthPoint #074 was the highest-performing pharmacy by revenue and profit.
- ZenHealth Herbal Tea Active was the top-performing product by revenue and profit.
- Promotional sales generated significantly lower revenue and profit than non-promotional sales, suggesting that the promotional campaigns did not produce a strong overall financial impact.
- July recorded the highest monthly revenue, while February recorded the lowest.
- Several products generated high sales but had relatively low profit margins, with margins around 21%–25%. These products may require pricing, cost, or margin optimization.
- Pharmacy profitability varied considerably across branches, indicating that lower-performing locations may require further operational review.
