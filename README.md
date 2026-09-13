# World Layoffs SQL Project: Data Cleaning & Exploratory Data Analysis

A comprehensive data portfolio project demonstrating end-to-end data manipulation, cleaning, and advanced analytical queries using MySQL.
---
## Phase 1: Data Cleaning
The objective of this phase was to take raw layoff records and transform them into a clean, structured format ready for analysis, ensuring the original dataset remained untouched.

### What I Did:
* **Created a Staging Table:** Copied the raw data into a separate staging table to preserve data integrity.
* **Removed Duplicates:** Used `ROW_NUMBER()` and window functions partitioned across all relevant columns to identify and delete duplicate rows.
* **Standardized Data:** Cleaned up inconsistent text formatting, trimmed white spaces, and corrected date types.
* **Handled Nulls:** Evaluated blank and `NULL` values, utilizing self-joins to populate missing information where applicable.
* **Dropped Unnecessary Data:** Removed redundant columns and temporary tracking variables (like row numbers).
---
## Phase 2: Exploratory Data Analysis (EDA)
After cleaning the dataset, this phase focused on querying the data to uncover trends, patterns, and insights regarding global layoffs.

### Key Analysis Performed:
* **Overview & Extremes:** Examined maximum total layoffs and maximum percentage laid off (identifying companies that went completely under).
* **Company & Industry Trends:** Aggregated total layoffs grouped by company and industry to find the hardest-hit sectors.
* **Temporal Trends:** Analyzed layoffs broken down by year and month to track chronological spikes.
* **Rolling Totals:** Used Common Table Expressions (CTEs) and window functions (`SUM() OVER`) to calculate a running progression of layoffs over time.
* **Company Rankings:** Utilized `DENSE_RANK()` partitioned by years to find the top 5 companies with the most layoffs each year.

## Repository Files
* `data_cleaning.sql` — The complete script containing all data cleaning queries.
* `exploratory_data_analysis.sql` — The complete script containing all EDA and advanced analytical queries.
