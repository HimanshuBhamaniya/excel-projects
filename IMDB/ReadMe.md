# IMDB Top 100 Movies Data Cleaning Project

## 📌 Project Overview
This project focuses on cleaning and preparing an IMDB dataset of 100 movies for analysis.  
The dataset contained **11 fields**:
- IMDB Title ID  
- Original Title  
- Release Year  
- Genre  
- Duration  
- Country  
- Content Rating  
- Director  
- Income  
- Votes  
- Score  

---

## 🔎 Initial Observations
- Data was semi‑colon separated.  
- Multiple values spread across columns, requiring consolidation.  
- Release dates were inconsistent, incorrectly formatted, or missing.  
- Duration field contained blanks, improper values, and NaN.  
- Country and Score fields had typos.  
- Income field contained numbers stored as text.  

---

## 🛠️ Cleaning Steps
1. **Appended Multiple Columns**  
   - Consolidated values from multiple columns into a single column where appropriate. 

2. **Converted Semi‑Colon Separated Data**  
   - Used Text to Columns to restructure into tabular format.   

3. **Standardized Release Dates**  
   - Fixed inconsistent formats (e.g., `23rd of December 1966` → `12/23/1966`).  
   - Corrected invalid dates using verified sources (e.g., *Scarface*, *Taxi Driver*).  

4. **Duration Field Cleanup**  
   - Fixed improper values.  
   - Converted blanks and NaN into a uniform `NaN`.  

5. **Country and Score Fields**  
   - Corrected typos to ensure consistency.  

6. **Income Field Conversion**  
   - Converted values stored as text into proper numeric format.  

---

## 📊 Notes
- Dataset is now standardized and reliable.  
- All fields cleaned for consistency and accuracy.  
- Ready for further analysis, visualization, or integration into larger projects.  

---

## 🎯 Purpose
This project demonstrates a structured approach to cleaning movie datasets in Excel, ensuring accurate dates, consistent numeric fields, and corrected categorical values for meaningful analysis.
