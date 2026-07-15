# Data Dictionary

# SaaS/E-Commerce Cohort Retention & Customer Lifetime Value (CLTV) Analysis

---

## Dataset Information

| Item | Details |
|------|---------|
| Dataset | Online Retail II |
| Source | UCI Machine Learning Repository |
| Records | 1,067,371 |
| Columns | 8 |
| Time Period | December 2009 – December 2011 |
| Business Domain | E-Commerce |

---

# Data Dictionary

| Column | Data Type | Description | Business Use |
|---------|-----------|-------------|--------------|
| Invoice | String | Unique transaction identifier. Values beginning with **C** indicate cancelled transactions. | Identify completed and cancelled orders. |
| StockCode | String | Unique product identifier. | Product-level analysis. |
| Description | String | Product description. | Product categorization and reporting. |
| Quantity | Integer | Number of units purchased. Negative values indicate returned or cancelled items. | Sales volume and order analysis. |
| InvoiceDate | DateTime | Date and time of transaction. | Cohort assignment, retention analysis, time-series analysis. |
| Price | Float | Unit selling price (£). | Revenue calculations and CLTV estimation. |
| Customer ID | Integer | Unique customer identifier. | Customer tracking, cohort creation, CLTV calculation. |
| Country | String | Customer's country of residence. | Geographic segmentation. |

---

# Derived Fields

The following variables will be created during preprocessing:

| Field | Description |
|--------|-------------|
| TotalSales | Quantity × Price |
| InvoiceMonth | Transaction month (YYYY-MM) |
| CohortMonth | Customer's first purchase month |
| CohortIndex | Number of months since first purchase |
| OrderMonth | Month of transaction |
| Year | Transaction year |
| Month | Transaction month |
| Quarter | Transaction quarter |

---

# Data Quality Considerations

Potential issues expected in this dataset include:

- Cancelled invoices
- Negative quantities
- Negative prices
- Missing customer IDs
- Duplicate records
- Inconsistent product descriptions

These issues will be addressed during the data cleaning phase before conducting cohort and CLTV analysis.