    # Final Project Documentation

## SaaS/E-Commerce Cohort Retention & CLTV Analysis

## 1. Project Purpose

The project was developed to transform transaction-level customer data into a structured customer-retention and customer-value intelligence solution.

The analytical solution combines cohort analysis and Customer Lifetime Value (CLTV) modelling to answer both operational and financial questions.

## 2. Business Objectives

The project objectives were to:

1. Measure customer retention across cohorts.
2. Identify lifecycle retention patterns and drop-off.
3. Calculate historical customer lifetime value.
4. Predict customer lifetime value.
5. Segment customers by value.
6. Identify high-value customers.
7. Provide business-facing Power BI reporting.
8. Support Product Manager and Finance Director decisions.
9. Translate analytical findings into practical recommendations.

## 3. Methodology

### 3.1 Data Preparation

Customer transactions were cleaned, validated, and transformed into customer-level analytical features.

### 3.2 Cohort Analysis

Customers were grouped into cohorts based on their purchase lifecycle.

Retention was evaluated by lifecycle month and visualized through a cohort heatmap and lifecycle retention trend.

### 3.3 Historical CLTV

Historical customer value was calculated from observed customer behaviour and transaction history.

### 3.4 Predictive CLTV

A predictive model was developed using customer-level behavioural and value features.

The model generated predicted CLTV for 5,878 customers.

### 3.5 Segmentation

Customers were segmented using historical CLTV quartile thresholds:

- Low Value
- Medium Value
- High Value

### 3.6 Business Intelligence

Power BI was used to combine retention, CLTV, segmentation, and customer-level analysis into an interactive three-page dashboard.

## 4. Validated Results

### Customer Value

- Customers modelled: **5,878**
- Average historical CLTV: **1,893.75**
- Average predicted CLTV: **1,875.72**
- Median historical CLTV: **882.36**
- Median predicted CLTV: **890.68**

### Model Performance

- MAE: **56.16**
- RMSE: **278.64**
- Training R²: **0.9294**
- Testing R²: **0.9904**

### Retention

- Total cohorts: **25**
- Month 1 retention: **100.00%**
- Month 12 retention: **16.64%**

### Segmentation

- Low Value: **1,703 customers / 28.97%**
- Medium Value: **2,705 customers / 46.02%**
- High Value: **1,470 customers / 25.01%**

## 5. Business Interpretation

The analysis shows that customer value is highly concentrated in the High Value segment while the Medium Value segment contains the largest customer population.

The retention analysis also shows substantial lifecycle attrition, with Month 12 retention at 16.64%.

These findings indicate two major management priorities:

1. Protect high-value customers from churn.
2. Improve lifecycle retention and develop suitable Medium Value customers toward higher-value behaviour.

## 6. Decision Framework

| Business Finding | Management Implication | Recommended Action |
|---|---|---|
| Month 12 retention = 16.64% | Significant lifecycle attrition | Identify earliest validated drop-off and activate re-engagement |
| High Value = 25.01% | Customer value is concentrated | Prioritize high-value retention |
| Medium Value = 46.02% | Largest segment has development potential | Increase purchase frequency and order value |
| Predicted CLTV = 1,875.72 | Future customer value can guide prioritization | Use CLTV in customer-management decisions |
| CAC unavailable | Actual acquisition economics cannot be calculated | Integrate marketing-cost data |
| Assumed CAC scenario = 1,000 | Scenario CLTV:CAC = 1.88x | Replace assumption with actual CAC when available |

## 7. Data and Analytical Limitations

The project does not claim actual CAC because acquisition-cost data is absent from the source dataset.

The dashboard's CAC scenario is therefore explicitly hypothetical.

The retention analysis supports identification of lifecycle drop-off, but specific intervention months should be determined from the validated heatmap rather than assumed.

## 8. Final Deliverables

The completed project includes:

- Customer summary
- Customer segment details
- Segment metrics
- CLTV predictions
- Feature importance
- Prediction summary
- Top predicted customers
- Power BI dashboard
- Week 4 project report
- Final README with business implications and recommendations

## 9. Project Completion

The project is considered implementation-complete.

The final Power BI dashboard was reviewed and committed to GitHub.

The remaining close-out activity is documentation finalization, executive reporting, and formal project closure.