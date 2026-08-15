# WEEK 4 PROJECT REPORT

## SaaS/E-Commerce Cohort Retention & CLTV Analysis

**Implementation Phase 4 | Final Implementation Week**

## 1. Project Information

| Item | Details |
|---|---|
| Project | SaaS/E-Commerce Cohort Retention & CLTV Analysis |
| Week | Week 4 — Implementation Phase 4 |
| Project Lead | Temitope Amos Agboola |
| Status | Completed |
| Primary tools | Python, Pandas, Power BI, DAX, Git/GitHub |

## 2. Executive Summary

Week 4 focused on completing the CLTV modelling, predictive analysis, customer segmentation, visualization, and Power BI implementation for the SaaS/E-Commerce Cohort Retention & CLTV Analysis project. The work progressed from the validated customer-level CLTV dataset to predictive modelling, model evaluation, segmentation, cohort-retention reporting, business-persona alignment, and final dashboard delivery.

The completed solution provides an end-to-end analytical workflow covering customer retention, historical customer value, predicted customer lifetime value, customer segmentation, and business decision support.

The final Power BI dashboard was completed, reviewed, and committed to the project GitHub repository.

## 3. Week 4 Objectives

- Complete the CLTV modelling dataset.
- Develop and evaluate the predictive CLTV model.
- Generate customer-level predicted CLTV values.
- Segment customers according to CLTV.
- Produce analytical outputs for business interpretation.
- Develop and validate the final Power BI dashboard.
- Align the dashboard with the identified business personas.
- Commit and push the completed project assets to GitHub.

## 4. Implementation Activities

### 4.1 CLTV Modelling Dataset

The customer-level modelling dataset was completed with **5,878 customers** and **13 modelling variables**. Historical CLTV was validated before predictive modelling.

| Metric | Historical CLTV |
|---|---:|
| Count | 5,878 |
| Mean | 1,893.75 |
| Median | 882.36 |
| Q1 | 0.00 |
| Q3 | 2,602.18 |
| Maximum | 296,684.72 |

### 4.2 Predictive CLTV Modelling

A predictive CLTV model was developed using customer-level behavioural and value features. Predicted CLTV was generated for all **5,878 customers**.

| Metric | Predicted CLTV |
|---|---:|
| Count | 5,878 |
| Mean | 1,875.72 |
| Median | 890.68 |
| Q1 | 0.00 |
| Q3 | 2,606.01 |
| Maximum | 201,754.40 |

The historical and predicted distributions showed close central-value alignment, supporting the model's ability to capture the major customer-value patterns in the dataset.

## 5. Model Performance

| Metric | Result |
|---|---:|
| MAE | 56.16 |
| RMSE | 278.64 |
| Training R² | 0.9294 |
| Testing R² | 0.9904 |

The testing R² of **0.9904** indicates a very strong relationship between predicted and historical CLTV in the evaluation dataset. The MAE of **56.16** indicates a relatively small average absolute prediction error compared with the overall CLTV distribution.

The model was used to generate customer-level predicted CLTV outputs for the final analytical solution.

## 6. Customer Segmentation

Customers were segmented using historical CLTV quartile thresholds.

- **Low Value:** Historical CLTV ≤ Q1
- **Medium Value:** Q1 < Historical CLTV < Q3
- **High Value:** Historical CLTV ≥ Q3

| Segment | Customers | Percentage | Avg Historical CLTV | Avg Predicted CLTV |
|---|---:|---:|---:|---:|
| Low Value | 1,703 | 28.97% | 0.00 | 4.79 |
| Medium Value | 2,705 | 46.02% | 1,084.65 | 1,090.74 |
| High Value | 1,470 | 25.01% | 5,576.51 | 5,487.67 |
| **Total** | **5,878** | **100%** | | |

## 7. Cohort Retention Analysis

The cohort retention analysis was incorporated into the final dashboard to support lifecycle and retention decision-making.

| Retention Metric | Validated Result |
|---|---:|
| Total cohorts | 25 |
| Month 1 retention | 100.00% |
| Month 12 retention | 16.64% |

The analysis includes:

- Cohort retention heatmap
- Customer cohort size analysis
- Average retention by customer lifecycle month

The retention analysis directly supports the Product Manager persona by providing visibility into customer stickiness and lifecycle drop-off.

## 8. Power BI Dashboard Development

The final Power BI dashboard was completed across three analytical pages.

| Page | Focus |
|---|---|
| **Page 1 — Executive CLTV Overview** | Customer base, revenue, historical and predicted CLTV, segmentation, and value comparison. |
| **Page 2 — Cohort Retention Analysis** | Retention KPIs, cohort heatmap, cohort size, and lifecycle retention trends. |
| **Page 3 — Customer Segmentation & CLTV Insights** | High-value customers, segment value, top predicted customers, revenue-per-transaction analysis, and CLTV:CAC scenario. |

## 9. Business Persona Alignment

### 9.1 Product Manager

**Primary need:** Understanding user stickiness and drop-off points.

