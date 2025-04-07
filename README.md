# 🧵 SQL String Functions: Filtering & Extracting Text Data
This notebook explores how to use SQL string functions to filter, query, and manipulate text data in your database. These techniques are essential for cleaning messy strings, extracting meaningful patterns, and making your queries more dynamic and readable.

🎓 Developed as part of ExploreAI Academy's Data Science course.
---
## 🎯 Learning Objectives
By the end of this notebook, you will learn how to:

✅ Use the `LIKE` operator to filter rows based on text patterns.

✅ Use the `PRAGMA table_info()` function to read columns characteristics.

✅ Concatenate values from multiple columns using `||` operator in SQLite and other string operations.
---
## 🧰 Tools & Environment
- SQL dialect: MySQL

- Database: `united_nations`

- Table used: `Access_to_Basic_Services`

- Environment: Jupyter Notebook or MySQL Workbench (local setup)
---
## 🧪 Examples of What You’ll Do
1. Filter rows using '%' operator:
```
SELECT * 
FROM Access_to_Basic_Services 
WHERE Country_name LIKE '%(%)%';
```
2. Create a single string by combining multiple column values:
```
SELECT 
    CONCAT(Country_name, ' - ', Time_period) AS Country_Year
FROM Access_to_Basic_Services;
```
---
## 📦 Requirements
Python (for notebook use)

- MySQL database set up locally

- `sqlalchemy + pymysql` (for notebook DB connection)

- Jupyter Notebook or compatible IDE
---
## 📌 Use Cases
- Creating readable column values for reporting

- Text filtering

- Identifying entries with embedded metadata (e.g., text in parentheses)

- Pre-processing text fields for downstream analysis
---
## 👨‍🏫 Developed By
ExploreAI Academy | Modified by **Ibrahim Ambale**

For educational and practical database skill-building
