# ACME End-to-End Invoice and Work Item Automation

## Overview

This UiPath automation project (Modern Design Experience) performs end-to-end web data extraction from the ACME system.

The bot:

- Logs into the ACME portal  
- Processes invoice numbers from an input Excel file  
- Extracts invoice details  
- Generates an invoice report  
- Extracts Work Items table data  
- Saves structured Excel outputs in the project folder  
- Logs out securely  

---

## Business Objective

To automate the manual process of:

- Searching invoices individually  
- Copying invoice details  
- Extracting Work Items table data  
- Preparing Excel reports  

This automation improves processing speed, reduces manual errors, and ensures structured reporting.

---

## Project Structure

### Main.xaml

Controls the entire execution flow:

1. Login to ACME Webpage
2. Navigate to Invoice Search  
3. Process all invoices  
4. Write invoice output  
5. Navigate to Work Items Page
6. Extract Work Items data  
7. Logout  

---

## Invoice Processing Workflow

### Input

- File: `Vendor_ID_Input.xlsx`  
- Location: `Input` folder  
- Contains: Invoice Numbers  

### Process

1. Read invoice numbers into DataTable `dt_InvoiceNumbers`
2. For each invoice number:
   - Search invoice in ACME
   - Extract:
     - Vendor Tax ID
     - Invoice Item
     - Total Amount
     - Invoice Date
   - Update the corresponding row in the DataTable
   - Navigate back to search page
3. After completing the loop, write updated DataTable to:
Output\Invoice_Data_Extraction.xlsx


> Writing to Excel is performed **outside the loop** to improve performance and avoid Excel locking issues.

---

## Work Items Extraction Workflow

1. Navigate to Home → Work Items page  
2. Extract table fields:
   - WIID  
   - Description  
   - Type  
   - Status  
   - Date  
3. Write extracted data to:
Output\Work_Items_Data_<Date>.xlsx


---

## Modular Workflow Files

- `ACME_WebPage_Login.xaml`  
- `Navigate_To_Search_Invoice.xaml`  
- `Search_For_Current_InvoiceNumber.xaml`  
- `Extract_InvoiceDetails.xaml`  
- `Navigate_BackTo_Search_Invoice.xaml`  
- `Extract_WorkItems.xaml`  
- `ACME_WebPage_LogOut.xaml`  
- `Main.xaml`  

Each workflow is modularized for reusability and clean separation of responsibilities.

---

## Output

- `Invoice_Data_Extraction.xlsx`  
- `Work_Items_Data_<Date>.xlsx`  

All output files are stored inside the `Output` folder.

---

## Key Technical Concepts Used

- Modern Design Experience  
- Use Application/Browser  
- Invoke Workflow File  
- For Each Row in DataTable  
- Multiple Assign  
- Table Extraction  
- Excel (Modern & Workbook activities)  
- Structured logging  
- Modular architecture  

---

## Performance Optimization

- DataTable is updated in memory during invoice processing.
- Excel write operation is executed only once after loop completion.
- Modular XAML design improves maintainability and scalability.

---

## Learning Outcomes

This project demonstrates:

- End-to-end web automation  
- Excel-driven transaction processing  
- Structured data extraction  
- Table extraction techniques  
- Clean orchestration logic  
- Professional RPA project structuring  
