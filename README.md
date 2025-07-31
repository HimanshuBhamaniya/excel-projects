# 🛍️ Retail Store Sales Data Cleaning Project

This Excel-based project focuses on cleaning and preparing a messy retail store sales dataset downloaded from **Kaggle**. 
The dataset contains transactional data across various product categories and includes several missing values 
requiring thoughtful handling to preserve data integrity.

## 📦 Dataset Overview

- **File Name:** `retail_store_sales.xlsx`
- **Total Records:** 12,576
- **Columns:** 11
  - Transaction ID
  - Customer ID
  - Category
  - Item
  - Price Per Unit
  - Quantity
  - Total Spent
  - Payment Method
  - Location
  - Transaction Date
  - Discount Applied

## 🎯 Objective

Clean and organize the dataset for analysis by:
- Handling missing values
- Structuring item-price relationships by category
- Creating reference tables to validate pricing consistency

## 🧹 Cleaning Summary

### Initial Observations
- Missing values were found in:
  - Item
  - Price Per Unit
  - Quantity
  - Total Spent
- All other columns were complete and had no duplicates.

### Cleaning Steps
1. **Column Adjustments:**
   - Resized column widths for clarity
   - Checked and confirmed no duplicate records

2. **Structured Data Table:**
   - Converted dataset into an Excel Table for easier filtering and formula application

3. **Category Breakdown:**
   - 8 categories identified:
     - Furniture
     - Electric Household Essentials
     - Milk Products
     - Computers & Electric Accessories
     - Food
     - Beverages
     - Butchers
     - Patisserie
   - 25 unique items per category
   - Reference lists for two categories provided; others built using Remove Duplicates tool

### Missing Value Handling
- **Item:** Imputed using `INDEX-MATCH` based on category and price reference lists
- **Price Per Unit:** Calculated as `Total Spent / Quantity` where both values were present
- **Quantity, Total Spent, Discount Applied:** Left blank if not inferable due to unclear source documentation

## 📊 Output Tables

Separate **Item-Price Tables** were created for each category, which helped:
- Impute missing item names
- Validate pricing across transactions

Each output table includes:
- Item
- Price Per Unit

## 📝 Notes
- All data transformations were documented
- Missing entries were handled conservatively to maintain analytical transparency
- Further clarification from domain experts may improve imputation logic

## 👨‍💻 Author

Created by **Himanshu Bhamaniya** — committed to improving real-world data workflows through structured analysis and intuitive cleanup strategies.

---

> This project sets the groundwork for deeper insights into retail trends and can be enhanced with visualization tools like Power BI.
