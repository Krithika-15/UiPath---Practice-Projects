# Invoice Details Extraction_ACME System

## Overview
This UiPath automation logs into the ACME Test System, searches for invoice details using invoice numbers from an Excel file, extracts relevant invoice data, and updates the same Excel file with the extracted information.

The automation demonstrates end-to-end web automation, data extraction, DataTable manipulation, and Excel integration.

## 🌐 Application Automated
- Website: https://acme-test.uipath.com
- Module Used: Invoices

## 📂 Input File
- File Name: Vendor_ID_Input.xlsx
- Sheet Name: Sheet1
- Input Column:
    - Invoice Number
    - Output Columns (Updated by Bot):
        - Vendor Tax ID
        - Invoice Item
        - Total
        - Date

## ⚙️ Workflow Steps
### 1️⃣ Login Process
- Open Edge browser
- Navigate to ACME login page
- Enter email and password (secure credential handling)
- Click Login
- Log success message

### 2️⃣ Navigate to Invoices
- Scroll to required section
- Click Invoices
- Click Search for Invoice
- Log navigation steps

### 3️⃣ Read Invoice Numbers from Excel
- Read data from Vendor_ID_Input.xlsx
- Store into DataTable (dt_InvoiceDetails)

### 4️⃣ Process Each Invoice (Loop)
- For each invoice number:
- Type invoice number into search field
- Click Search
- Extract:
    - Vendor Tax ID
    - Invoice Item
    - Total Amount
    - Invoice Date
- Update DataTable using Multiple Assign

### 5️⃣ Logout
Click Log Out

### 6️⃣ Update Excel File
- Write updated DataTable back to Excel
- Start writing from cell A1

## 🛠️ Key Concepts Used
- Browser Automation (Edge)
- Secure Password Handling
- DataTable Manipulation
- For Each Row Loop
- Get Text Activity
- Multiple Assign
- Structured Logging
- Excel Read & Update
- End-to-End Automation Design

## ✅ Output
The Excel file is updated with complete invoice details for all invoice numbers provided in the input sheet.

## 🎯 Learning Outcome
- This project demonstrates:
- Real-world invoice processing automation
- Web data extraction
- Efficient DataTable updating
- Clean workflow structure
- Professional logging and logout handling