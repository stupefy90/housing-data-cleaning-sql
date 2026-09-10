# housing-data-cleaning-sql
My First Data Cleaning Project With SQL
A portfolio project demonstrating data cleaning techniques in MySQL. 

### What I Did:
1. **Created a Staging Table:** Copied the raw data to ensure the original dataset remained untouched.
2. **Removed Duplicates:** Used `ROW_NUMBER()` and a CTE to identify and delete duplicate rows.
3. **Standardized Data:** Cleaned up inconsistent text formatting, trimmed white spaces, and fixed date types.
4. **Handled Nulls:** Evaluated blank and NULL values, using self-joins to populate missing data where possible.
5. **Dropped Unnecessary Data:** Removed redundant columns and temporary tracking rows.

### Files Included:
* `data_cleaning.sql` - Full SQL script containing all queries.
