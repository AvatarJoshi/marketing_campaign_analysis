# Analysis of Marketing Campaign Results

# Overview

## Background
Freedom Debt Relief is an organization that helps individuals who have accrued significant debt as a result of unexpected hardship and are no longer able to meet their minimum monthly requirements. Upon enrolling in Freedom’s Debt Relief program, customers cease making payments to their creditors and instead make deposits they can afford into a new dedicated bank account with Freedom. Freedom uses these funds to negotiate with each of the client’s creditors to settle the debt, typically at only a fraction of what was originally owed. Freedom collects fees (proportional to the monthly deposited amount) from the client for agreements it successfully negotiates.

## Objectives
Freedom recently ran a marketing campaign to promote their debt relief program. The cost of the campaign was $5 million. The campaign was run during month 3. The overarching goal of this project is to:

1. Provide a quantitative assessment of whether the marketing campaign was successful. Explain why these metrics were choosen.

2. Recommend ways the campaign strategy can be adjusted in the future to improve performance.

# Resources

[client_data](/resources/datasets/client_data.csv) - Contains data regarding client's age, residence status, and geographical region

[deposit_data](/resources/datasets/depost_data.csv) - Contains data regarding client deposit behavior. These include deposit type, deposit amount, deposit cadence, and deposit date.

[calendar_data](/resources/datasets/calendar_data.csv) - Contains calendar information in relation to deposit and client datasets.

# Results

## Question 1: Provide a Quantitative Assessment of the Marketing Campaign's Success
In order to quantify the success of the marketing campaign, the monetary value of deposits over the course of the 5 month period was assessed. Below we can see that a substantial increase in total deposits was observed while the marketing campaign was running (month 3) and that total deposits remained high after the campaign ended (months 4 and 5).

![Total_Deposit_Amount](/resources/images/deposit_amount_by_month.png)

On average, Freedom charges a fee of 21.5% of the total amount of debt that they are able to settle on behalf of their clients. Therefore, the total deposit amount per month was multiplied by 0.215 to calculate the profit per month.

![Profit_Per_Month](/resources/images/profit_by_month.png)

On average, the profit per month before the campaign was ~$6.3 million while after the campaign it was ~$8.3 million. This indicates the marketing campaign increased profit ~$2 million per month. 

To better understand the cost and benefits of the marketing campaign, hypothetical data was generated to show total profit over a 12 month period with/without the campaign. It was assumed that profit each month would reflect the average profit per month before and after the campaign (before = $6.3 million and after = $8.3 million). In addition, since the marketing campaign cost $5 million the with campaign began at -$5 million. We can see that by the 4th month the campaign would have increased profits by $700,000 and by the 12th month profits would be icnreased by $15,900,000. 

![Hypothetical Profit](/resources/images/hypothetical_profit.png)

Based on this data, it appears the marketing campaign will have been well worth the $5 million investment provided there isn't a significant increase in client churn or significant changes in client's depoist amounts.

## Question 2: Recommend Ways to Improve the Marketing Campaign
The marketing campaign couuld be improved by targeting specific groups that enrolled as a result of the marketing strategy and also make higher value deposits each month. 

First, clients were grouped based on age and the change in client's based on age was graphed. We can see that the marketing campaign was successful in generating new clients across most age groups. However, this was most prominent in individuals between 31-70 years of age. 

![Deposit_by_Age](/resources/images/total_deposit_amount_by_age_each_month.png)


We also observe that individuals who own homes were also more responsive to the marketing campaign.

![Owner_Renter](/resources/images/number_of_owners_vs_renters_each_month.png)

We find similar trends when we look at the total number of Freedom's clients that are renters vs owners by age.

![Owner_Renter_Age](/resources/images/client_residence_status_by_age.png)

Based on this data, future marketing campaigns could be targeted at middle aged individuals and those who are home owners. 


# Summary
This project focused on analyzing the success of a marketing campaign and identifying ways to improve it during future iterations. The campaign was found to result in a ~$2 million per month increase in profits when compared to pre-campaign data. Even accounting for the cost of the campaign, if trends hold, it is expected an additional $16 million in profit would be generated 1 year after the campaign compared to if the campaign had not been run at all. Finally, the largest increases in clients as a result of the marketing campaign were from middle aged individuals and those who are home owners. Based on this, future campaigns could focus their efforts on targeting individuals belonging to these groups.