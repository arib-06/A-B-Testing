# A/B Testing Analysis: Marketing Campaign Effectiveness

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Statsmodels](https://img.shields.io/badge/Statsmodels-7db049?style=for-the-badge)
![Matplotlib](https://img.shields.io/badge/Matplotlib-315e73?style=for-the-badge)

## Executive Summary

This project conducts a comprehensive A/B testing analysis to evaluate and compare the effectiveness of two distinct marketing strategies: the **Control Campaign** and the **Test Campaign**. By leveraging statistical hypothesis testing, we aim to determine which campaign yields a significantly higher conversion rate and provides better ROI for the business.

The analysis concluded that the **Control Campaign** significantly outperformed the Test Campaign, achieving a conversion rate of **9.83%** compared to **8.64%**, with a statistically significant p-value of **0.026**.

## Project Objective

The primary goal is to perform a data-driven evaluation of marketing performance. We focus on:
- Analyzing key performance indicators (KPIs) across both campaign groups.
- Statistically validating the difference in conversion rates.
- Providing actionable business recommendations based on the findings.

## Data Dictionary

The dataset includes the following metrics for both Control and Test campaigns:

| Metric | Description |
| :--- | :--- |
| **Campaign Name** | The identifier for the experimental group (Control or Test). |
| **Date** | The date of the observed metrics. |
| **Spend [USD]** | Total financial investment in the campaign on a given day. |
| **Impressions** | Total number of times the advertisement was displayed. |
| **Reach** | Number of unique users who saw the advertisement. |
| **Clicks** | Number of times the advertisement was clicked. |
| **Searches** | Number of users who performed a search on the website after seeing the ad. |
| **Content Views** | Number of users who viewed product details. |
| **Add to Carts** | Number of users who added a product to their shopping cart. |
| **Purchases** | Number of users who completed a transaction. |
| **Conversion Rate** | The ratio of Purchases to Content Views (or relevant engagement metric). |

## Statistical Methodology

To determine the effectiveness of the campaigns, we employed a **one-tailed Z-test for proportions**.

### Hypothesis Formulation
- **Null Hypothesis ($H_0$):** There is no significant difference between the conversion rates of the Control and Test campaigns, or the Test campaign performs better.
  $$H_0: p_{control} \leq p_{test}$$
- **Alternative Hypothesis ($H_1$):** The Control campaign has a significantly higher conversion rate than the Test campaign.
  $$H_1: p_{control} > p_{test}$$

### Significance Level
The test was conducted at a significance level ($\alpha$) of **0.05**.

## Key Results & Insights

The statistical analysis yielded the following results:

- **Control Campaign Conversion Rate:** 9.83%
- **Test Campaign Conversion Rate:** 8.64%
- **Calculated P-Value:** 0.026

Since the p-value ($0.026$) is less than the alpha level ($0.05$), we **reject the Null Hypothesis**. There is sufficient evidence to conclude that the Control Campaign's conversion rate is statistically significantly higher than that of the Test Campaign.

## Business Recommendations

Based on the statistical findings, the following recommendations are proposed:
1. **Prioritize Control Campaign Strategy:** Since the Control Campaign demonstrated a superior conversion rate, its underlying marketing strategy (e.g., creative assets, targeting, or messaging) should be prioritized for future scaling.
2. **Review Test Campaign Elements:** Analyze the specific components of the Test Campaign to identify why it underperformed. It may be that the new strategy reached a broader but less engaged audience.
3. **Optimize Spend Allocation:** Reallocate budget from the Test Campaign to the Control Campaign or a modified version that incorporates successful elements from both.
4. **Iterative Testing:** Continue performing A/B tests on specific sub-variables (e.g., ad placement or copy) within the successful Control strategy to further optimize performance.

## Technology Stack
- **Python**: Core programming language for analysis.
- **Pandas & NumPy**: Data manipulation and numerical computation.
- **Statsmodels**: Statistical modeling and hypothesis testing.
- **Matplotlib**: Data visualization.

---
*This analysis serves as a professional case study in data-driven marketing decision-making.*
