
# Myntra Apparel Data Analysis 

 ## Project Overview

This project focuses on analyzing a dataset of apparel products from Myntra, one of India’s leading online fashion retailers. The analysis includes data cleaning, transformation, analysis, and retrieval operations to generate insights into pricing trends, discounts, size availability, and product ratings.

## Problem Statement
As a data analyst at Myntra, you have been asked to analyze the dataset to provide insights on pricing, discounts, ratings, and available sizes. This will help the management in making data-driven decisions.


## Project Objectives
 ### A. Data Cleaning & Preparation

**Remove Duplicate Records**
- Checked using Remove Duplicates on all columns.

**Standardize DiscountOffer Format**
- Cleaned and converted all values into percentage or numeric format.

**Fill Missing DiscountPrice**
-  Where both DiscountPrice and DiscountOffer were null, filled using category-wise average discount price.

**Handle Missing Sizes**
-  Replaced all null values in SizeOption with "Not Available".

###  B. Data Analysis

- **Calculate the overall average original price for products with ratings greater than 4.**
```bash
 =ROUND(AVERAGEIF([Ratings],">4",[Original Price (in Rs)]),2)

```
- **Count the number of products with a discount offer greater than 50% OFF.**
```bash
=COUNTIF([DiscountOffer],">50%")
```
- **Count the number of products available in size "M."**
  
  Used filter function; result: 308,461 products.

- **Create a new column to label the products as "High Discount" if the discount offer is greater than 50% OFF, otherwise label them as "Low Discount."**
```bash
==IF([DiscountOffer]>0.5,"High Discount","Low Discount")
```
###  C. Data Retrieval & Lookup

VLOOKUP/XLOOKUP
→ Fetched brand, price, and rating for Product ID: 11226634.

INDEX + MATCH
→ Retrieved DiscountPrice for Product ID: 6744434.

Nested XLOOKUP
→ Used to retrieve any column’s value by providing Product ID.

### Connect with Me

🔗 [LinkedIn - Chinmay Singole](https://www.linkedin.com/in/chinmay-singole/)
"""

### Contributions
Contributions are welcome! Feel free to open an issue or submit a pull request.

### License
This project is licensed under the MIT License.

