# Cyclistic Bike-Share Case Study
---

## Introduction 

This case study investigates how casual riders and annual members use the Cyclistic (a bike-sharing company) service differently. The analyzed dataset originates from the [Divvy Bike Share System Data](https://divvybikes.com/system-data), which is publicly available under a data license agreement provided by [Motivate International Inc](https://divvybikes.com/data-license-agreement). The data analysis and data visualizations were conducted in R.

---

## Business Problem

The executive team at Cyclistic wants to convert casual riders into annual members to drive profitability. Therefore, they are seeking my data-driven insights to design new marketing strategies for this purpose. I identified two business problems: 

A. How do annual members and casual riders use bikes differently?
  
B. What insights from these differences can drive marketing strategy?

Data suggests that：

1. On average, casual riders took significantly longer rides (Mean = 76.93 minutes) than annual members (Mean = 12.11 minutes). A Gamma regression model indicated a strong negative effect of being an annual member, where their average ride lengths were about 64% shorter than those of casual riders (p < .001).
   
2. Overall, annual members take  significantly more ride trips (Mean = 720,313) than casual riders (Mean = 71,526). A Poisson regression model indicated a strong positive effect of being an annual member, where annual members took about 10.07 times more trips than casual riders (p < .001).

3. 
