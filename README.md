# Telco Customer Churn Analysis

# Project Overview
 The project explores Telco Customer Churn dataset. The goal was to identify key factors driving customer churn and its impact on revenue. 
 I used Python and Pandas for Data Analysis and Matplotlib for Data Visualization. 
## Problem
Customer churn directly erodes recurring revenue, and acquiring a new 
customer typically costs more than retaining an existing one. Telco needed to 
understand which customers were most likely to churn and why, in order to 
prioritize retention spend where it would have the greatest impact
## Dataset 
- Telco Customer Churn Dataset.
- The dataset has column such as customer id, contract type, payment method, 
  tenure, churn status and monthly/total charges.
  

## Tools 
- Google Colab
- Python
- Pandas(data cleaning and analysis)
- Matplotlib(data visualization)

## Methodology
1. Data Inspection & Cleaning - Loaded the dataset into Pandas, inspected it 
   with .head(), .shape, .info(), and checked for missing values. Found 
   whitespace-only entries in 'TotalCharges' column customer with 0 tenure, 
   stripped and replaced them with '0.0', then converted the column to float.
2. Churn Analysis - Calculated the overall churn rate, then broke it down by 
   contract type and payment method individually, and by both combined, to find 
   the highest-risk customer segment.
3. Revenue Analysis - Summed 'Monthly Charges' column for churned vs. stayed 
   customers to quantify revenue at risk, both in aggregate and segmented by 
   contract type and payment method, then annualized the monthly loss.
4. Built four visuals in Matplotlib (histogram, boxplot, grouped bar, bar 
   chart) to communicate each finding visually, using consistent color coding 
   (crimson = churned, steelblue = stayed) throughout.
   

## Findings
- Telco is losing 26% of its customers.
- Customers on month-to-month contract are most likely to leave. About 43% of 
  them churn.
- Customers who pay using electronic check have the highest churn rate, with 
  45% leaving the company.
- Customers who use electronic check and are on month-to-month contract have 
  the highest churn rate at 54%.
- Most customers who churn leave within the first 12 months and churn is 
  heavily concentrated in the 0-6 month window.
  
- Churned customers cluster tightly at low tenure while customers who stay show
  a much wider spread.
  
- Churn decreases as customer tenure increases. Customers who stay for more than two years are much less likely to churn.

## Impact on Business
- About 30.5% of monthly revenue is associated with customers who churn, which 
  is approximately $139130.85 per month.
- Customers on month-to-month contracts account for approximately $120,847.10 
  in monthly revenue associated with churn.
- Customers paying through electronic check account for approximately 
  $84,288.75 in monthly revenue associated with churn.
- This represents approximately $1,669,570.20 in annualized revenue at risk if 
  current churn levels continue.

## Recommendations.
- Focus retention efforts on customers during their first 12 months, since this 
  is when most churn occurs.
- Encourage customers on month-to-month contracts to switch to longer-term 
  contracts by offering discounts.
- Investigate why customers paying by electronic check churn at a higher rate 
  and address any issues (e.g. lack of autopay, failed payment) that may be 
  contributing to it.

## How to Run
- Open the notebook in Google Colab.
- The dataset is loaded directly from the source URL.
- Run the cell.
- Note: The note book covers inspections, cleaning, churn analysis, revenue analysis and visualization. 
