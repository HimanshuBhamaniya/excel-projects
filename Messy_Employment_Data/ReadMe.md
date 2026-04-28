# Employment Survey Data Cleaning Project

## 📌 Project Overview
This project focuses on cleaning and preparing an employment survey dataset from India for research purposes.  
The dataset originally contained **15,208 records** across 9 fields:
- Status  
- Age Group  
- Education  
- Industry  
- Location  
- AI Risk  
- Years of Experience  
- Monthly Salary (INR)  
- Date Recorded  

---

## 🔎 Initial Observations
- Numerous blank cells across multiple fields (common in survey data).  
- Improper character case in field values.  
- Extra spaces before text values.  

---

## 🛠️ Cleaning Steps
1. **Standardized Text Case**  
   - Applied `PROPER` function to fix inconsistent capitalization.  

2. **Removed Extra Spaces**  
   - Used Find & Replace to eliminate leading/trailing spaces.  

3. **Handled Missing Values**  
   - Removed all records containing any blank fields.  
   - Decision made because survey datasets are used for research, and incomplete records reduce reliability.  

---

## 📊 Notes
- Dataset reduced to complete records only.  
- All transformations applied consistently.  
- Final dataset is clean, standardized, and ready for further analysis.  

---

## 🎯 Purpose
This project demonstrates a structured approach to cleaning survey data in Excel, ensuring that only complete and reliable records are retained for research and analysis.
