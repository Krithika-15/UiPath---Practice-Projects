# UiBank Loan_Using Web Recorders

## Overview
This UiPath project demonstrates how to use the App/Web Recorder to automate a complete loan application process in a web browser.

The automation opens the UiBank Loan website, fills in required details, submits the application, extracts the generated Loan ID, and displays it in a message box.

## Objective
To understand and practice:
- Using Use Application/Browser activity
- Recording web actions using Web Recorder
- Configuring Click, Type Into, Select Item, and Get Text activities
- Working with input methods and verification
- Extracting dynamic values from web pages

## Application Used
Browser: Chrome
URL: https://uibank.uipath.com/loans

## Workflow Steps
1. Use Browser (Chrome)
    - Opens the UiBank Loan page.
2. Click – "Apply For A Loan"
    - Navigates to the loan application form.
3. Type Into – Loan Amount Requested
    - Enters: 100000
4. Select Item – Loan Term
    - Selects: 5 years
5. Type Into – Current Yearly Income
    - Enters: 600000
6. Type Into – Age
    - Enters: 23
7. Click – Submit Loan Application
8. Get Text – Loan ID
    - Extracts the generated Loan ID
    - Stores it in variable: LoanId
9. Message Box
    - Displays the extracted Loan ID

## Key Concepts Learned
1. How the Web Recorder automatically generates activities inside Use Browser
2. Difference between Click type, Mouse button, and typing options
3. Using Empty field before typing
4. Using Verify text is typed
5. Extracting dynamic data using Get Text
6. Saving extracted value into a variable
7. Editing recorded activities after recording

## Outcome
1. The automation successfully:
2. Fills the loan form automatically
3. Submits the application
4. Captures the system-generated Loan ID
5. Displays it to the user

## Learning Outcome
1. This project helped me understand:
2. How UiPath Web Recorder works internally
3. How recorded activities are structured
4. How to modify and improve recorded steps
5. How to extract and use dynamic web data