# Data Cleaning Summary – Messy HR Dataset

## Dataset Overview
- **Fields (10):** Name, Age, Salary, Gender, Department, Position, Joining Date, Performance, Email, Phone Number  
- **Objective:** Clean and prepare HR data for reliable analysis by fixing inconsistent formats, missing values, and invalid entries.

---

## Initial Observations
- **Name:** All values were in lowercase.  
- **Age & Salary:** Contained mixed text and numeric values (e.g., "thirty", "30", "sixty thousand", "65000").  
- **Joining Date:** Multiple inconsistent formats (e.g., `April 5, 2018`, `01/01/2000`, `01-01-2000`, `2000.12.01`).  
- **Email, Age, Salary, Phone Number:** Included missing values, `nan`, and `NAN`.  
- **Gender, Department, Position:** Clean — no missing values, case issues, or invalid entries.  
- **Duplicates:** None found.

---

## Cleaning Steps
1. **Name Field**
   - Applied `PROPER` function to convert lowercase names into proper case.

2. **Handling Missing Values**
   - Replaced `nan`, `NAN`, and blanks with `"UNKNOWN"` (except Salary, where blanks were preserved to avoid calculation errors).

3. **Age & Salary Fields**
   - Converted text values into appropriate numeric values (e.g., `"thirty"` → `30`, `"sixty thousand"` → `60000`).

4. **Joining Date Field**
   - Standardized formats by replacing separators (`/`, `.`, `,`) with `-` using Find & Replace.
   - Ensured consistent date formatting across all records.

5. **Salary Field**
   - Left blanks for missing values to prevent interference with calculations.

---

## Notes
- No duplicate records were present.  
- All replacements and transformations were documented and applied consistently.  
- The dataset is now standardized and ready for analysis.

---

📌 *This project demonstrates a structured approach to cleaning HR data in Excel, ensuring consistency and reliability for further analysis.*
