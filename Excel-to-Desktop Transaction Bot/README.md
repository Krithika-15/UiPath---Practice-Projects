# Excel-To-Desktop Transaction Bot

## Overview

This UiPath automation reads transaction data from an Excel file, enters the values into a desktop application (DoubleUI), retrieves the generated Transaction Number, and writes it back into the same Excel file.

## Input
- File Name: DoubleUI-Transactions.xlsx
- Sheet Name: Sheet1
- Columns Used:
    - CashIn
    - OnUsCheck
    - Transaction Number (Output column)

## Workflow Steps
1. Use Application/Browser → Opens doubleui.exe
2. Read Range Workbook → Reads Excel data into dt_Transaction
3. For Each Row in DataTable
4. Type CashIn value into the application
5. Type OnUsCheck value into the application
6. Click Accept
7. Extract generated Transaction Number
8. Write the Transaction Number into Column C of Excel
9. Repeat until all rows are processed.

## Output
The Excel file is updated with generated Transaction Numbers in Column C for each processed transaction.

## Learning Outcome
This project demonstrates:
- Desktop application automation
- Excel Workbook activities
- Looping and iteration logic
- Variable scope importance
- Debugging using breakpoints