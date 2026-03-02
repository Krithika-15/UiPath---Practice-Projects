ACME End-to-End Invoice & Work Items Automation
📌 Overview

This UiPath automation project (Modern Design Experience) performs end-to-end web data extraction from the ACME system.

The bot:

Logs into the ACME portal

Processes invoice numbers from an input Excel file

Extracts invoice details

Generates an invoice report

Extracts Work Items table data

Saves structured Excel outputs in the project folder

Logs out securely

🎯 Business Objective

To automate the manual process of:

Searching invoices individually

Copying invoice details

Extracting Work Items table data

Preparing Excel reports

This automation improves processing speed, reduces manual errors, and ensures structured reporting.

🏗 Project Structure
Main.xaml

Controls the entire process flow:

Login

Navigate to Invoice Search

Process invoices

Write invoice output

Extract Work Items

Logout

📂 Modular Workflows

ACME_WebPage_Login.xaml

Navigate_To_Search_Invoice.xaml

Search_For_Current_InvoiceNumber.xaml

Extract_InvoiceDetails.xaml

Navigate_BackTo_Search_Invoice.xaml

Extract_WorkItems.xaml

ACME_WebPage_LogOut.xaml

Each workflow is designed for reusability and clean separation of responsibilities.

🔄 Functional Workflow
1️⃣ Login Process

Prompts user for email and password

Logs into ACME web portal

2️⃣ Invoice Processing
Step 1: Read Input File

Reads invoice numbers from:

Input\Vendor_ID_Input.xlsx

Stores data in DataTable: dt_InvoiceNumbers

Step 2: Process Each Invoice

For each invoice number:

Search invoice in ACME

Extract:

Vendor Tax ID

Invoice Item

Total Amount

Invoice Date

Update the corresponding row in dt_InvoiceNumbers

Navigate back to Search page

Step 3: Write Invoice Output

After completing the loop:

Writes updated dt_InvoiceNumbers to:

Output\Invoice_Data_Extraction.xlsx

✅ Writing is done outside the loop for better performance and to prevent Excel locking issues.

3️⃣ Work Items Table Extraction

Navigates to Work Items page

Extracts table fields:

WIID

Description

Type

Status

Date

Writes output to:

Output\Work_Items_Data_<Date>.xlsx
4️⃣ Logout

Logs out from ACME system

Closes session cleanly

📥 Input & 📤 Output
Input

Vendor_ID_Input.xlsx (Contains invoice numbers)

Output

Invoice_Data_Extraction.xlsx

Work_Items_Data_<Date>.xlsx

All files are stored inside the project Input and Output folders.

🛠 Key Technical Concepts Used

Modern Design Experience

Use Application/Browser

Invoke Workflow

For Each Row in DataTable

Multiple Assign

Table Extraction

Excel (Workbook & Modern Excel activities)

Structured Logging

Modular workflow architecture

⚡ Performance Optimization

DataTable is updated in memory during the loop.

Excel write operation is executed only once after loop completion.

Modular XAML design improves maintainability and scalability.

📚 Learning Outcomes

This project demonstrates:

End-to-end web automation

Excel-driven transaction processing

Structured data extraction

Table extraction techniques

Clean orchestration logic

Professional RPA project structuring