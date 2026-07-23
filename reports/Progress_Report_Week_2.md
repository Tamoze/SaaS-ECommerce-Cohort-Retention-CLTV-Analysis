# Week 2 Project Progress Report

## Summary

Successfully completed the Customer Cohort Retention Analysis phase of the SaaS & E-Commerce Cohort Retention and Customer Lifetime Value (CLTV) Analysis project. This stage focused on transforming the cleaned transaction dataset into meaningful customer cohorts, measuring customer retention over time, and generating analytical outputs that will serve as the foundation for Customer Lifetime Value modelling in Week 3.

---

## Activities Completed

### 1. Cohort Feature Engineering

Customer acquisition cohorts were created by identifying each customer's first purchase month. Additional cohort attributes were engineered, including:

- Invoice Month
- Cohort Month
- Cohort Index (Months Since First Purchase)

These features established the temporal structure required for customer retention analysis.

---

### 2. Customer Cohort Analysis

Customers were grouped into monthly acquisition cohorts, and unique customer counts were calculated for every cohort-month combination.

A customer cohort matrix was generated to monitor customer activity across successive months following acquisition.

---

### 3. Customer Retention Analysis

Monthly retention rates were calculated by dividing the number of returning customers by the size of each acquisition cohort.

A retention matrix containing 25 customer cohorts across 25 monthly periods was successfully produced.

---

### 4. Customer Retention Visualizations

Several executive-level visualizations were developed, including:

- Customer Cohort Retention Heatmap
- Average Monthly Customer Retention Trend
- Customer Acquisition by Cohort

These visualizations provide a clear understanding of customer retention behaviour throughout the observation period.

---

### 5. Cohort Performance Evaluation

The strongest and weakest customer cohorts were identified using Month 2 retention as an indicator of early customer loyalty.

Key findings include:

- Highest Month 2 Retention:
  - 2009-12 (37.5%)
  - 2011-09 (34.2%)
  - 2011-10 (33.5%)

- Lowest Month 2 Retention:
  - 2010-12 (11.7%)
  - 2011-11 (17.2%)
  - 2010-05 (19.3%)

These results provide valuable insights into customer engagement across acquisition periods.

---

### 6. Exported Analysis Outputs

The following analytical datasets were generated for downstream analysis:

- cohort_counts.csv
- retention_matrix.csv
- cohort_sizes.csv

These datasets will be reused during Customer Lifetime Value modelling and Power BI dashboard development.

---

## Key Business Insights

- Customer retention declined sharply after the first purchase, with Month 2 retention averaging approximately 25%.
- Retention stabilized between 16% and 23% during later months, indicating the presence of a loyal core customer segment.
- Several acquisition cohorts consistently outperformed others, suggesting potential differences in acquisition quality or seasonal purchasing behaviour.
- Early customer retention represents the greatest opportunity for improving Customer Lifetime Value.

---

## Deliverables Completed

- Customer Cohort Feature Engineering
- Customer Cohort Matrix
- Customer Retention Matrix
- Customer Retention Heatmap
- Average Retention Trend Analysis
- Customer Acquisition by Cohort Analysis
- Best and Worst Performing Cohort Analysis
- Exported Analysis Tables

---

## Next Phase

Week 3 will focus on Customer Lifetime Value (CLTV) Analysis, including customer revenue aggregation, purchase frequency analysis, customer lifespan estimation, CLTV calculation, customer segmentation, and executive-level CLTV visualizations.