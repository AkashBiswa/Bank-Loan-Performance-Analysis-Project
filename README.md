# Bank Loan Report Dashboard

## Project Summary

This project presents an end-to-end data analytics solution for monitoring and evaluating a bank’s loan portfolio. By combining SQL-based data analysis with interactive Tableau dashboards, it delivers actionable insights into loan performance, borrower behavior, and financial risk.

## Objectives

* Track loan application trends over time
* Evaluate funding and repayment performance
* Distinguish between good and bad loans
* Identify key factors influencing lending decisions
* Support data-driven financial strategy


## Tech Stack

* MySQL
* Tableau


## Dataset

* File: `financial_loan_data_excel.xlsx`


## Key KPIs

### Lending Performance

* Total Loan Applications
* Total Funded Amount
* Total Amount Received
* Month-to-Date (MTD) Metrics
* Month-over-Month (MoM) Changes

### Risk Metrics

* Average Interest Rate
* Average Debt-to-Income Ratio (DTI)

### Loan Quality

**Good Loans (Fully Paid, Current)**

* Percentage of Good Loans
* Total Applications
* Funded Amount
* Amount Received

**Bad Loans (Charged Off)**

* Percentage of Bad Loans
* Total Applications
* Funded Amount
* Amount Received

### Dashboard Interation

* [View Dashboard](https://public.tableau.com/views/BankLoanReportDashboard_17746858234880/Summary?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

<img width="1000" height="649" alt="1" src="https://github.com/user-attachments/assets/e0434c42-d453-4a14-a22f-a9990525d622" />



## Project Workflow

### 1. Data Import

* Loaded CSV data into MySQL using `LOAD DATA INFILE`

### 2. Data Preparation

* Cleaned and validated data
* Standardized categorical fields
* Checked for missing or inconsistent values

### 3. Data Analysis

* Used SQL aggregations (SUM, COUNT, AVG)
* Created time-based metrics (MTD, PMTD, MoM)
* Segmented loans into good and bad categories

### 4. Data Visualization

Developed three interactive dashboards in Tableau:

#### Summary Dashboard

* KPI overview
* Good vs Bad loan comparison
* Loan status breakdown

#### Overview Dashboard

* Monthly trends
* Regional distribution
* Loan term analysis
* Employment length insights
* Loan purpose breakdown
* Home ownership distribution

#### Details Dashboard

* Consolidated loan-level data
* Interactive filtering for detailed exploration


## Key Insights

* The bank processed 38.5K loan applications with total funding of $435.7M and $473.0M received, indicating strong profitability.
* There is consistent month-over-month growth in applications, funding, and repayments, showing increasing lending activity.
* The average interest rate (~12%) has slightly increased, contributing to higher returns.
* Average DTI (~13.3%) shows a moderate borrower risk level with a slight upward trend.
* 86.17% of loans are performing (Good Loans), reflecting a healthy portfolio.
* 13.82% are charged-off loans, causing a significant gap between funded and recovered amounts, indicating credit risk exposure.


## Business Recommendations

* Improve credit risk assessment to reduce charged-off loans
* Implement risk-based pricing for high-risk borrowers
* Monitor and control DTI thresholds during loan approval
* Focus on high-performing customer segments
* Maintain a balance between growth and risk management

## Conclusion

The loan portfolio is financially strong and growing, with stable returns and a high proportion of good loans. However, the presence of bad loans (~14%) and rising borrower risk (DTI) suggests the need for improved risk control to sustain long-term performance.

## Future Enhancements

* Predictive modeling for loan default risk
* Real-time data integration
* Deployment as an interactive web application
