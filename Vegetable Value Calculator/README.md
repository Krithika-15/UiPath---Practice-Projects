# Vegetable Value Calculator

## Overview
This UiPath automation reads a vegetable production Excel file, calculates the **Estimated Value** (Quantity × Price per Kg), updates the workbook, and generates a Pivot Table with a stacked column chart for summary reporting.

## Input
- File: `VegetablesProduction.xlsx`
- Sheet: `Tracker`
- Key Columns:
  - Quantity
  - Price per Kg
  - Vendor Name
  - Production Month
  - Storage Zone

## Process
1. Read Excel data into a DataTable  
2. Check if **Estimated Value** column exists  
3. Add column (if not present)  
4. Calculate Estimated Value for each row  
5. Write updated data back to Excel  
6. Create Pivot Table summary  
7. Insert and update chart  

## Output
- Updated worksheet with calculated values  
- Pivot Table summary  
- Stacked column chart titled **"Estimated Sales"**

## Key Features
- Re-runnable workflow  
- Automated calculation logic  
- Pivot-based summarization  
- Chart generation  
- End-to-end Excel reporting automation