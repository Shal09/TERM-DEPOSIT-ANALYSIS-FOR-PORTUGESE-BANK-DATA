# TERM-DEPOSIT-ANALYSIS-FOR-PORTUGESE-BANK-DATA

![image](https://github.com/user-attachments/assets/0c32bc34-bbbc-40ac-8c58-cb5c86b9509a)


**Aim of the project:**

1. To create a system that helps us decide which customers to target in our
marketing campaigns for term deposits. This system will predict if a customer is likely to
say "yes" or "no" to a term deposit offer.

2. Calculated the Expected Value Framework which is the based on the Machine Learning
Prediction and taking managerial decision.

3. Clustering is explored to find customers who should be targeted for successful
conversion.

**Introduction**

A term deposit is a fixed-term investment that includes the deposit of money into an account at a
financial institution. Term deposit investments usually carry short-term maturities ranging from
one month to a few years and will have varying levels of required minimum deposits. The
investor must understand when buying a term deposit that they can withdraw their funds only
after the term ends. In some cases, the account holder may allow the investor early termination or
withdrawal if they give several days notification. Also, there will be a penalty assessed for early
termination.

A lot of people are influenced by marketing campaign for buying a product.
The bank offer term deposit in a higher percentage of interest than savings account as it wants to
invest the term deposit amount in giving loan to the other customer at higher rate and earn more
profit from it. Banks offer term deposit accounts in the terms that the customer does not
withdraw their funds for a fixed period in return for a higher rate of interest paid on the account.


A Portuguese bank data is collected from 2008 to 2013

<img width="1035" alt="image" src="https://github.com/user-attachments/assets/c2b97f13-7643-4c3a-8eff-e47a68f85745" />


**Data Understanding**

Extracted data from UCI machine learning Repository.
https://archive.ics.uci.edu/dataset/222/bank+marketing to conduct the analysis on the Portuguese
banking institution with a goal to predict term deposit which is indicated with a categorical
response variable ‘y’- no or yes.
Instances: 45211 and Features: 16

**Accuracy score of the model**

<img width="839" alt="image" src="https://github.com/user-attachments/assets/2486545a-ae85-46bc-b589-ae006c516076" />


**EXPECTED VALUE FRAMEWORK**

1. Profitability Calculation
   
The formula for total profit for a single customer:

Profit=0.35×balance×(Loan Interest Rate−Term Deposit Rate)−Call/SMS cost

Given:

Loan Interest Rate = 6% = 0.06

Term Deposit Rate = 3.2% = 0.032

Investment Fraction = 0.35

Call/SMS Cost = €1

The profit for one customer depends on their balance.

Aggregate Metrics:

Total Net Profit = €5,793,813.94

Mean Profit per Customer = €1,690.14

These values indicate the overall profitability and average return on engaging with each customer, after accounting for engagement costs.

2. Classification Metrics
   
The classification metrics assess the performance of a model used for decision-making:

•	True Positive (TP): 2,852 — Customers correctly identified as profitable.

•	False Positive (FP): 576 — Non-profitable customers incorrectly classified as profitable.

•	True Negative (TN): 2,474 — Non-profitable customers correctly classified.

•	False Negative (FN): 479 — Profitable customers missed by the model.

<img width="670" alt="image" src="https://github.com/user-attachments/assets/cc038840-64c6-47e2-8490-c4746416203e" />


3. Business Implications
   
Profitability: The positive net profit and mean profit suggest the model is effective in identifying customers that generate significant returns for the bank.

Missed Opportunities (FN): The 479 false negatives highlight potential areas to improve the model’s recall, as these represent missed profitable customers.

Overhead (FP): The 576 false positives represent costs incurred for targeting non-profitable customers.



**Clustering**

 The objective is to understand customer behavior and identify groups with higher likelihoods of subscribing to term deposits. Below is a summary of the clustering results and analysis.

 <img width="745" alt="image" src="https://github.com/user-attachments/assets/34ee4570-e290-451f-92ba-72e17beeaff8" />


Cluster 4 has the highest conversion rate (100%), though it contains only 2 data points.

Cluster 3 shows a high conversion rate of 61.36%, making it a significant group for targeting potential customers.

Clusters 1 and 2 also exhibit promising conversion rates, indicating opportunities for focused marketing strategies.

Average account balance of people who deposit their money: 2003.46

The clustering analysis provides valuable insights into customer behavior and can help the bank design targeted marketing strategies to increase term deposit subscriptions. Clusters with higher conversion rates should be prioritized for personalized campaigns.
