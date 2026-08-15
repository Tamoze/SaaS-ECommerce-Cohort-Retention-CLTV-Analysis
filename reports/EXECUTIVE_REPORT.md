    # Executive Report

## SaaS/E-Commerce Cohort Retention & CLTV Analysis

## Executive Summary

This project converts customer transaction data into actionable intelligence on retention and customer lifetime value.

The final analysis covers **5,878 customers**, **25 cohorts**, historical CLTV, predicted CLTV, customer segmentation, and lifecycle retention.

The final Power BI dashboard provides three views:

1. Executive CLTV Overview
2. Cohort Retention Analysis
3. Customer Segmentation & CLTV Insights

The analysis demonstrates that customer value is concentrated in a smaller High Value segment while the Medium Value segment contains the largest customer population. At the same time, customer retention declines materially over the lifecycle, with Month 12 retention at **16.64%** compared with **100.00%** in Month 1.

## 1. Key Executive Metrics

| KPI | Result |
|---|---:|
| Customers analysed | 5,878 |
| Average Historical CLTV | 1,893.75 |
| Average Predicted CLTV | 1,875.72 |
| Testing R² | 0.9904 |
| MAE | 56.16 |
| RMSE | 278.64 |
| Total cohorts | 25 |
| Month 1 retention | 100.00% |
| Month 12 retention | 16.64% |
| High Value customers | 1,470 |
| High Value customer share | 25.01% |
| Medium Value customer share | 46.02% |

## 2. What the Analysis Means

### Customer Retention

The most important retention finding is the substantial reduction in retained customers over the customer lifecycle.

Month 12 retention is only 16.64%.

**Business implication:** Retention should not be treated as a single KPI. It should be managed as a lifecycle process.

**Recommended action:** Use the cohort heatmap to identify the earliest validated material drop-off and deploy an automated re-engagement sequence at that point.

Potential interventions include:

- Re-engagement email
- Personalized product recommendations
- Inactivity reminders
- Targeted offers
- Customer journey interventions

The exact intervention month should be determined from the validated heatmap rather than assumed.

### Customer Value

Average predicted CLTV is **1,875.72**, compared with historical CLTV of **1,893.75**.

The predicted value distribution is therefore broadly aligned with historical customer value.

**Business implication:** Customer value can be used to prioritize customer-management activities rather than treating the entire customer base uniformly.

### High Value Customers

High Value customers represent **25.01%** of customers and have:

- Average historical CLTV: **5,576.51**
- Average predicted CLTV: **5,487.67**

**Business implication:** This group warrants disproportionate retention attention because its average customer value is substantially higher.

**Recommended action:** Establish a high-value retention program with proactive engagement, personalized offers, cross-sell/upsell opportunities, and churn monitoring.

### Medium Value Customers

Medium Value customers represent **46.02%**, making them the largest segment.

Average predicted CLTV is **1,090.74**.

**Business implication:** This is the largest opportunity pool for customer-value development.

**Recommended action:** Focus on increasing purchase frequency, average order value, and product breadth among customers with demonstrated potential to move toward High Value status.

## 3. Finance and Acquisition Economics

Actual CAC cannot be calculated from the source dataset because acquisition-cost data is not available.

The dashboard therefore uses a scenario:

| Scenario | Value |
|---|---:|
| Assumed CAC | 1,000 |
| Predicted CLTV:CAC | 1.88x |
| Implied CAC at 3:1 target | 625.24 |

**Executive recommendation:** Integrate actual acquisition-spend data before using CLTV:CAC as an operational acquisition rule.

Once actual CAC is available, management can compare predicted CLTV against acquisition cost and establish customer-acquisition spending limits by segment.

## 4. Strategic Recommendations

### Priority 1 — Improve Lifecycle Retention

Use cohort analysis to identify the earliest material retention drop-off.

**Action:** Deploy automated re-engagement journeys at the validated lifecycle stage.

### Priority 2 — Protect High Value Customers

Use predicted CLTV and historical value to identify customers that warrant proactive retention.

**Action:** Establish high-value customer monitoring and personalized engagement.

### Priority 3 — Develop Medium Value Customers

The Medium Value segment is the largest customer group.

**Action:** Use targeted offers, cross-selling, and purchase-frequency interventions to increase customer value.

### Priority 4 — Control Retention Economics

Not all customers should receive the same level of retention investment.

**Action:** Use predicted CLTV to prioritize higher-value customers while maintaining low-cost automated engagement for low-value customers.

### Priority 5 — Integrate CAC Data

The current CAC analysis is scenario-based.

**Action:** Integrate actual marketing and acquisition costs into the analytical model so that observed CLTV:CAC can be calculated and monitored.

## 5. Management Decision Framework

| Decision Area | Current Evidence | Recommended Management Response |
|---|---|---|
| Retention | Month 12 retention = 16.64% | Identify earliest material lifecycle drop-off and intervene |
| High-value customers | 25.01% of customers; avg historical CLTV 5,576.51 | Prioritize retention and personalized engagement |
| Medium-value customers | 46.02% of customers | Develop customers with value-growth potential |
| Predicted customer value | Avg predicted CLTV 1,875.72 | Use for prioritization and planning |
| Acquisition economics | CAC unavailable | Integrate actual acquisition-cost data |
| Scenario economics | 1.88x at assumed CAC of 1,000 | Replace assumption with observed CAC before operational use |

## 6. Final Assessment

The project successfully delivers an integrated customer-retention and CLTV analytics solution.

The strongest business opportunity is not simply identifying which customers are valuable; it is using the combination of **retention timing + predicted customer value + segmentation** to determine where management attention should be allocated.

The dashboard therefore provides a foundation for:

- Retention strategy
- Customer prioritization
- Lifecycle engagement
- Customer-value development
- Acquisition-cost planning
- Executive performance monitoring

## 7. Final Recommendation

Management should operationalize the analysis in three stages:

1. **Retention:** identify and intervene at the earliest validated lifecycle drop-off.
2. **Value:** prioritize High Value customers and develop suitable Medium Value customers.
3. **Economics:** integrate actual CAC data and establish segment-level CLTV:CAC thresholds.

The current analysis is suitable as a decision-support foundation, with actual acquisition-cost integration and ongoing model monitoring recommended before full operational deployment.