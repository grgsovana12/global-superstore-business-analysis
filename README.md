# Global Superstore — Business Analysis & Data Quality Assessment

## Project Overview

This project analyzes the Global Superstore dataset to evaluate retail sales performance, product profitability, customer segments, shipping costs, discounts, and data quality.

The goal was to turn historical transaction data into actionable business insights while identifying data quality issues that could affect reporting and decision-making.

## Project Objectives

- Evaluate overall sales, profit, and profitability.
- Identify top-performing and underperforming products.
- Compare performance across categories and customer segments.
- Examine relationships between discounts, shipping costs, and profitability.
- Perform data quality checks and document exceptions.
- Present findings through a Tableau dashboard and business analysis report.

## Tools & Technologies

- SQL
- Python
- Tableau Public
- Excel
- Business Requirements Documentation (BRD)
- Data Quality Testing

## Dataset Overview

- Records: 51,290
- Fields: 27
- Period: 2011–2014

## Key Business Findings

- Total sales were approximately $12.64 million.
- Total profit was approximately $1.47 million.
- Overall profit margin was 11.61%.
- Technology had the highest category sales, at approximately $4.74 million.
- Furniture had a lower profit margin than the other major categories, at 6.94%.
- Home Office had the highest customer-segment profit margin, at 11.99%.
- The Tables sub-category generated approximately $64,083 in losses, with an overall margin of -8.47%.
- Higher discount levels were associated with weaker profitability in the analyzed data.

## Data Quality Assessment

Eight data quality checks were performed:

| Test ID | Data Quality Check | Result|
|---|---|---|
| DQ-001 | Completeness | PASS |
| DQ-002 | Row ID Uniqueness | PASS |
| DQ-003 | Date Validity | PASS |
| DQ-004 | Shipping Date Sequence | PASS |
| DQ-005 | Sales Validation | PASS |
| DQ-006 | Zero Sales | FLAGGED | 
| DQ-007 | Profit Validation | FLAGGED |
| DQ-008 | Market Consistency | FLAGGED |

## Key Data Quality Findings

- Zero Sales: 1 transaction with $0 sales and -$1.11 profit.
- Negative Profit: 12,544 records with negative profit.
- Market Consistency: 10,378 records with mismatches between Market and Market2.

Flagged results require further investigation and business clarification; they are not automatically classified as data errors.

## Project Deliverables

- Business Requirements Document (BRD)
- Data Quality Test Cases
- Business Analysis Report
- SQL and Python analysis
- Tableau dashboard

## Tableau Dashboard

[View Interactive Tableau Dashboard] (https://public.tableau.com/app/profile/sovana.gurung/viz/GlobalSuperstoreBusinessAnalysis_17928099899260/Dashboard1)

## Repository Structure

global-superstore-business-analysis/
├── README.md
├── documentation/
│   ├── Business_Requirements_Document.pdf
│   ├── Data_Quality_Test_Cases.pdf
│   └── Business_Analysis_Report.pdf
├── analysis/
│   └── Global_Superstore_Analysis.ipynb
├── dashboard/
│   └── tableau_dashboard_link.txt
└── images/
    └── tableau_dashboard.png

## Business Recommendations

- Review discounting practices for products with consistently weak profitability.
- Investigate loss-making products in the Tables sub-category.
- Review geographic market mappings for consistency.
- Validate flagged transactions and clarify business rules before using them in recurring reports.

## Project Limitations

This analysis is based on historical transaction data from 2011–2014. Observed relationships between discounts, shipping costs, and profitability are descriptive 
and do not establish causation. Flagged data quality findings require business clarification.

---

**Project Focus:** Business Analysis | Data Quality Assurance | SQL | Python | Tableau
