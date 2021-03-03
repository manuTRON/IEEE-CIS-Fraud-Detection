# IEEE-CIS Fraud Detection
## Description
Imagine standing at the check-out counter at the grocery store with a long line behind you and the cashier not-so-quietly announces that your card has been declined. In this moment, you probably aren’t thinking about the data science that determined your fate. While perhaps cumbersome (and often embarrassing) in the moment, this fraud prevention system is actually saving consumers millions of dollars per year. Researchers from the IEEE Computational Intelligence Society (IEEE-CIS) want to improve this figure, while also improving the customer experience. With higher accuracy fraud detection, you can get on with your chips without the hassle.

## Problem Statement
Make e-commerce safer by detecting fraud detection in real time and accurately.
## Sources/Useful Links
* https://www.kaggle.com/c/ieee-fraud-detection/data
* https://www.kaggle.com/c/ieee-fraud-detection/discussion/111284#latest-670375
* https://www.kaggle.com/cdeotte/xgb-fraud-with-magic-0-9600/output
* https://www.kaggle.com/c/ieee-fraud-detection/discussion/101203#latest-671062
* https://www.kaggle.com/c/ieee-fraud-detection/discussion/99979#latest-648115 *https://www.kaggle.com/c/ieee-fraud-detection/discussion/111308#latest-664620
## Real world/Business Objectives and constraints
Precisely detect a fraud transaction.
## Machine Learning Probelm
## Data Information
Source: https://www.kaggle.com/c/ieee-fraud-detection/data

The data is broken into two files identity and transaction, which are joined by TransactionID. Not all transactions have corresponding identity information.

## Categorical Features - Transaction
* ProductCD
* card1 - card6
* addr1, addr2
* P_emaildomain
* R_emaildomain
* M1 - M9
## Categorical Features - Identity
* DeviceType
* DeviceInfo
* id_12 - id_38

The TransactionDT feature is a timedelta from a given reference datetime (not an actual timestamp).

## Mapping the real world problem to an ML problem
It is a binary classification problem, for a transaction we need to predict if it is fraud or not.
## Performance Metric
Source: https://www.kaggle.com/c/ieee-fraud-detection/overview/evaluation

## Metric:

area under the ROC curve
