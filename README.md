# Amazon-Product-Review-Analysis
Excel Case Study - Analyzing Amazon Reviews and Product Insights

Role: Junior Data Analyst Company: RetailTech Insights Tools: Microsoft Excel (Pivot Tables, Formulas, Functions) Dataset: 1,465 products | 16 fields Duration: [June 2025 – July 2025]

## Project Overview

As part of a data analytics engagement at RetailTech Insights for DSA Final Project work, I work on the analysis of product and customer review data scraped from Amazon product pages. The goal was to generate insights for product development, marketing strategies, and customer engagement. This analysis leveraged Excel to clean, structure, and visualize data that could drive smart business decisions for Amazon sellers.

## Initial Setup
- Load the dataset in Excel. [Download Here](amazon_dataset.xlsx)
- Review the 16 columns to understand the structure. Clean data where necessary (remove NaNs, fix formatting in discount/price fields, etc.).

## Data Cleaning Steps
- Inspected Data Types & Structure Reviewed fields including product name, category, prices, discount, ratings, and aggregated reviews.
- Removed Duplicates, Eliminated redundant entries based on product names and IDs to ensure data integrity.
- Handled Missing Values
  - Replaced missing categories with “Unknown”
  - Imputed missing prices with median values when necessary
  - Standardized Formats
- Converted price columns to number format, stripped currency symbols ###
  -  Applied TRIM, CLEAN, and PROPER to product names and review titles
- Created Derived Fields
  - Discount Percentage
  - Estimated Revenue = actual price × rating count
  - Price Range Buckets: <₹200, ₹200–₹500, >₹500
  - Distribution Rating: 1.0, 2.0, 3.0, 4.0, 5.0
- Split comma-separated values into appropriate columns if needed.
- Convert price fields from strings to numerical values (₹200 → 200).
- Create calculated fields: e.g., discount_percentage, actual_price, revenue = rating_count × actual_price.

## Analysis Tasks Using Excel

### Perform the Pivot Tables & Calculated Columns by Using Excel:

#### Task	                                      Calculation
1. Avg discount % by category	                  Group by category, average discount_percentage
2. Count of products per category	              Group by category, count rows
3. Total reviews per category	                  Sum of review_count per category
4. Products with highest avg ratings	          Sort by rating, descending
5. Avg actual vs discounted price by category	  Group by category, avg of both prices
6. Products with highest number of reviews	    Sort by review_count, descending
7. Products with ≥50% discount	                Filter discount_percentage >= 50%
8. Distribution of ratings	                    Histogram or count by rating values (1.0, 2.0, 3.0, 4.0...)
9. Total potential revenue per category	        rating_count × actual_price aggregated
10. Products per price bucket	                  Create bins: <200, 200–500, >500
11. Rating vs Discount	                        Correlation/Scatter plot
12. Products with <1000 reviews	                Filter and count
13. Categories with highest discounts	          Avg discount by category
14. Top 5 products (rating + reviews)	          Rank using: normalized_rating + normalized_review_count

## GitHub Portfolio Structure
### Create a public GitHub repo. Example structure:
amazon-review-analysis/
│
├── 📁 data/
│   └── amazon_products_clean.csv
│
├── 📁 notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_analysis.ipynb
│   └── 03_visualizations.ipynb
│
├── 📁 visuals/
│   ├── category_discount.png
│   ├── [rating_distribution.png](https://github.com/Worthwad/amazon-product-review-analysis/blob/main/Distribution%20Rating.png)
│   └── amazon_dashboard.png
│[Download Here](amazon_dashboard.png)
├── 📁 dashboard/
│   └── Amazon_Review_Insights_Dashboard.xlsx
│
├── README.md
└── requirements.txt
📌 README.md Sample Outline:
markdown
Copy
Edit
# Amazon Product Review Analysis

## Objective
Analyze Amazon product review data to extract insights for product improvements and marketing strategies.

## Tools Used
- Excel (for pivot tables & dashboard)
- Git for version control

## Repository Structure
- `data/`: Cleaned dataset [Download Here](amazon_transformed_data.xlsx)
- `notebooks/`: Jupyter notebooks for each step 
- ![Amazon_Review_Insight_Dashboard](https://github.com/user-attachments/assets/da37dfbd-0f8e-4cc9-bdcb-42f42b36b6a4)
- `visuals/`: Key plots and dashboard snapshots
- ![Average Actual vs Discounted Price](https://github.com/Worthwad/amazon-product-review--analysis/blob/main/Average%20Actual%20vs%20Discounted%20Price.png) 
- ![Total Product By Category](https://github.com/Worthwad/amazon-product-review-analysis)
- ![Total Product By Category](https://github.com/Worthwad/amazon-product-review-analysis/blob/main/Total%20Product%20By%20Category.png)
- ![Distribution Rating](https://github.com/Worthwad/amazon-product-review-analysis/blob/main/Distribution%20Rating.png)

## Key Insights
- Average discount is highest in Home Improvement.
- Category X has the most reviews.
- Top-rated product with 5.0 stars.
  -  Amazon Basics Wireless Mouse (B09ZHCJDP1)
  -  Syncwire LTG to USB Cable (B0BP7XLX48)
  -  REDTECH USB‑C to Lightning Cable (B0BQRJ3C47) 
  
## Dashboard Preview
![Amazon_Review_Insight_Dashboard](https://github.com/user-attachments/assets/8e8a123b-82fb-4f0e-beae-6aec0c055ea0)

## How to Run
Clone the repo and run notebooks in order. Excel dashboard included for quick insights.
