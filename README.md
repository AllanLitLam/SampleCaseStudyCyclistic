# Cyclistic Bike-Share Case Study
---

## Introduction 

This case study investigates how casual riders and annual members use the Cyclistic (a bike-sharing company) service differently. The analyzed dataset originates from the [Divvy Bike Share System Data](https://divvybikes.com/system-data), which is publicly available under a data license agreement provided by [Motivate International Inc](https://divvybikes.com/data-license-agreement). The data analysis and data visualizations were conducted in R.

---

## Business Problem

The executive team at Cyclistic wants to convert casual customers into annual subscribers to drive profitability. Therefore, they are seeking my data-driven insights to design new marketing strategies for this purpose. I identified two business problems: 

A. How do annual subscribers and casual customers use bikes differently?
  
B. What insights from these differences can drive marketing strategy?

Data suggests that：

1. On average, casual customers took significantly longer rides (Mean = 76.93 minutes) than annual subscribers (Mean = 12.11 minutes). A Gamma regression model indicated a strong negative effect of being an annual subscriber, where their average ride lengths were about 64% shorter than those of casual customers (p < .001).
   
2. Overall, annual subscribers take  significantly more ride trips (Mean = 720,313) than casual customers (Mean = 71,526). A Poisson regression model indicated a strong positive effect of being an annual subscriber, where annual subscribers took about 10.07 times more trips than casual customers (p < .001).

---

## Solutions 
Recommendation: Create an incentivized subscriber plan for longer rides
Since casual customers tend to ride for longer durations, we can create sign-up bonuses for annual membership that reward longer riding. For instance, if you aggregate 60 minutes of total ride time, you can purchase an annual membership at a discounted rate or earn free trips by signing up. 

Pros: Specifically targeted for casual customers

Cons: Limit reach for infrequent riders in general 

---

## Conclusions 
Casual customers used Cyclistic less frequently, but whenever they ride, they tend to ride longer than annual subscribers. Therefore, by tokenizing longer ride time as a sign-up incentive, the new marketing strategy can effectively target customers who already knew and used Cyclistic, and introduce a stronger desire for them to rely on Cyclistic more. 

