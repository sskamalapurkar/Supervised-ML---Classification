# **Credit Card default Prediction** 
**Introduction**
> In recent years, the credit card issuers in Taiwan faced the cash and credit card debt crisis and the delinquency is expected to peak in the third quarter of 2006 (Chou,2006). In order to increase market share, card-issuing banks in Taiwan over-issued cash and credit cards to unqualified applicants. At the same time, most cardholders, irrespective of their repayment ability, overused credit card for consumption and accumulated heavy credit and cash–card debts. The crisis caused the blow to consumer finance confidence and it is a big challenge for both banks and cardholders.

> This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. We can use the K-S chart to evaluate which customers will default on their credit card payments.

> The main objective is to build a predictive classification model, which could help in predicting the defaulters among the credit card users.
# **DATA DESCRIPTION:**

**Attribute Information:

This research employed a binary variable, **default payment (Yes = 1, No = 0)**, as the response variable. This study reviewed the literature and used the following 23 variables as explanatory variables:

**X1:** Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit

**X2:** Gender (1 = male; 2 = female)

**X3:** Education (1 = graduate school; 2 = university; 3 = high school; 4 = others; 5 = unknown; 6 = unknown)

**X4:** Marital status (1 = married; 2 = single; 3 = others)

**X5:** Age (year)

**X6 - X11: History of past payment. We tracked the past monthly payment records (from April to September, 2005) as follows:

**X6 =** the repayment status in September, 2005

**X7 =** the repayment status in August, 2005

**X8 =** the repayment status in August, 2005

**X9 =** the repayment status in August, 2005

**X10 =** the repayment status in August, 2005

**X11 =** the repayment status in April, 2005

**The measurement scale for the repayment status is: -2 = No consumption; -1 = pay duly; 0 = use of revolving credit (paid minimum only); 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.

**X12-X17: Amount of bill statement (NT dollar)

**X12 =** amount of bill statement in September, 2005

**X13 =** amount of bill statement in August, 2005

**X14 =** amount of bill statement in September, 2005

**X15 =** amount of bill statement in September, 2005

**X16 =** amount of bill statement in September, 2005

**X17 =** amount of bill statement in April, 2005

**X18-X23: Amount of previous payment (NT dollar)

**X18 =** amount paid in September, 2005

**X19 =** amount paid in August, 2005

**X20 =** amount paid in August, 2005

**X21 =** amount paid in August, 2005

**X22 =** amount paid in August, 2005

**X23 =** amount paid in April, 2005
