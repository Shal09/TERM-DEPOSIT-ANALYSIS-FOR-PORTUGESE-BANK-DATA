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

Calculation of Value of the Cost to bank by taking the following:
Loan Interest Rate = 6% (taken from the website of the bank)

Term Deposit Rate = 3.2% (taken from the website of the bank)

We are assuming that the customer is investing 35% of the balance.

Call/sms cost = 1 Eur

**Total Profit Calculation by the bank for One customer:
**
0.35*balance*(Loan Interest Rate - Term Deposit Rate) – Call/sms cost

Total Net Profit incurred by the bank using the model :  5793813.94

Mean profit(individual profit average) incurred by the bank :  1690.14

False Negative:  479

False Positive:  576

True Negative:  2474

True Positive:  2852

TruePositiveRate/Sensitivity:  0.8561993395376764

FalsePositiveRate/Fallout:  0.18885245901639344

TrueNegativeRate/Specificity:  0.8111475409836065

FalseNegativeRate/Miss:  0.14380066046232362

Accuracy:  0.8346654129446796

Precision:  0.8319719953325554

Recall:  0.8561993395376764

F1Score:  0.8439118212753366

P(positive):  0.5220184923993104

P(negative):  0.4779815076006895

**Clustering**

Number of data points in cluster 0 with y-coordinate 0: 3525

Number of data points in cluster 0 with y-coordinate 1: 3459


Number of data points in cluster 1 with y-coordinate 0: 158

Number of data points in cluster 1 with y-coordinate 1: 227


Number of data points in cluster 2 with y-coordinate 0: 20

Number of data points in cluster 2 with y-coordinate 1: 29


Number of data points in cluster 3 with y-coordinate 0: 655

Number of data points in cluster 3 with y-coordinate 1: 1040


Number of data points in cluster 4 with y-coordinate 0: 0

Number of data points in cluster 4 with y-coordinate 1: 2


Cluster and Conversion rate: [[0, 49.53], [1, 58.96], [2, 59.18], [3, 61.36], [4, 100.0]]


Average account balance of people who deposit their money: 2003.46
