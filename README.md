# Marketing Mix Performance Analytics

## Business Problem
The organization invests marketing budgets across multiple channels, including TV, digital, search, and social media. With limited budgets and increasing pressure to improve return on investment, leadership needs data-driven insights to understand how effectively each channel contributes to revenue and overall business performance.

## Key Business Questions
1. Which marketing channels drive the highest revenue?
2. Which channels deliver the best return on investment (ROI)?
3. Is marketing spend saturated across any channels?

## Success Criteria
- Clear visibility into channel-level revenue and ROI performance  
- Evidence-based insights into spend efficiency and saturation  
- Interactive dashboards to support executive decision-making  
- Actionable recommendations for marketing budget optimization

## Dataset Overview
The dataset contains historical marketing spend and sales data across multiple channels over time.

## Data Dictionary

| Column Name | Description |
|------------|-------------|
| date | Date of the observation |
| tv_spend | Marketing spend on TV advertising |
| digital_spend | Marketing spend on digital channels |
| search_spend | Marketing spend on search advertising |
| social_spend | Marketing spend on social media advertising |
| sales | Total revenue generated |

## Mapping Business Questions to Data

| Business Question | Relevant Columns |
|------------------|------------------|
| Which channel drives the most revenue? | tv_spend, digital_spend, search_spend, social_spend, sales |
| Which channel has the best ROI? | Channel spend columns, sales |
| Is marketing spend saturated? | Channel spend columns, sales, date |

## Data Assumptions & Expectations
- Date represents the reporting period for both sales and marketing spend.
- Sales values are expected to be non-negative.
- Marketing spend values may be zero during periods without active campaigns.
- Data is assumed to be aggregated at a daily or weekly level.

