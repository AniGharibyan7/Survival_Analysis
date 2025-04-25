# Survival Analysis Report - Telecom Customer Churn

## Factors Affecting Churn Risk

Based on my analysis of the telecom customer dataset using the LogNormal Accelerated Failure Time (AFT) model, I have identified several key factors affecting customer churn risk:

- **Tenure**: Higher tenure strongly correlates with lower churn probability (evident in the tenure distribution plot), confirming that customers who have been with the company longer are more likely to stay.

- **Internet Service**: Internet service subscription is the strongest predictor of customer retention with exp(coef) = 0.42, indicating that customers with internet service have less than half the churn risk of those without it.

- **Service Type**: Plus service customers have the lowest churn probability (4.6%), while Basic service customers have the highest (18.9%), demonstrating that comprehensive service packages significantly reduce churn risk.

- **Age**: Older customers tend to have longer customer lifetimes, with exp(coef) = 1.04, pointing to higher loyalty among older demographic segments.

- **Marital Status**: Unmarried customers have lower expected tenure (exp(coef) = 0.65) compared to married customers.

- **Voice Service**: Customers with voice services show significantly lower churn risk (exp(coef) = 0.64).

## Most Valuable Customer Segments

My definition of valuable customers combines high Customer Lifetime Value (CLV) with relatively low churn risk. The most valuable segments are:

1. **Plus Service Customers**: These customers have the highest average CLV ($1,443.77) and the lowest churn probability (4.6%), making them the most valuable segment by far.

2. **E-Service Customers**: With the second highest CLV ($1,401.49) and very low churn probability (6.8%), these customers also represent a highly valuable segment.

3. **Customers with Internet Service**: Internet service strongly correlates with retention and higher CLV values, indicating that service bundling creates stickier customer relationships.

Interestingly, my analysis revealed zero overlap between high-value and high-risk customers, indicating a strong inverse relationship between customer value and churn risk in this dataset. This suggests the high-value customers are already quite loyal.

## Retention Budget and Recommendations

Assuming this dataset represents the entire customer population, I recommend an annual retention budget of $6,347.52. This calculation is based on:
1. Identifying high-value customers (top 25% by CLV)
2. Calculating their potential revenue loss using their CLV values and 12-month churn probabilities
3. Setting the retention budget at 15% of the potential revenue loss ($42,316.83)

Since I discovered zero overlap between high-value and high-risk customers, I've calculated this based on all high-value customers and their average churn probability. This approach ensures we protect the most valuable customer segments even if their individual churn risk is relatively low.

This budget should be allocated to:

1. **New Customer Retention**: The tenure distribution clearly shows that churn risk is highest in the first 24 months. Implementing special onboarding and early relationship management programs could significantly reduce early churn.

2. **Basic Service Upgrades**: With the highest churn rate (18.9%), Basic service customers represent the greatest retention opportunity. Incentivizing these customers to upgrade to Plus or E-service packages could improve both retention and CLV.

3. **Internet Service Adoption**: Given that internet service is the strongest predictor of retention, creating compelling offers to add internet service for voice-only customers could substantially reduce churn.

4. **Service Bundling**: The data clearly shows that customers with more comprehensive service packages have lower churn rates. Creating attractive bundle offers could encourage higher service adoption and improved loyalty.

5. **Targeted Age Demographics**: Younger customers show higher churn rates, suggesting that age-appropriate retention offers might be effective for this demographic.

By focusing retention efforts on these specific segments and addressing the key factors driving churn, the company can significantly improve customer lifetime value and overall profitability while making efficient use of the retention budget.
