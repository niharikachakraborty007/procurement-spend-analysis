# Procurement Spend Analysis | Power BI

## Project Overview

An interactive Power BI dashboard designed to analyse procurement expenditure, supplier performance, buyer spending patterns and product-level purchasing trends.

The project uses a company purchasing dataset containing 500 transactions across 2024. It demonstrates data preparation, dimensional modelling, DAX calculations and interactive dashboard development.

## Business Objectives

- Analyse overall procurement expenditure.
- Identify the highest-spending product categories.
- Evaluate supplier spending concentration.
- Compare buyer-level procurement activity.
- Examine monthly spending trends and month-over-month changes.
- Identify products contributing most to total procurement spend.

## Dataset Overview

The dataset contains 500 purchase transactions and 9 columns:

- TransactionID
- ItemName
- Category
- Quantity
- UnitPrice
- TotalCost
- PurchaseDate
- Supplier
- Buyer

Coverage: January–December 2024.

The dataset contains 10 unique products, 6 categories, 5 suppliers and 20 buyers.

## Data Preparation and Modelling

Data preparation was performed using Power Query.

Key steps:
- Inspected data quality and checked for missing values and duplicates.
- Verified transaction identifiers and positive quantity and price values.
- Created dimension tables for products, suppliers and buyers.
- Created a calendar table using DAX.
- Built a star-schema data model with one-to-many relationships.

### Data Model

- Fact Purchases
- DimDate
- DimItem
- DimSupplier
- DimBuyer

## DAX and Measures

Key measures developed include:

- Total Procurement Spend
- Total Transactions
- Total Quantity Purchased
- Average Purchase Value
- Average Unit Price
- Category Spend Contribution %
- Supplier Spend Contribution %
- Previous Month Spend
- Monthly Spend Change
- MoM Growth %
- Top 5 Product Spend
- Top 5 Product Spend %
- Unique Products Purchased
- Average Quantity per Transaction
- Highest Supplier Spend
- Top Supplier Spend Contribution %

## Dashboard Pages

### 1. Executive Overview
- Overall procurement KPIs
- Category-wise spending
- Monthly procurement trend
- Supplier spending comparison
- Top five products by spend
  
### 2. Supplier & Buyer Analysis
- Supplier and buyer KPIs
- Supplier contribution analysis
- Supplier spend distribution
- Top five buyers by procurement spend
- Monthly spend and month-over-month growth

### 3. Product & Spending Analysis
- Top five products by spend
- Category spending distribution
- Product-level quantity and price analysis
- Detailed product spend table

Interactive slicers allow users to filter the report by date, category, supplier, buyer and product.

## Dashboard Previews

### 1. Executive Overview

![Executive Overview](screenshots/Executive%20Overview%20.png)

### 2. Supplier & Buyer Analysis
![Supplier and Buyer Analysis](screenshots/Supplier-buyer%20analysis.png)

### 3. Product & Spending Analysis
![Product Spending Analysis](screenshots/Product%20Spending%20Analysis.png)


## Key Findings

- Total procurement expenditure: 1,240,580.53
- Total purchase transactions: 500
- Electronics accounted for approximately 56.25% of total expenditure.
- Software accounted for approximately 27.09% of total expenditure.
- The top five products contributed approximately 90.74% of total procurement spend.
- TechMart Inc. was the highest-spending supplier, contributing approximately 26.50% of expenditure.
- Laptop and Annual Software License were the two highest-spending products.

*Note: The dataset does not specify a currency, so monetary figures are presented without a currency designation.*

## Tools and Technologies

- Microsoft Power BI Desktop
- Power Query
- DAX
- Data Modelling
- Data Visualization

## Project Files

- `Procurement Spend Analysis.pbix` — Power BI report
- `Procurement Spend Analysis.pdf` — Dashboard export
- `screenshots/` — Dashboard page previews

## Author

Created as a practical data analytics portfolio project to demonstrate Power BI, data modelling, DAX and business reporting skills.
