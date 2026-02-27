# UiBank Loan_Using Web Recorders

## Overview
This UiPath project demonstrates how to use the App/Web Recorder to automate a complete loan application process in a web browser.
The automation opens the UiBank Loan website, fills in required details, submits the application, extracts the generated Loan ID, and displays it in a message box.

## Objective
To understand and practice:
Using Use Application/Browser activity
Recording web actions using Web Recorder
Configuring Click, Type Into, Select Item, and Get Text activities
Working with input methods and verification
Extracting dynamic values from web pages

## Application Used
Browser: Chrome
URL: https://uibank.uipath.com/loans

## Workflow Steps
Use Browser (Chrome)
Opens the UiBank Loan page.
Click – "Apply For A Loan"
Navigates to the loan application form.
Type Into – Loan Amount Requested
Enters: 100000
Select Item – Loan Term
Selects: 5 years
Type Into – Current Yearly Income
Enters: 600000
Type Into – Age
Enters: 23
Click – Submit Loan Application
Get Text – Loan ID
Extracts the generated Loan ID
Stores it in variable: LoanId
Message Box
Displays the extracted Loan ID

## Key Concepts Learned
How the Web Recorder automatically generates activities inside Use Browser
Difference between Click type, Mouse button, and typing options
Using Empty field before typing
Using Verify text is typed
Extracting dynamic data using Get Text
Saving extracted value into a variable
Editing recorded activities after recording

## Outcome
The automation successfully:
Fills the loan form automatically
Submits the application
Captures the system-generated Loan ID
Displays it to the user

## Learning Outcome
This project helped me understand:
How UiPath Web Recorder works internally
How recorded activities are structured
How to modify and improve recorded steps
How to extract and use dynamic web data