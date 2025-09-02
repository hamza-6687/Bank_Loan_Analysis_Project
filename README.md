# 📊 Bank Loan Performance Analysis

_Analyzing loan performance and default risk to support data-driven credit decisions and portfolio optimization using SQL, Python, and Power BI._

---

## 📌 Table of Content

- [Executive Summary](#executive-summary)
- [Business Problem](#business-problem)
- [Dataset](#dataset)
- [Tools & Technologies](#tools--technologies)
- [Project Structure](#project-structure)
- [Dashboard Screenshots](#dashboard-screenshots)
- [Key Portfolio Insights](#key-portfolio-insights)
- [Segmentation Insights](#segmentation-insights)
- [Trend Analysis](#trend-analysis)
- [Recommendations for Management](#recommendations-for-management)
- [Author & Contact](#author--contact)

---

## Executive Summary

The dataset, covering the period from January 2021 to December 2021, consists of approximately 39,000 records across 24 variables.  
During this time, a total of 38.6K loan applications were received, with an overall funded amount of USD 435.8 million. In comparison, the total amount received stood at USD 473.1 million, resulting in a surplus of USD 37.3 million, which is about 8.6% higher than the funded amount.  

This surplus highlights additional financial flexibility and lowers funding risk. Furthermore, the loans carried an average interest rate of 13.5%, reflecting the overall lending landscape during the year.  

From a structural perspective, 60-month loans dominate the portfolio, making up 62.3% of the amount received, while 36-month loans account for 37.7%.  
By loan purpose, Debt Consolidation is the largest category ($0.25B), followed by Credit Card ($0.07B) and Home Improvement ($0.04B).  

Recovery on bad loans is relatively robust at 57%, with $37.3M collected against $65.5M funded, though this results in a loss given default (LGD) of $28.2M.  
The gross portfolio yield stands at 8.6%, reflecting a profitable and growing loan book, though risk concentration in long-tenor loans and specific purposes creates vulnerabilities.  

---

## Business Problem

Effective loan portfolio management is critical for sustaining profitability and reducing risk in the banking and financial industry.  
Banks must ensure they are not incurring losses due to high default rates, risky borrower profiles, or inefficient lending practices.  

The objective of this project is to analyze the bank’s loan portfolio in order to identify key factors influencing borrower repayment behavior and loan defaults.  

By examining borrower characteristics such as debt-to-income ratio, annual income, credit grade, loan term, and loan purpose, good loan vs bad loan.  
The analysis aims to uncover risk patterns and performance trends.  

The ultimate goal is to provide actionable insights that enable the bank to strengthen credit risk management, minimize default rates, and enhance overall profitability through data-driven decision-making.  

---

## Dataset

The dataset used for this analysis comprises loan application records from the bank's internal systems.  
It includes various borrower attributes, loan details, and repayment outcomes.  

Key features of the dataset include:  
- Borrower ID  
- Loan Amount  
- Interest Rate  
- Loan Term  
- Debt-to-Income Ratio  
- Credit Grade  
- Employment title  
- Annual Income  
- Loan Purpose  
- Loan Status  

---

## Tools & Technologies

The following tools and technologies were utilized in this project:  
- SQL (Common Table Expression, Joins, Filtering)  
- Power BI (Interactive Data Visualization)  
- GitHub (Version Control and Collaboration)  

---

## Project Structure

The project follows a structured directory layout to organize the various components effectively.  
Below is an overview of the project structure:  

```bash
bank-loan-performance-analysis/
│── README.md
│── .gitignore
│── Bank Loan Analysis Report.pdf
│── Bank_loan_Analysis_SQL/       # SQL queries and solutions
│── dashboard/                    # Power BI dashboard file
└── Bank Loan Analysis Project.pbix

### Key Portfolio Insights

## Loan Status  
The loan status distribution provides further insight into portfolio health.  

- Currently, there are **1,098 active loans** with **$18.9M funded** and **$24.2M received**.  
- **Charged-off loans** total **5,333**, with **$65.5M funded** and **$37.3M received**.  
- **Fully paid loans** are the majority at **32,145**, representing **$351.4M funded** and **$411.6M received**.  

This equates to a default rate of **13.8% by count**.  

---

## Risk Drivers  
The primary drivers of risk are:  
- Longer-tenor loans  
- Borrowers with higher DTI ratios  
- Riskier purposes such as small business and unsecured “other” categories  

Borrowers with **DTI above 15%** represent elevated risk and should be managed with stricter eligibility or higher pricing.  

---

## Segmentation Insights  

## By Purpose  
- **Debt Consolidation** dominates receipts but poses concentration risk. If underwriting weakens, defaults could increase significantly.  
- **Credit Card** and **Home Improvement** loans are secondary contributors but also warrant close monitoring.  

## By Employment Length  
- Borrowers with stable employment histories, particularly **10+ years**, show stronger repayment performance, contributing **$126M in receipts**.  
- Borrowers with **less than 1 year** of tenure are riskier and should be subject to tighter underwriting.  

## By Term  
- Long-term (**60-month**) loans account for the majority of receipts but create greater duration and LGD risk compared to 36-month loans.  
- Shifting a portion of growth to shorter terms can mitigate these risks.  

---

## Trend Analysis  

## Growth Overview  
Loan receipts have shown a significant upward trajectory over the year, starting at **$28M in January** and rising to **$58M in December**.  
This represents an absolute increase of **$30M** and a percentage growth of approximately **107% year-on-year**.  
In other words, receipts more than doubled within the twelve-month period.  

## Monthly Growth Rate  
The compounding monthly growth rate across this period is estimated at **6.3%**.  
At this pace, receipts could potentially double every 12 months if sustained, underscoring the strong momentum within the portfolio.  

## Seasonal Patterns  
There is evidence of seasonality in the data:  
- Receipts remained modest in the first quarter (**$28M–$32M**), reflecting a slower lending cycle after the holiday season.  
- Inflows increased consistently throughout the year, with the highest volumes in the fourth quarter (**$49M–$58M**), aligning with higher borrowing and spending activity during the holiday and year-end period.  

---

## Recommendations for Management  

- **Tighten Risk Controls:** Limit 60-month exposures within each purpose and set stricter eligibility criteria for high-risk segments.  
- **Dynamic Pricing:** Implement grade-by-purpose price floors to achieve an 80–150 basis point uplift on riskier categories.  
- **Collections Improvement:** Enhance collections processes to lift bad-loan recovery rates from 57% to at least 62%, adding an estimated **$3.3M** in incremental receipts.  
- **Approval Discipline:** Monitor approval rates and post-funding delinquency by channel, pausing underperforming channels.  
- **Scorecard Refresh:** Re-weight key features such as DTI, employment length, purpose, and term to improve predictive accuracy by 3–5%.  

---

## Author & Contact  

**Hamza Tahir**  
_Data Analyst_  
📧 Email: **hamtah4850@gmail.com**  
🔗 [LinkedIn](https://www.linkedin.com/in/hamza-tahir-analyst/)  
