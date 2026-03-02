# UiPath Practice Projects

This repository contains hands-on UiPath automation projects developed while learning through UiPath Academy and practicing real-world business scenarios.

The projects focus on building strong fundamentals in RPA development, including:

- File handling  
- DataTable manipulation  
- Excel automation  
- Web automation  
- Conditional logic  
- Looping mechanisms  
- Workflow modularization  
- Structured automation design  

---

## 🛠 Tools & Technologies

- UiPath Studio (Modern Design Experience)
- Excel (Modern & Workbook Activities)
- DataTable Operations
- File System Automation
- Web Automation
- Table Extraction
- Conditional Logic (If / Switch)
- Looping (For Each / For Each File in Folder)
- Invoke Workflow (Modular Architecture)

---

## 📂 Projects Overview

---

### 1. Separate Invoice by Company Code and Year

Automates invoice classification by extracting company code and year from file names and organizing them into structured folders.

**Concepts Used:**
- String manipulation
- File system activities
- Switch condition
- Folder creation and file movement

---

### 2. Separate Invoice by Company Code

Sorts invoices into company-specific folders using conditional logic and file system automation.

**Concepts Used:**
- For Each File in Folder
- Conditional branching
- Dynamic folder paths

---

### 3. Error Code Classification

Processes an array of error codes and categorizes them based on prefixes ("Ax", "Bx", "Cx") into separate arrays.

**Concepts Used:**
- Arrays
- Substring operations
- Conditional logic
- Looping

---

### 4. Employee Salary Consolidation and Increment Automation
Reads multiple employee Excel files, consolidates them into a single dataset, filters Marketing department employees, applies a salary increment, and generates an updated output report.

**Concepts Used:**
- For Each File in Folder
- DataTable merge & filter
- Salary calculation logic
- Excel report generation

---


### 5. Vegetable Value Calculator

Reads a vegetable production Excel file, calculates **Estimated Value (Quantity × Price per Kg)**, updates the workbook, and generates a Pivot Table with a stacked column chart for summary reporting.

**Concepts Used:**
- Add Data Column
- Data calculation
- Pivot Table creation
- Chart generation
- Re-runnable workflow design

---

### 6. Excel-to-Desktop Transaction Bot

Reads transaction data from an Excel file, enters the values into a desktop application (DoubleUI), retrieves the generated Transaction Number, and writes it back into the same Excel file.

**Concepts Used:**
- Desktop automation
- Input activities (Type Into / Click)
- Data extraction
- Excel integration
- Transaction processing pattern

---

### 7. Invoice Details Extraction – ACME System

Logs into the ACME Test System, searches for invoice details using invoice numbers from an Excel file, extracts relevant invoice data, and updates the output Excel file.

**Concepts Used:**
- Web automation
- Data extraction
- DataTable update
- Modular workflows
- Excel write optimization (write outside loop)

---

### 8. ACME End-to-End Invoice & Work Items Automation

Performs complete end-to-end automation on the ACME portal:

- Logs into ACME
- Processes invoice numbers from Excel
- Extracts:
  - Vendor Tax ID
  - Invoice Item
  - Total
  - Invoice Date
- Generates structured Invoice report
- Navigates to Work Items page
- Extracts Work Items table data
- Generates separate Work Items report
- Logs out securely

**Concepts Used:**
- Modern Web Automation
- Table Extraction
- Invoke Workflow (Modular Design)
- DataTable-based processing
- Performance-optimized Excel writing
- End-to-end orchestration logic

---

### 9. UiBank Loan – Using Web Recorders

Demonstrates App/Web Recorder usage by automating a complete loan application process in a web browser.

The automation:
- Opens the UiBank Loan website
- Fills required details
- Submits the application
- Extracts the generated Loan ID
- Displays it in a message box

**Concepts Used:**
- App/Web Recorder
- Web form automation
- Data extraction
- End-to-end browser automation

---

## 🎯 Skills Demonstrated

- File and folder automation  
- Multi-file Excel processing  
- Data extraction from filenames  
- Excel automation (Workbook & Modern)  
- DataTable merging, filtering, and updating  
- Business rule implementation  
- Web automation & table extraction  
- Desktop automation  
- Modular workflow architecture  
- Performance optimization techniques  
- Structured and scalable automation design  

---

## 📌 Purpose of This Repository

This repository serves as a structured learning portfolio that showcases progressive improvement in UiPath automation skills.

It demonstrates:

- Foundational RPA concepts  
- Real-world business use cases  
- Clean project structuring  
- End-to-end automation solutions  
- Transition from practice-level to developer-level automation design  