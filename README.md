# SaaS/E-Commerce Cohort Retention & Customer Lifetime Value (CLTV) Analysis

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?logo=pandas)
![NumPy](https://img.shields.io/badge/NumPy-Scientific%20Computing-013243?logo=numpy)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?logo=powerbi)
![Git](https://img.shields.io/badge/Git-Version%20Control-F05032?logo=git)
![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?logo=github)

---

## Project Overview

Customer retention is a critical driver of sustainable business growth. This project applies **cohort retention analysis, historical Customer Lifetime Value (CLTV), predictive CLTV modelling, and customer segmentation** to transactional e-commerce data.

The solution moves from transaction-level data preparation to customer-value modelling, retention analysis, Power BI reporting, and actionable business recommendations.

## Business Problem

Without visibility into retention and customer lifetime value, businesses can struggle to:

- Identify where customers drop off during the lifecycle
- Prioritize retention interventions
- Protect high-value customers
- Develop medium-value customers
- Allocate customer-management resources efficiently
- Evaluate acquisition spending against expected customer value

## Project Objectives

- Perform customer cohort analysis.
- Calculate monthly cohort retention rates.
- Identify customer lifecycle retention patterns.
- Calculate historical CLTV.
- Develop and evaluate a predictive CLTV model.
- Segment customers by value.
- Identify high-value and top predicted-value customers.
- Develop a Power BI executive dashboard.
- Translate findings into business recommendations.
- Demonstrate CLTV:CAC scenario planning.

## Business Questions

1. How does customer retention change across the customer lifecycle?
2. How many cohorts are represented?
3. What is retention by lifecycle month?
4. What is the historical customer value?
5. What is the predicted future CLTV?
6. Which customer segments contribute the greatest value?
7. Which customers have the highest predicted CLTV?
8. How should retention strategies differ by customer value?
9. How can CLTV support acquisition-cost decisions?

## Dataset and Analytical Scope

The project uses the **Online Retail II** transaction dataset.

The final customer-level modelling population contains:

- **5,878 customers**
- **13 modelling variables**

## Analytical Workflow

```text
Business Understanding
        ↓
Data Acquisition
        ↓
Data Cleaning & Validation
        ↓
Customer-Level Feature Engineering
        ↓
Historical CLTV Calculation
        ↓
Cohort Retention Analysis
        ↓
Predictive CLTV Modelling
        ↓
Model Evaluation
        ↓
Customer Segmentation
        ↓
Power BI Dashboard
        ↓
Business Recommendations
        ↓
Final Documentation & GitHub Submission
```

## Technology Stack

- Python 3.11
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook
- Power BI
- Git
- GitHub

# Key Results

## Customer Value

| Metric | Result |
|---|---:|
| Customers modelled | 5,878 |
| Average Historical CLTV | 1,893.75 |
| Average Predicted CLTV | 1,875.72 |
| Median Historical CLTV | 882.36 |
| Median Predicted CLTV | 890.68 |
| Maximum Historical CLTV | 296,684.72 |
| Maximum Predicted CLTV | 201,754.40 |

## Predictive Model Performance

| Metric | Result |
|---|---:|
| MAE | 56.16 |
| RMSE | 278.64 |
| Training R² | 0.9294 |
| Testing R² | 0.9904 |

The testing R² of **0.9904** indicates a very strong relationship between predicted and historical CLTV in the evaluation dataset. Model performance should still be monitored on future customer data before operational deployment.

## Customer Segmentation

| Segment | Customers | Percentage | Avg Historical CLTV | Avg Predicted CLTV |
|---|---:|---:|---:|---:|
| Low Value | 1,703 | 28.97% | 0.00 | 4.79 |
| Medium Value | 2,705 | 46.02% | 1,084.65 | 1,090.74 |
| High Value | 1,470 | 25.01% | 5,576.51 | 5,487.67 |

The **Medium Value segment is the largest at 46.02%**, while the **High Value segment represents 25.01% of customers but has substantially higher average CLTV**.

## Cohort Retention

| Retention KPI | Result |
|---|---:|
| Total cohorts | 25 |
| Month 1 Retention | 100.00% |
| Month 12 Retention | 16.64% |

The reduction from **100.00% Month 1 retention to 16.64% Month 12 retention** demonstrates substantial customer attrition across the observed lifecycle.

# Business Implications and Recommendations

## 1. Improve Lifecycle Retention

**Finding:** Month 12 retention is **16.64%**, compared with 100.00% in Month 1.

**Business implication:** A substantial proportion of customers do not remain active through the longer lifecycle.

**Recommendation:** Use the cohort heatmap to identify the earliest validated material drop-off point and introduce targeted lifecycle interventions such as automated re-engagement emails, inactivity reminders, personalized recommendations, targeted offers, and post-purchase engagement.

If the validated heatmap identifies Month 2 as the first material drop-off point, an automated re-engagement sequence should be introduced around Month 2.

## 2. Protect High-Value Customers

High Value customers represent **25.01%** of the customer base and have average historical CLTV of **5,576.51**.

**Recommendation:** Develop a High Value retention program using personalized engagement, priority service, cross-sell/upsell opportunities, churn-risk monitoring, and targeted loyalty initiatives.

## 3. Develop the Medium-Value Segment

Medium Value customers represent the largest segment at **46.02%**.

**Recommendation:** Develop programs that increase purchase frequency, average order value, product breadth, and repeat-purchase consistency, with the goal of moving suitable Medium Value customers toward High Value status.

## 4. Apply Different Retention Economics

Low Value customers represent **28.97%** of customers.

**Recommendation:** Use lower-cost automated engagement for low-value customers while reserving high-touch interventions for High Value customers and Medium Value customers with strong growth potential.

## 5. Prioritize Customers Using Predicted CLTV

The project produces customer-level predicted CLTV and a Top Predicted Customers view.

Predicted CLTV can support:

- Retention prioritization
- Account management
- Personalized offers
- Cross-sell and upsell planning
- Customer service prioritization

## 6. Use CLTV for CAC Scenario Planning

Actual CAC is **not available in the source dataset**, so the dashboard uses an assumed scenario.

| Metric | Value |
|---|---:|
| Average Predicted CLTV | 1,875.72 |
| Assumed CAC | 1,000 |
| Predicted CLTV:CAC | 1.88x |
| Implied CAC at 3:1 CLTV:CAC | 625.24 |

**Recommendation:** Replace assumed CAC with actual acquisition-cost data when available and use observed CLTV:CAC to establish acquisition-spend thresholds.

> The CAC figures above are scenario values, not observed CAC values from the source dataset.

# Dashboard

## Page 1 — Executive CLTV Overview

- Customer base
- Revenue
- Historical CLTV
- Predicted CLTV
- Customer segmentation
- Historical versus predicted value

## Page 2 — Cohort Retention Analysis

- Total cohorts
- Month 1 retention
- Month 12 retention
- Cohort retention heatmap
- Cohort size
- Lifecycle retention trends

## Page 3 — Customer Segmentation & Predictive CLTV

- High Value customer analysis
- Segment size and value
- Predicted CLTV
- Top predicted customers
- Revenue per transaction by segment
- CLTV:CAC scenario analysis

# Business Personas

## Product Manager

**Primary need:** Understand user stickiness and drop-off points.

**Dashboard interaction:** Uses the cohort heatmap to identify where retention materially declines after acquisition.

**Recommended action:** Trigger product and lifecycle interventions at the earliest validated retention drop-off point.

## Finance Director

**Primary need:** Revenue forecasting and profitability/customer-value analysis.

**Dashboard interaction:** Uses historical CLTV, predicted CLTV, customer segmentation, High Value analysis, and CLTV:CAC scenario analysis.

**Recommended action:** Combine predicted CLTV with actual CAC data to establish defensible acquisition-spend thresholds.

# Final Deliverables

- Customer-level analytical outputs
- CLTV predictions
- Customer segmentation outputs
- Feature importance outputs
- Cohort retention analysis
- Power BI dashboard
- Final dashboard screenshots
- Week 4 project progress report
- Final project documentation
- Executive report

# Repository Structure

```text
SaaS-ECommerce-Cohort-Retention-CLTV-Analysis/
│
├── data/
│   ├── raw/
│   └── processed/
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   ├── 02_cohort_analysis.ipynb
│   ├── 03_cltv_analysis.ipynb
│   └── 04_visualizations.ipynb
├── reports/
│   ├── Project_Progress_Report_Week_4.md
│   ├── FINAL_PROJECT_DOCUMENTATION.md
│   └── EXECUTIVE_REPORT.md
├── images/
│   ├── Cohort Retention Dashboard.png
│   ├── Executive Overview Dashboard.png
│   └── Predictive CLTV Dashboard.png
├── src/
├── visuals/
│   └── SaaS_ECommerce_Cohort_Retention_CLTV_Dashboard.pbix
├── README.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── LICENSE
├── requirements.txt
└── .gitignore
```

# Quality Assurance

The completed project included validation of:

- Customer counts
- Historical CLTV
- Predicted CLTV
- Model performance
- Customer segmentation
- Cohort retention KPIs
- Power BI table relationships
- Visual aggregations
- KPI values
- Dashboard page consistency

The final visualization notebook was executed successfully after the final updates.

# Limitations

1. Actual CAC is not available in the source dataset.
2. CAC analysis is therefore scenario-based.
3. Retention recommendations should be based on validated cohort patterns rather than unsupported assumptions.
4. Predicted CLTV should support, not replace, commercial judgement.
5. Predictive model performance should be monitored on new customer cohorts before production deployment.
6. Historical customer behaviour may not fully represent future purchasing behaviour.

# Recommended Next Steps

## Short Term

1. Integrate actual marketing and acquisition-cost data.
2. Monitor cohort retention regularly.
3. Establish lifecycle re-engagement triggers.
4. Prioritize High Value customers for retention.
5. Develop Medium Value customer conversion campaigns.

## Medium Term

1. Build a recurring CLTV monitoring pipeline.
2. Add churn-risk modelling.
3. Integrate actual CAC and calculate observed CLTV:CAC.
4. Monitor predictive model drift using new customer cohorts.
5. Connect customer-value outputs to CRM and customer-engagement workflows.

# Four-Week Project Roadmap

### Week 1
- Data acquisition
- Data cleaning
- Data preparation
- Feature engineering

### Week 2
- Cohort identification
- Cohort retention matrix
- Retention rate calculation

### Week 3
- Average Order Value
- Purchase Frequency
- Historical CLTV
- Customer segmentation
- Predictive CLTV modelling

### Week 4
- Retention heatmap
- Retention trend analysis
- Predictive CLTV insights
- Power BI dashboard
- Executive insights
- Final documentation
- GitHub submission

# Project Status

**Status: COMPLETED**

The project progressed from business understanding and transaction-level data preparation through cohort analysis, historical and predictive CLTV modelling, customer segmentation, Power BI dashboard development, business insight generation, final documentation, and GitHub submission.

The final solution provides a business-facing framework for understanding customer retention and customer value and translating those insights into targeted customer-management and acquisition decisions.

# Author

**Temitope Amos Agboola**

Data Analyst | Business Analytics | Business Intelligence

# License

This project is licensed under the MIT License.
