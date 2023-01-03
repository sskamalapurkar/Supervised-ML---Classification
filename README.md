# **Credit Card default Prediction** 
**Introduction**

Banks all around the world would receive countless applications for loans every day. Some of them are good and will be repaid, but there is a still high risk that one creditor defaults his/her loans. How could we prevent this problem from happening? Or, in another word, how could we know in advance which creditors are trustworthy? 
     
In recent years, the credit card issuers in Taiwan faced the cash and credit card debt crisis and the delinquency is expected to peak in the third quarter of 2006 (Chou,2006). In order to increase market share, card-issuing banks in Taiwan over-issued cash and credit cards to unqualified applicants. At the same time, most cardholders, irrespective of their repayment ability, overused credit card for consumption and accumulated heavy credit and cash–card debts. The crisis caused the blow to consumer finance confidence and it is a big challenge for both banks and cardholders.

This project is aimed at predicting the case of customers default payments in Taiwan. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. We can use the K-S chart to evaluate which customers will default on their credit card payments.

The main objective is to build a predictive classification model, which could help in predicting the defaulters among the credit card users.

# **DATA DESCRIPTION:**

**Attribute Information:**

This research employed a binary variable, **default payment (Yes = 1, No = 0)**, as the response variable. This study reviewed the literature and used the following 23 variables as explanatory variables:

**X1:** Amount of the given credit (NT dollar): it includes both the individual consumer credit and his/her family (supplementary) credit

**X2:** Gender (1 = male; 2 = female)

**X3:** Education (1 = graduate school; 2 = university; 3 = high school; 4 = others; 5 = unknown; 6 = unknown)

**X4:** Marital status (1 = married; 2 = single; 3 = others)

**X5:** Age (year)

**X6 - X11: History of past payment. We tracked the past monthly payment records (from April to September, 2005) as follows:**

**X6 =** the repayment status in September, 2005

**X7 =** the repayment status in August, 2005

**X8 =** the repayment status in August, 2005

**X9 =** the repayment status in August, 2005

**X10 =** the repayment status in August, 2005

**X11 =** the repayment status in April, 2005

**The measurement scale for the repayment status is: -2 = No consumption; -1 = pay duly; 0 = use of revolving credit (paid minimum only); 1 = payment delay for one month; 2 = payment delay for two months; . . .; 8 = payment delay for eight months; 9 = payment delay for nine months and above.**

**X12-X17: Amount of bill statement (NT dollar)**

**X12 =** amount of bill statement in September, 2005

**X13 =** amount of bill statement in August, 2005

**X14 =** amount of bill statement in September, 2005

**X15 =** amount of bill statement in September, 2005

**X16 =** amount of bill statement in September, 2005

**X17 =** amount of bill statement in April, 2005

**X18-X23: Amount of previous payment (NT dollar)**

**X18 =** amount paid in September, 2005

**X19 =** amount paid in August, 2005

**X20 =** amount paid in August, 2005

**X21 =** amount paid in August, 2005

**X22 =** amount paid in August, 2005

**X23 =** amount paid in April, 2005

**What is credit card default?**

>Credit card default happens when you have become severely delinquent on your credit card payments. Default is a serious credit card status that affects not only your standing with that credit card issuer but also your credit standing in general and your ability to get approved for other credit-based services.


**How Credit Card Default Happens?**

>When you accept a credit card, you agree to certain terms. For example, you agree to make your minimum payment by the due date listed on your credit card statement. If you miss the minimum payment six months in a row, your credit card will be in default. Your credit card issuer will likely close your account and report the default to the credit bureaus.

**Approach Taken**
1. Data inspection and cleaning
2. Explored data, checked for null and duplicate values
3. Data Pre-processing
4. EDA on features
- Univariate, Bivariate and Multivariate analysis
- Checked distributions of numeric variable
- Checked for imbalance of the dataset. Handled imbalance by oversampling the minor class, using SMOTE
5. Modelling (Implementing Machine Learning Algorithms)
- Logistic Regression
- Decision Tree
- Random Forest
- SVM
6. Hyperparameter tuning for some models
7. Evaluated all models based on metrics such as - Accuracy, Precision, Recall, Confusion Matrix, f1 score
8. Model Selection

# **Conclusions**

> 1. Among all 4 models which we tried to build here to predict defaulters correctly, Random Forest is the best and robust model with 82% recall score, which is very good.
> 2. According to RandomForest model, features like **paid_total, total_bill, dues, cred_lim, age, repay_status_sep_2, repay_status_aug_1 and marriage status as married** are found to be **most important features to predict future defaulters.**
> 3. The credit card holder has paid minimum credit amount for past 6 months, also for every month if the dues of that customers are increasing, then it is obvious that the customer will have default for sure!
> 4. While this age and limit_bal are the other two important predictors as we discussed in the data preparation part. This also makes sense because as one gets older, one is more likely to accumulate more resource and cares more about his reputations, which makes credit default less likely. Also, if one and one’s family get more given credits, the person is more likely to live in a wealthier environment which also makes credit default less likely.
> 5. Further, repay status is also playing a vital role in predicting future defaulters. If the creditor is not repaying for the past one or more months, he is more likely to default in upcoming months.


At the end of the day, having the ability to predict 82% (recall score) of potential defaults would save a-lot of money on credit card charge-offs. Obviously, real-world application is more nuanced, but this modeling process is a step in the right direction.
          
**THANK YOU !**
