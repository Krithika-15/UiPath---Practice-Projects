# Vegetable Value Calculator

## Overview
This UiPath automation reads a vegetable production Excel file, calculates the **Estimated Value** for each record by multiplying **Quantity × Price per Kg**, and writes the updated data into a **new/updated worksheet**.

## Input File
- **File:** `VegetablesProduction.xlsx`
- **Sheet:** `Tracker`
- **Columns Used:**
  - `Quantity`
  - `Price per Kg`

## Output
- Adds a new column: **Estimated Value**
- Writes the updated DataTable back to Excel (to a new sheet or updated sheet as configured)

## Workflow Logic
1. **Read Range Workbook** → Reads data from Excel into a DataTable (`dt_VegetablesData`)
2. **Add Data Column** → Adds a new column named `Estimated Value`
3. **For Each Row in DataTable**
   - Calculates: `Estimated Value = Quantity * Price per Kg`
   - Stores result into the new column
4. **Write Range Workbook** → Writes the updated DataTable to Excel

## Activities Used
- Read Range Workbook
- Add Data Column
- For Each Row in DataTable
- Assign
- Write Range Workbook

## How to Run
1. Open the project in **UiPath Studio**
2. Place `VegetablesProduction.xlsx` in the project folder (or update the file path in the workflow)
3. Run the workflow
4. Check the output sheet in the same Excel file

## Notes
- Ensure the column names match exactly: `Quantity` and `Price per Kg`
- Recommended data types:
  - Quantity: Integer
  - Price per Kg: Decimal
  - Estimated Value: Decimal