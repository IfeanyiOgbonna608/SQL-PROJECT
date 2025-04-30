# Intermediate SQL - Sales Analysis

## Overview
Analysis customer behavior, retention trends, and lifetime value to enhance retention strategies and optimize revenue for an e-commerce business.

## Business Questions
1. **Customer Segmentation Analysis:** Who are our most valuable customers?
2. **Cohort Analysis:** How do different customer groups generate revenue?
3. **Customer Retention:** Which customers haven't purchased recently?

## Analysis Approach

### 1. Customer Segmentation Analysis
- Categorized customers based on total lifetime value (LTV)
- Assigned customers to High, Mid, and Low-value segments
- Calculated key metrics: total revenue

🖥 Query: [1_customer_segmentation.sql](/1_customer_segmentation.sql) 

**📈 Visualisation:** 

![alt text](../images/1_customer_segmentation.png)

📊 **Key Findings:**
- High-value segment (25% of customers) drives 66% of revenue($135.4M)
- Mid-value segment (50% of customers) generates 32% of revenue ($66.6M)
- Low-value segment (25% of customers) accounts for 2% of revenue ($4.3M)

💡 **Business Insights** 
-  Prioritize High-Value Customers (Retention & Expansion)
Personalization & Loyalty Programs: These customers drive 66% of revenue, so investing in retention is crucial. Offer VIP programs, exclusive discounts, and premium services tailored to their preferences.

Upselling & Cross-Selling: Since they already spend significantly, find ways to increase their lifetime value further through complementary product recommendations, personalized services, or tiered offerings.

-  Optimize Mid-Value Customers (Growth & Conversion)
Customer Segmentation & Targeted Engagement: The mid-value segment is sizable (50% of total customers) but generates less revenue. Identify behavioral triggers that could push them toward high-value status, such as offering incentives for increased spending.

Educational & Value-Based Marketing: Strengthen their connection to the brand by providing relevant content, training, or insights into maximizing the value of their purchases.

-  Reevaluate Low-Value Customers (Efficiency & Cost Reduction)
Resource Allocation: The low-value segment constitutes 25% of customers but contributes only 2% of revenue. Evaluate whether supporting this segment is cost-effective.

Alternative Monetization Strategies: Consider bundling products, offering freemium models, or shifting marketing efforts toward retention rather than acquisition of these customers.

Potential for Upscaling: If possible, assess whether a portion of these customers could be moved into mid-tier spending through discounts or limited-time offers.

-  Data-Driven Decision Making
Predictive Analytics: Use AI and historical trends to forecast customer behavior and optimize strategies accordingly.

Customer Lifetime Value Modeling: Enhance profitability by focusing on segments with the highest potential for long-term engagement.

- Strategic Resource Allocation
Given the revenue distribution, allocate marketing budget proportionally: Prioritize high-value customers, invest in converting mid-value customers, and optimize resources for the low-value segment.

Focus efforts on long-term retention rather than acquisition—ensuring sustainable revenue growth from high-value customers.

## Strategic Recommendations 

1. High-Value Customers (66% of revenue) – Strengthen loyalty with VIP programs, personalized offers, and upselling opportunities to boost lifetime value.

2. Mid-Value Customers (32% of revenue) – Use behavioral insights to encourage higher spending, offer targeted incentives, and improve engagement through educational marketing.

3. Low-Value Customers (2% of revenue) – Optimize resource allocation, explore alternative monetization strategies, and assess opportunities to shift some customers into mid-tier spending.

4. Data-Driven Growth – Leverage predictive analytics and lifetime value modeling to refine acquisition, retention, and pricing strategies.

5. Strategic Budget Allocation – Prioritize high-value customers, invest in converting mid-tier customers, and optimize low-tier support to ensure sustainable revenue growth.

### 2. Cohort Analysis
- Tracked revenue and customer count per cohorts
- Cohorts were grouped by year of first purchase
- Analyzed customer retention at a cohort level

🖥 Query: [2_cohort_analysis.sql](/2_cohort_analysis.sql)


**📈 Visualisation:** 

![alt text](<../images/Cohort Analysis 1.png>)

📊 **Key Findings:**
- Declining Revenue Per Customer Over Time
- Consistently Weaker Performance from the 2022-2024 Cohorts
- Net Revenue Growth Driven by Customer Volume, Not Customer Value

These findings indicate that while the business is scaling, customer spending behavior is shifting unfavorably. Addressing these trends will require evaluating pricing models, customer retention strategies, and overall business positioning.

💡 **Business Insights** 
1. Declining Customer Revenue Per Cohort Year Signals Profitability Risks
The customer revenue metric shows a downward trend over time, indicating that each customer is contributing less revenue compared to earlier cohorts.

Possible Causes:

Changing customer behavior—new customers may be purchasing lower-value products or services.

Pricing strategy issues—discounts or lower pricing could be reducing revenue per customer.

Increased competition—customers may be splitting spending among more competitors.

