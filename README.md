## Introduction ##

This project **Bank Statement** report is designed to analysis the cash inflow and outflow for the month July.

The reports explores
- Total Transactions
- Inflow
- Outflow
  
  It purpose is to how money is being spent for the duration of the month July.
  
# Problem Statement
The account holder is experiencing challenges in tracking monthly inflows, outflows, and spending patterns, making financial monitoring and decision making difficult. There is a need to analyze transaction trends,account balances, and expenditure behaviour to gain meaningful finanacial insights.

This project addresses these challenges by transforming one month's bank statement data into useful insights using PowerBI, highlighting cashflow, spending patterns, transaction categories and balance movements.

# Key Questions
- What is the total number of transactions recorded during the month?
- What are the total cash inflows,total cash outflows and net cash flow for the period?
- What were the highest credit and highest debit transactions recorded?
- What were the opening balance, closing balance, net movement, and average account balance during the month?
- What day of the week recorded the highest number of debit transactions?
- What day of the week recorded the highest number of credit transactions?
- What day of the week had the highest volume of transactions overall?
- What day recorded the highest debit amount and highest credit amount?
- What are the major spending patterns observed in the account?
- What trends or insights can be derived from the account's transaction behavior and cashflow movements?
  
# Dataset Overview

This dataset contains **86 Transations** it captured detailed informations like Transaction date, Value date, Debit, Credit, Balance, Originating Branch and Remarks.

-**Transaction date** - The date the transaction was initiated. 
-**Value date** - The date the transaction takes effecton the account balance.
-**Debit** - Money taken out of the account.
-**Credit** - Money paid into the account. 
-**Balance** - The ammount of money in the account after a transaction.
-**Originating Branch** - The bank branch where the transaction was processed.
-**Remarks** - A brief description or narration of the transaction.
-**Net Transaction** - The difference between total credits and total debits.
-**Day of the week** - The weekday the transaction occurred.
-**Week Number** - The specific week of the month or year in which the transaction occured.
-**Payment Type** - The method used for the transaction, such as transfer, ATM withdrawal, POS, or deposit.

# Data Preparation
To ensure accuracy, the dataset underwent a series of **cleaning and transformation steps** before analysis.This process was taken into **Excel** and **PowerBI** focusing on recovering inconsistencies, deriving new fields and preparing the data for visualization.

### Key Steps taken
- Downloaded the account statement from email.
- Used PDFgear to convert into excel files.
- Used the function **Textjoin** to close the unnecessary spacing in the texts in **Excel**.
- Loaded the into **PowerBI**
- Created a column to calculate Net transaction.
- Created a column to calculate Day of the week.
- Created a column to calculate Weeknumber.
- Created a column to extrate Payment type from the remark column given.
- Loaded the cleaned dataset into **PowerBI**  for the chart modelling.

 # Measures (DAX)
 **Description**
 Contains calculated measures created using **DAX function** in **PowerBI** to define key KPIs and evaluate the transactions for the month. These measures form the backbone of the dashboard, providing insights to the Inflow and Outflow of money.

 **Fields**
 - Total Transaction.    - Selected Day         - Average Balance
 - Total Inflow          - Selected Weekday     - Closing Balance
 - Total Outflow         - Payment Type         - Highest Credit
 - Top Debit Amount      - Opening Balance      - Highest Debit
 - Top Debit Weekday     - Net Movement         - Interactive Title
 - Top Credit Amount     - Net Flow             - Top Credit Weekday

  **Purpose**
  To analyze bank statement data in order to track cash flow, understand spending patterns, detect transaction trends, and support better financial planning and decision-making.

## Data Analysis and Visualization

The dashboard is structured into a page,which focuses on Total transactions, Total Inflow, Total Outflow, Highest Credit and Average balance.

## Page 1:Overall Insight

**Ovearall Insights**
<img width="894" height="505" alt="Bank Statement" src="https://github.com/user-attachments/assets/ce691c04-fe4a-4d96-8427-5c45dbdc85e7" />

# Key Metrics( Top of the page): Total Transations, Total Inflow, Total Outflow, Average balance, Highest Credit.

- *Total Transations:*
- Total Inflow:
- Total Outflow:
- Average balance:
- Highest Credit:
