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
 - Total Inflow                
 - Total Outflow                
 - Top Debit Amount             
 - Top Debit Weekday              
 - Top Credit Amount                  
 - Top Credit Weekday
 - Selected Weekday
 - Closing Balance
 - Payment Type
 - Opening Balance
 - Net Movement
 - Net Flow
 - Highest Credit
 - Highest Debit
 - Interactive Title
   
  **Purpose**
  To analyze bank statement data in order to track cash flow, understand spending patterns, detect transaction trends, and support better financial planning and decision-making.

## Data Analysis and Visualization

The dashboard is structured into a page,which focuses on Total transactions, Total Inflow, Total Outflow, Highest Credit and Average balance.

## Page 1:Overall Insight

**Ovearall Insights**
<img width="894" height="505" alt="Bank Statement" src="https://github.com/user-attachments/assets/ce691c04-fe4a-4d96-8427-5c45dbdc85e7" />

# Key Metrics( Top of the page): Total Transations, Total Inflow, Total Outflow, Average balance, Highest Credit.
- **Dynamic Title:** is a title that changes automatically based on data or filters applied.
- **Total Transations:** The total number of all money activities (credits and debits) in the account within the month July.
- **Total Inflow:** The total amount of money received into the account.
- **Total Outflow:** The total amount of money sent out or spent from the account.
- **Average balance:** The average amount of money in the account over the period in July.
- **Highest Credit:** The single largest amount of money received in one transaction.

This KPIs helps  understand spending patterns, detect transaction trends, and support better financial planning and decision-making.

-------

## Visuals
-**Total Inflow and Total Outflow (Pie Chart):** It represents the distribution of Inflow and Outflow of cash in percentage making it easy to identify.
-**Debit by Day of the week (Column Chart):** It represents the amount debited for each weekday.
-**Credit by Day of the week (Column Chart):** It represents the amount credited for each day of the week.
-**Debit by Payment type (Column Chart):** It represent the type of payment in which money is debited for.
-**Debit and Credit by day (Line Chart):** It represent the credit and debit for the duration of the month in days.

## Slicers: Transaction date and Day of the week.

The dashboard includes Transaction date and Day of the week which would help identify transactions easily for a specific period of time.

This interactve fliters ensures the Title ,KPIs, charts and visuals adapts instantly which gives easy access to identify specific dates.

# Key Analysis Findings

This bank statement analysis provided insights the inflow, Outflow which helped to understand spending patterns and detect transaction trends.

- **Total Transactions-** *86*
- **Total Inflow-** *5.63M*
- **total Outflow-** *5.58M*
- **Netflow-** *54.14K*
- **Highest Credit-** *1.44M*
- **Highest Debit-** *1.00M*
- **Opening Balance-** *740.15K*
- **Closing Balance-** *1.29M*
- **Net Movement-** *554.29K*
- **Average Balance-** *968.74K*
- **Top Debit Weekday-** *Monday*
- **Top Credit Weekday-** *Thursday*
- **Top Debit Amount-** *1.94M*
- **Top Credit Amount-** *2.02M*
- **Lowest Debit Weekday-** *Friday*
- **Lowest Credit Weekday-** *Tuesday*
- The originating branch is *635 Akin Adesola.

# Overall Insights
- Total inflow **(5.63M)** is almost equal to total outflow **(5.58M)**.
- The pie chart confirms a near **50/50** split, meaning the account is **financially stable but not strongly accumulating cash**.
- The difference between inflow and outflow is very small, showing minimal profit/retention **(low netflow)**.
- **86** transactions indicate consistent account usage and active financial movement.
- Debit peaks on Monday **(1.94M)** → likely operational or start-of-week spending.
- Credit peaks on Thursday **(2.02M)** → strongest inflow day, possibly settlements or business payments.
- Lowest activity days: Tuesday **(credit)** and Friday **(debit)**, showing uneven mid-week activity flow.
- Debits are mainly driven by:
    - **TRA (3.1M) and NIB (2.5M)** → major contributors to outflow.
- Other channels (AIR, ELE, VAT, etc.) are almost negligible.
- Average balance **(968.74K)** shows the account maintains a mid-level liquidity buffer without major spikes or drops.
- The line chart shows irregular spikes in both debit and credit, suggesting:
     - Non-daily bulk transactions
     - Periodic business inflows/outflows rather than steady daily flow.
       
 # Recomendations 

  Based on the analysis, the following recommendations can help improve spending patterns:
  
- Since inflow ≈ outflow, focus on **increasing revenue streams or reducing high-cost debits (TRA, NIB)**.
- Strengthen financial activity around **Thursdays (best credit day)** for collections or settlements.
- Investigate **TRA and NIB payments**, as they account for most outflows.
- Consider optimizing or negotiating recurring charges.
- Smooth out irregular spikes by **spreading payments more evenly across the week**.
- Encourage inflows on **Tuesdays and Fridays** to avoid weak cash days.

# Limitations

- The analysis is limited to July, so seasonal or long-term trends cannot be confirmed.
- There is no reference to other months or branches for performance comparison.
 
