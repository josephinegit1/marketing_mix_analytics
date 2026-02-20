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

1️⃣ Objective

Understand the impact of marketing channels (TV, Digital, Social, Print, Promo, In-Store Display) on sales.

Quantify the ROI of marketing investments.

Recommend optimal budget allocation to maximize revenue.

Provide an interactive executive dashboard for decision-making.

2️⃣ Methodology

Data Collection & Cleaning

Weekly regional marketing and sales data collected.

Cleaned and transformed using Python (Pandas, NumPy) and SQL.

Exploratory Analysis

Checked correlations, trends, and seasonality.

Detected multicollinearity across individual channels.

Modeling

Aggregated correlated channels into Total Marketing Spend.

Built linear regression (Marketing Mix Model) to quantify marginal impact of each driver on sales.

Validated model using R² (0.996) and residual analysis.

Simulation & Optimization

Ran scenario simulations to identify optimal allocation for marketing spend, promo, and in-store display.

Visualization

Developed an interactive Power BI dashboard with key KPIs.

3️⃣ Model Results
Feature	Coefficient / Impact	Interpretation
Total Marketing Spend	2.13	Every $1 invested generates $2.13 in sales
Promo Discount %	982	Each 1% promo increases sales by $982
In-Store Display	4121	Display activation adds ~$4.1K per week
Holiday Flag	2746	Holiday weeks increase sales by ~$2.7K
Competitor Spend	-2.54	Each $1 competitor spend reduces sales by $2.54

R²: 0.996 (very high explanatory power)

5️⃣ Business Impact

Quantified marketing ROI and channel contributions.

Identified high-impact investments: marketing spend, in-store displays.

Recommended tactical promo usage instead of aggressive discounting.

Provided executives with an interactive dashboard for real-time, data-driven budget decisions.

Scenario simulations helped allocate budget optimally to maximize expected sales.

## Data Assumptions & Expectations
- Date represents the reporting period for both sales and marketing spend.
- Sales values are expected to be non-negative.
- Marketing spend values may be zero during periods without active campaigns.
- Data is assumed to be aggregated at a daily or weekly level.

