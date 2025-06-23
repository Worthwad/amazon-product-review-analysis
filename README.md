# Amazon-Product-Review-Analysis
Excel Case Study - Analyzing Amazon Reviews and Product Insights

Role: Junior Data Analyst Company: RetailTech Insights Tools: Microsoft Excel (Pivot Tables, Formulas, Functions) Dataset: 1,465 products | 16 fields Duration: [Add duration: e.g., June 2025 – July 2025]

## Project Overview

As part of a data analytics engagement at RetailTech Insights for DSA Final Project work, I work on the analysis of product and customer review data scraped from Amazon product pages. The goal was to generate insights for product development, marketing strategies, and customer engagement. This analysis leveraged Excel to clean, structure, and visualize data that could drive smart business decisions for Amazon sellers.

## Data Cleaning Steps
### Inspected Data Types & Structure Reviewed fields including product name, category, prices, discount, ratings, and aggregated reviews.
### Removed Duplicates Eliminated redundant entries based on product names and IDs to ensure data integrity.
### Handled Missing Values
  - Replaced missing categories with “Unknown”
  - Imputed missing prices with median values when necessary
  - Standardized Formats
### Converted price columns to number format, stripped currency symbols ###
  -  Applied TRIM, CLEAN, and PROPER to product names and review titles
### Created Derived Fields
  - Discount Percentage
  - Estimated Revenue = actual price × rating count
  - Price Range Buckets: <₹200, ₹200–₹500, >₹500