Decline in customer engagement—new cohorts may not be fully utilizing the offerings.

Business Action: It may be necessary to improve retention strategies, increase customer engagement, or adjust pricing models to maintain profitability.

2. Poor Performance of 2022-2024 Cohorts Indicates Acquisition & Retention Challenges
Customers acquired in 2022, 2023, and 2024 are generating lower revenue per customer compared to earlier cohorts.

Possible Causes:

Marketing strategies may be attracting lower-value customers.

Changes in customer expectations—products/services may not be appealing as they were before.

Declining brand loyalty—new customers may be less committed or engaged.

Business Action: A review of customer acquisition strategies is needed. Focus on attracting high-value customers and improving retention efforts.

3. Net Revenue Growth Driven by Customer Volume Rather Than Value
While total revenue is increasing, this appears to be a result of adding more customers rather than improving per-customer spending.

This means the business is relying on expansion rather than depth of value per customer.

Possible Risks:

Acquisition costs may become unsustainable if customers contribute less revenue over time.

Business may need to work harder to maintain profitability despite revenue growth.

Business Action:

Improve customer lifetime value (LTV) by increasing engagement, upselling, or enhancing loyalty programs.

Consider targeting high-value customer segments rather than focusing solely on expanding the customer base.

Optimize pricing strategies to encourage higher spending per customer.

4. Warning Signs for Future Revenue Trends
If the declining customer revenue trend continues, future revenue growth may stall unless customer spending improves.

Business should track customer engagement closely and work on strategies to maintain long-term value.

## Strategic Recommendation

1. Customer Retention & Engagement – Develop personalized loyalty programs, improve onboarding processes, and use automated re-engagement tactics to sustain long-term customer relationships.

2. Pricing & Product Strategy – Optimize pricing models, conduct segmentation analysis to adjust offerings based on customer spending behavior, and introduce premium products to encourage higher-value purchases.

3. Customer Acquisition Quality – Refine marketing strategies to attract high-value customers, enhance brand messaging, and build partnerships or referral programs to improve customer lifetime value.

4. Increasing Customer LTV – Implement subscription models, upsell and cross-sell strategies, and create unique customer experiences to deepen engagement and drive sustained revenue growth.

5. Addressing Underperformance in 2022–2024 Cohorts – Analyze cohort weaknesses through surveys and churn analysis, improve onboarding for newer customers, and introduce incentives to encourage long-term engagement.

### 3. Customer Retention 
🖥 Query: [3_retention_analysis.sql](/3_retention_analysis.sql)

**📈 Visualisation:** 

![alt text](../images/Customer_Churn_by_Cohort_Year.png)

📊 **Key Findings:**
- Cohort Churn stabilizes at ≈90% after 2-3 years, indicating a predictable long-term retention pattern.
- Retention rates are consistently low(8-10%) across all cohorts, suggesting retention issues are systemic rather than specific to certain years. 
- New cohorts (2022-2023) show similar churn trajectories, signaling that without intervention, future cohorts will follow the same pattern.

💡 **Business Insights**

1. Strong Customer Retention Across All Cohorts

- Each cohort exhibits a high percentage of active customers, indicating strong customer loyalty and satisfaction.

- The retention rate appears relatively consistent across different years, suggesting that the business has effective retention strategies in place.

2. Predictable Churn Patterns

- A small but steady percentage of churned customers across all cohort years suggests that churn is not spiking unpredictably.

- The company can forecast future churn trends and plan retention initiatives based on historical churn rates.

3. Cohort-Based Strategy Opportunities

- Since customer retention is tracked by cohort year, analyzing specific cohorts could reveal differences in behavior.

- Older cohorts (2016–2018) show sustained retention, while more recent cohorts (2020–2022) may need additional engagement strategies to improve long-term retention.

4. Potential for Customer Engagement Improvements

- While retention is high, a small portion of customers churn each year, suggesting room for targeted retention efforts.

- The business could gather feedback from churned customers to identify pain points, optimize services, and strengthen loyalty programs.

5. Customer Loyalty & Stability

- The stable retention rate across different years suggests a strong customer base. The company can leverage this brand loyalty by introducing upsell opportunities, referral programs, and exclusive customer rewards.

6. Minimized External Impact

- Since the churn rate remains relatively stable, it indicates that economic shifts or competitor movements haven’t drastically affected customer retention.

- However, monitoring external factors such as market trends or industry disruptions could help proactively address future risks.


## Strategic Recommendations

- Personalized Retention Strategies: Offer targeted incentives like discounts, loyalty perks, or VIP experiences for high-value customers.

- Proactive Churn Prevention: Identify customers at risk of churn (e.g., those showing reduced engagement) and re-engage them via personalized outreach.

- Data-Driven Cohort Analysis: Compare cohorts to understand which customer groups need additional support and refine marketing strategies accordingly.


## Technical Details
- **Database:** PostgreSQL
- **Analysis Tools:** PostgreSQL
- **Visualization:** PowerBI 
```