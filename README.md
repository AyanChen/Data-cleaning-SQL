This project focuses on cleaning and preparing a dataset of company layoffs using SQL.
The process was carried out in multiple steps to ensure data accuracy, consistency, and usability for further analysis.

Steps Performed:
1)Remove Duplicates — eliminated duplicate records
    -Created staging tables.
    -Identified duplicates using ROW_NUMBER().
    -Removed duplicate rows.
    
2)Standardize the Data — unified formatting (e.g., text, dates)
    -Trimmed extra spaces from company names.
    -Standardized industry names (e.g., all variations of Crypto → Crypto).
    -Cleaned up country names (e.g., United States. → United States).
    
3)Handle Null or Blank Values — processed missing or empty values
    -Replaced empty strings with NULL.
    -Filled missing industry values by referencing other rows from the same company.
    
4)Remove Unnecessary Columns — dropped irrelevant columns that do not add value to analysis
    -Deleted rows where both total_laid_off and percentage_laid_off were missing.
    -Dropped the helper column row_num.

Final Result
The cleaned dataset (layoffs_staging2) is free of duplicates, standardized, consistent, and ready for Exploratory Data Analysis (EDA) or further processing.
