# Cafe Sales Data Cleaning Project

## Overview
This project focuses on cleaning and preparing a café sales dataset for further analysis.  
The dataset originally contained **10,001 records** across 8 columns:
- Transaction ID  
- Item  
- Quantity  
- Price Per Unit  
- Total Spent  
- Payment Method  
- Location  
- Transaction Date  

The primary objective was to handle missing, invalid, and inconsistent values to ensure the dataset is reliable for analysis.

---

## Initial Observations
- Numerous **missing values** (blank cells) across most columns.  
- **Invalid entries** such as `"ERROR"` and `"UNKNOWN"`.  
- Transaction Date column had valid entries only up to **12/31/2023**; later entries were blank or invalid.  
- Transaction ID was already clean and required no changes.

---

## Cleaning Steps
1. **Replaced Invalid Values**
   - Converted `"ERROR"` and `"UNKNOWN"` to `NaN` or contextually appropriate values.
   - Used Excel functions like **VLOOKUP** and **INDEX-MATCH** to fill missing or incorrect values from reference data.

2. **Handled Missing Values**
   - Filled blank cells with `"UNKNOWN"` or appropriate replacements.
   - Missing prices were filled using a reference price list.

3. **Transaction Date Column**
   - Dates beyond 12/31/2023 were marked as invalid.
   - Invalid dates replaced with `NaN`; blanks filled with `"UNKNOWN"` for clarity.

---

## Notes
- All replacements and imputations were documented and applied consistently.  
- The cleaned dataset is now ready for analysis, with missing or uncertain values clearly marked.  

---

## Purpose
This project demonstrates a structured approach to **data preparation and cleaning** in Excel, ensuring that raw, messy data is transformed into a reliable dataset suitable for analysis and reporting.

---

📌 *Future work may include exploratory data analysis (EDA), visualization, and building dashboards to uncover insights from the cleaned dataset.*
