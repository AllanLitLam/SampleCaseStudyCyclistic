# Cyclistic Bike-Share Case Study
---

## Introduction 

This case study investigates how casual riders and annual subscribers use the Cyclistic (a bike-sharing company) service differently. This case study uses publicly available data from the [Divvy Bike Share System Data](https://divvybikes.com/system-data) to analyze user behavior and provide actionable insights for Cyclistic's business growth. The data is publicly available under a data license agreement provided by [Motivate International Inc](https://divvybikes.com/data-license-agreement). Data analysis and data visualizations were conducted in R.

---

## R Code and Analysis Method
- Descriptive summary statistics
- GLM 
- ANOVA

Analysis Scripts:
- [Cyclistic Bike-Share Case Study.Rmd](./Cyclistic-Bike-Share-Case-Study.Rmd) 

---

## Business Problem

The core business problem is to increase profitability by converting casual riders into annual subscribers. My analysis aims to answer: What are the key behavioral differences between casual and annual riders, and how can we leverage these differences to create an effective marketing campaign that drives conversions?

My analysis revealed two significant behavioral patterns:

1. I found that casual customers ride for a significantly longer average duration (77 minutes) compared to annual subscribers (12 minutes). My analysis using a Gamma regression model confirmed this, showing that being an annual subscriber is associated with a 64% decrease in ride duration (p<0.001).
   
2. However, the annual subscribers took significantly more ride trips on average (720,313) than casual customers (71,526). I used a Poisson regression model to confirm this, showing that annual subscribers took about 10.07 times more trips than casual customers (p < .001).

Therefore, casual customers took more valuable ride trips than annual subscribers. Fewer trips, but each with a longer ride duration. 

---

## Recommendation: Create a ride-time-based incentive plan for casual customers

To convert casual riders into annual members, we can create a tiered discount plan based on their cumulative ride time. My analysis shows that the average casual ride is 77 minutes, which is a powerful insight we can leverage.

Proposed Discount Structure:

* Tier 1: Casual riders who have logged a cumulative ride time of 77 minutes or more in a year are eligible for a 7% discount on a new annual membership.

* Tier 2: To further incentivize long-distance riders, an additional 1% discount can be awarded for every 30 minutes of cumulative ride time beyond the initial 77 minutes, up to a maximum discount of 10%. This cap ensures the profitability of the plan.

This campaign is specifically designed to target the most valuable segment of casual riders, especially those who already use the service for longer trips. While casual riders, as a group, take fewer trips than members (average of 71,526 total trips for all casuals vs. 720,313 for all members), this plan focuses on capturing their unique, high-value behavior: the extended ride. Limiting the total number of rides aggregated for a single customer for this campaign (e.g., to a reasonable personal cap) will ensure it remains a program for casuals and not a loophole for members.

- **Pros1:** This campaign targets high-value casual riders who already use Cyclistic frequently and have found value in those purchased trips. They are more likely to be converted to annual members than riders who do not use the app as much. 

- **Cons1:** This program may incentivize existing members to cancel their membership and rejoin later at the discounted rate. This risk could be mitigated by implementing a waiting period for former members to rejoin at a discounted rate or by restricting the campaign to new sign-ups only.

- **Cons2:** Although the mean number of trips for all casual riders was 71,526, using this as a per-customer limit is impractical and could be confusing. A better approach would be to focus the campaign solely on ride duration, as this is the core behavior identified in high-value casual riders. Experimentation, possibly through A/B testing, would be crucial to determine the most effective incentive tiers and ensure the program is both profitable and appealing to customers.

---

## Conclusions 
My analysis of Cyclistic's rider data revealed a fundamental behavioral difference: while annual members are frequent riders who take short trips, casual customers, though less frequent, are the ones who consistently take longer, more valuable rides.

Therefore, a marketing strategy focused on both the ride duration and ride count is the most effective way to convert these high-value casual riders. The proposed tiered discount plan, which uses cumulative ride time as a direct incentive, is specifically designed to capture this unique behavior and create a strong financial reason for casuals to commit to an annual membership.

By targeting casual riders who already find significant value in extended trips, this strategy is likely to improve conversion rates and increase overall profitability. It leverages a previously untapped metric (ride duration) to create a compelling offer that rewards the very behavior we want to encourage among new subscribers.

---

## Next Steps

To validate this recommendation, my next steps would involve building a pilot program to A/B test this new campaign against existing marketing efforts. I would also recommend a deeper analysis of the seasonal and geographic patterns of long-distance rides to further optimize campaign targeting and messaging. This data-driven, iterative approach will ensure we maximize our return on investment.

