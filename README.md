# Churn Status Prediction

## Introduction:
Customer churn is the percentage of customers who stopped using a company's products or services during a specified time period.

Measuring customer churn is important for several reasons:

- **Revenue Impact:** High customer churn means loss of recurring revenue.

- **Customer Insights:** Understanding why customers leave can provide valuable insights into product or service shortcomings, and areas needing improvement.

- **Cost Efficiency:** Acquiring new customers is often more expensive than retaining existing customers.

**Date Source:** Customer Churn dataset on [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn) 

<br>

## Exploratory Data Analysis:

![Visualizing Churn Status](/images/1.png)

Out of the total customer base, **5,174** customers did not churn, while **1,869** customers have churned. This indicates that approximately **26.5%** of the customers have left, meaning a significant portion of the customers are loyal, but there is still a notable number of customers leaving.

<br><br>

![Visualizing Customer Churn by Gender](/images/2.png)

**Overall Churn:**

- The total number of customers who have not churned (5,174) is significantly higher than those who have churned (1,869). This indicates a relatively high retention rate.

**Gender Distribution in Churn:**

- Among those who have not churned, there are slightly more male customers (2,625) compared to female customers (2,549).
- Among those who have churned, the numbers for females (939) and males (930) are almost equal.

**Gender-wise Churn Rate:**

- For Females: 939 out of 3,488 total female customers have churned. This gives a churn rate of approximately 27%.
- For Males: 930 out of 3,555 total male customers have churned. This gives a churn rate of approximately 26%.

**Key Takeaways:**

- The overall retention rate is strong, but there is still a notable percentage of customers who are churning.

- Both male and female customers are churning at similar rates, with a very slight difference favoring male retention.

- While the number of male and female customers is almost balanced, any strategies to further reduce churn could consider targeted approaches for each gender.

<br><br>

![Visualizing Customer Churn by Senior Citizen Status](/images/3.png)

**Non-Senior Citizens:**

- 76.4% No Churn: The majority of non-senior citizen customers do not churn, indicating a higher level of satisfaction or retention among this group.

- 23.6% Churn: A smaller portion of non-senior citizens churn, suggesting that there may still be some concerns or issues leading to churn in this group.

**Senior Citizens:**

- 58.3% No Churn: A little more than half of the senior citizen customers do not churn. This is a lower retention rate compared to non-senior citizens.

- 41.7% Churn: A significant portion of senior citizens churn, indicating that this group has higher dissatisfaction or retention challenges.

**Recommendations:**

- The company can consider conducting detailed surveys or focus groups with senior citizen customers to understand their specific pain points and preferences.

- The company can create tailored offerings or support services specifically designed to address the needs and concerns of senior citizens.

<br><br>

![Visualizing the Distribution of Customers by Contract Type and Churn Status](/images/4.png)

**Month-to-Month Contract:**

- Total customers: 3,875 (2,220 no churn + 1,655 churn)
- Churn rate: **43%** (1,655 churn out of 3,875)

**One Year Contract:**

- Total customers: 1,473 (1,307 no churn + 166 churn)
- Churn rate: **11%** (166 churn out of 1,473)

**Two Year Contract:**

- Total customers: 1,695 (1,647 no churn + 48 churn)
- Churn rate: **3%** (48 churn out of 1,695)

**Higher Retention for Longer Contracts:**

- The churn rate is significantly higher for customers on month-to-month contracts compared to those on one-year or two-year contracts.
- Longer-term contracts have much lower churn rates.

**Customer Loyalty:**

- Customers with longer-term contracts demonstrate stronger loyalty, as seen by their lower churn rates.
- This suggests that longer-term contracts may provide a sense of commitment and stability for customers.

**Opportunity for Upselling:**

- There is an opportunity to reduce churn by encouraging customers on month-to-month contracts to switch to longer-term contracts.
- Offering incentives, discounts, or additional benefits for signing longer-term contracts could be effective.

<br>

## Classification Model Evaluation:

In this classification machine learning project, a false positive and a false negative are two types of prediction errors that can occur.

- A false positive (Type I Error) is when the model incorrectly predicts that a customer will churn when, in reality, they will stay.
- A false negative (Type II Error) happens when the model incorrectly predicts that a customer will stay when, in fact, they will churn.

In the context of churn prediction, a false negative can be considered more costly than a false positive. With a false negative, the company misses the opportunity to take proactive measures to retain the customer. This can result in lost revenue and potentially long-term negative effects on customer loyalty and brand reputation. False negatives mean that the company misses out on the opportunity to engage with the customer and address any issues they may have, which could have been resolved to prevent churn.

<br>

![Classification Metrics](/images/5.png)

- Higher Precision indicates that a model has fewer false positives.
- Higher Recall means that the model has fewer false negatives.
- For this use case the most important metric to prioritize is Recall, because the cost of missing a potential churn (false negative) is typically higher than the cost of incorrectly predicting a churn (false positive).

<br>

## Final Model and Predictions:
The model that had the highest Recall value was the AdaBoost classifier, and it will be used to make customer churn predictions.

<br>

![Predictions](/images/6.png)

<br>

## Key Takeaways:

- Customers with month-to-month contracts have a significantly higher churn rate compared to those with one-year or two-year contracts. This indicates that customers on shorter-term contracts are more likely to leave.

- Customers with higher monthly charges tend to have a higher churn rate. This suggests that cost sensitivity is a significant factor in customer retention, and customers may be seeking more affordable alternatives.

- Customers with longer tenure are less likely to churn. This indicates that once customers are engaged and satisfied over a longer period, they tend to remain loyal to the company.

<br>

## Recommendations:

- The company can consider encouraging customers to switch from month-to-month contracts to one-year or two-year contracts by offering incentives such as discounts, additional benefits, or loyalty rewards. This can help reduce churn rates and increase customer retention.

- Another consideration can be implementing strategies to address cost sensitivity among customers with higher monthly charges. This could include offering tiered pricing plans, bundling services at a discounted rate, or providing personalized offers based on customer usage patterns.

- Focusing on improving the onboarding experience and providing exceptional support during the initial months of a customer's tenure can help build strong relationships early on and reduce the likelihood of churn.


**Please click [here](https://github.com/eric5412/Churn-Status-Prediction/blob/main/customer%20churn%20project.ipynb) for the entire project.**

<br><br>
<br><br>
