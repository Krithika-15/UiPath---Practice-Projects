# Employee Salary Consolidation and Increment Automation
- Built using: UiPath Studio
- Type: RPA – Excel Automation

## 📌 Overview
This UiPath automation reads multiple employee Excel reports from a folder, consolidates them into a single dataset, filters Marketing department employees, applies a salary increment, and generates an updated output report.

## ⚙️ Activities Used
- For Each File in Folder
- Read Range (Workbook)
- Merge Data Table
- Filter Data Table
- For Each Row
- Assign (Salary Calculation)
- Write Range (Workbook)

## 🔄 Process Flow

- Loops through multiple input Excel files.
- Reads employee data from each file into DataTables.
- Merges all data into one consolidated DataTable.
- Filters employees belonging to the Marketing department.
- Iterates through filtered records.
- Applies salary increment logic.
- Writes the updated employee data into a new Excel report.

## 🎯 Key Features
- Multi-file Excel processing
- DataTable manipulation
- Conditional filtering
- Business rule-based salary increment
- Automated output generation

## 🛠 Skills Demonstrated
- DataTable handling
- Looping and conditional logic
- Excel automation using Workbook activities
- Structured workflow design
- Real-world business scenario implementation