The dashboard addresses this need through:

- Cohort retention heatmap
- Lifecycle retention analysis
- Month 1 and Month 12 retention KPIs
- Cohort-level customer analysis

These visuals allow the Product Manager to identify retention patterns and lifecycle stages where customer retention declines.

### 9.2 Finance Director

**Primary need:** Revenue forecasting and profitability/customer-value analysis.

The dashboard addresses this need through:

- Historical CLTV
- Predicted CLTV
- Customer segmentation
- High-value customer identification
- Top predicted customers
- CLTV:CAC scenario analysis

The source dataset does not contain customer acquisition cost data. Therefore, actual CAC was not calculated. Instead, the dashboard provides a clearly labelled assumed-CAC scenario.

| Scenario | Result |
|---|---:|
| Assumed CAC | 1,000 |
| Predicted CLTV:CAC | 1.88x |
| Implied CAC at 3:1 target | 625.24 |

> **Note:** The CAC values above are scenario outputs based on predicted CLTV and are not observed acquisition costs from the dataset.

## 10. Key Analytical Findings

- The modelling population contains **5,878 customers**.
- Average historical CLTV is **1,893.75**, while average predicted CLTV is **1,875.72**.
- The predictive model achieved a testing R² of **0.9904**.
- High Value customers represent **25.01%** of customers and have substantially higher average CLTV than Medium and Low Value customers.
- Medium Value customers represent the largest segment at **46.02%**.
- Month 12 retention is **16.64%**, compared with 100.00% in Month 1, highlighting substantial lifecycle attrition.
- The final dashboard combines retention, customer value, segmentation, and decision-support views.

## 11. Challenges and Resolutions

| Challenge | Resolution |
|---|---|
| CLTV modelling dataset and historical values required revalidation | Notebook was updated, kernel restarted, and all cells were rerun successfully. |
| Model evaluation initially referenced undefined training/testing R² variables | Training and testing R² calculations were added and validated. |
| Power BI relationships and aggregations required refinement | Relationships were reviewed and visual aggregations were corrected. |
| Dashboard visual configuration issues occurred | Visuals were simplified or replaced where necessary and validated. |
| CAC was not present in the source dataset | A clearly labelled assumed-CAC scenario was used instead of claiming an actual CAC calculation. |

## 12. Deliverables Completed

- `customer_summary.csv`
- `customer_segment_details.csv`
- `segment_metrics.csv`
- `cltv_predictions.csv`
- `feature_importance.csv`
- `prediction_summary.csv`
- `top_predicted_customers.csv`
- `SaaS_ECommerce_Cohort_Retention_CLTV_Dashboard.pbix`

## 13. Quality Assurance and Validation

- Validated customer count and historical CLTV statistics.
- Validated predicted CLTV statistics.
- Validated model performance metrics.
- Validated customer segmentation thresholds and distribution.
- Validated cohort retention KPIs, including the final Month 12 value of **16.64%**.
- Reviewed Power BI relationships, aggregation choices, KPI values, and page-level visuals.
- Restarted the modelling notebook kernel and executed all cells successfully without errors.
- Completed final dashboard review before version-control submission.

## 14. GitHub and Version Control

The completed Power BI dashboard was committed and pushed to the project repository.

GitHub is mandatory for Data Analytics projects under the Infotact project guidelines. The guidelines also specify that valid commits include meaningful code changes, documentation updates, README updates, configuration changes, assets, and merge commits.

The Infotact final review evaluates implementation completion, GitHub commit discipline, code quality/documentation, and team collaboration. Week 4 represents Implementation Phase 4.

## 15. Week 4 Outcomes

- Completed customer-level CLTV modelling for **5,878 customers**.
- Generated and validated predicted CLTV for all customers.
- Achieved **0.9904 testing R²** with MAE of **56.16** and RMSE of **278.64**.
- Completed Low, Medium, and High Value customer segmentation.
- Completed cohort retention analysis with **25 cohorts** and validated Month 12 retention of **16.64%**.
- Completed the three-page Power BI dashboard.
- Addressed Product Manager and Finance Director analytical needs.
- Implemented a transparent CLTV:CAC scenario without introducing unsupported actual CAC data.
- Committed and pushed the final dashboard to GitHub.

## 16. Overall Project Status

The Week 4 implementation successfully transitioned the project from analytical modelling into a completed business intelligence solution:

**Validated data → Cohort analysis → CLTV modelling → Predictive modelling → Customer segmentation → Business insights → Power BI dashboard → Version-controlled final deliverable**

The project is ready for final project documentation, the Executive Report, and project close-out.

## 17. Conclusion

Week 4 completed the implementation of the SaaS/E-Commerce Cohort Retention & CLTV Analysis solution.

The final outputs combine customer retention analysis with historical and predictive customer value, enabling segmentation and business-oriented decision support. The completed Power BI dashboard provides an integrated view for operational and financial stakeholders, while the documented assumptions and validation steps preserve analytical transparency.