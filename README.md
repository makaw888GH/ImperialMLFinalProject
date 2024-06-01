# Customer Credit Scorecard

## NON-TECHNICAL EXPLANATION OF YOUR PROJECT
Apply machine learning to build a system which score customers for credit worthiness and and decide which customers is eligible for new offers. The ML scoring system must provide rationale to support the scoring output and enhance explainability.

## DATA
The dataset is from Kaggle titled Default of Credit Card Clients Dataset. https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset

<br>This dataset contains information on default payments, demographic factors, credit data, history of payment, and bill statements of credit card clients in Taiwan from April 2005 to September 2005.

There are 25 variables:

* ID: ID of each client
* LIMIT_BAL: Amount of given credit in NT dollars (includes individual and family/supplementary credit
* SEX: Gender (1=male, 2=female)
* EDUCATION: (1=graduate school, 2=university, 3=high school, 4=others, 5=unknown, 6=unknown)
* MARRIAGE: Marital status (1=married, 2=single, 3=others)
* AGE: Age in years
* PAY_0: Repayment status in September, 2005 (-1=pay duly, 1=payment delay for one month, 2=payment delay for two months, … 8=payment delay for eight months, 9=payment delay for nine months and above)
* PAY_2: Repayment status in August, 2005 (scale same as above)
* PAY_3: Repayment status in July, 2005 (scale same as above)
* PAY_4: Repayment status in June, 2005 (scale same as above)
* PAY_5: Repayment status in May, 2005 (scale same as above)
* PAY_6: Repayment status in April, 2005 (scale same as above)
* BILL_AMT1: Amount of bill statement in September, 2005 (NT dollar)
* BILL_AMT2: Amount of bill statement in August, 2005 (NT dollar)
* BILL_AMT3: Amount of bill statement in July, 2005 (NT dollar)
* BILL_AMT4: Amount of bill statement in June, 2005 (NT dollar)
* BILL_AMT5: Amount of bill statement in May, 2005 (NT dollar)
* BILL_AMT6: Amount of bill statement in April, 2005 (NT dollar)
* PAY_AMT1: Amount of previous payment in September, 2005 (NT dollar)
* PAY_AMT2: Amount of previous payment in August, 2005 (NT dollar)
* PAY_AMT3: Amount of previous payment in July, 2005 (NT dollar)
* PAY_AMT4: Amount of previous payment in June, 2005 (NT dollar)
* PAY_AMT5: Amount of previous payment in May, 2005 (NT dollar)
* PAY_AMT6: Amount of previous payment in April, 2005 (NT dollar)
* default.payment.next.month: Default payment (1=yes, 0=no)

### Acknowledgements
Any publications based on this dataset should acknowledge the following:
<br>Lichman, M. (2013). UCI Machine Learning Repository [http://archive.ics.uci.edu/ml]. Irvine, CA: University of California, School of Information and Computer Science.
<br>A summary of the data you’re using, remembering to include where you got it and any relevant citations. 

## MODEL 
The model selected is Logistic Regression (LR)

For this project based on time available (1 week) LR is the most used algorithm in the credit scorecard modeling process is Logistic Regression. Other algorithms which are suitable for later implementation include ensemble techniques, AdaBoostClassifier, GradientBoostingClassifier, RandomForestClassifier, ExtraTreesClassifier

Other reasons include :

* Simple linear relationship: the relationship between variables is a linear relationship
* Good Interpretability: the effect of input variables on target variables is readily available
* Give probabilities instead of discriminative classes: the customer’s characteristic information (such as marriage, age, historical credit performance, etc.) can be integrated and converted into a probability value, which provides an intuitive basis to predict whether the customer is good or bad. That is, the larger the value, the smaller the probability that the customer will default in the future.
* Easy to deploy: testing, deployment, monitoring, tuning, etc., are relatively simple

## HYPERPARAMETER OPTIMSATION

The list of hyperparameters that can be tuned can be found in the scikit learn documentation: https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html

The hyperparameters selected for tuning are the following:

* C: Inverse of regularization strength; must be a positive float. Like in support vector machines, smaller values specify stronger regularization
* penalty: {‘l1’, ‘l2’, ‘elasticnet’, None}, default=’l2’ Specify the norm of the penalty
* solver: Algorithm to use in the optimization problem. Default is ‘lbfgs’
* max_iterint, default=100 Maximum number of iterations taken for the solvers to converge

## RESULTS

![alt text](https://github.com/[username]/[reponame]/blob/[branch]/image.jpg?raw=true)

![alt_text](https://github.com/makaw888GH/ImperialMLFinalProject/blob/main/PostTuningResults.png?raw=true)

A summary of your results and what you can learn from your model 

You can include images of plots using the code below:
![Screenshot](image.png)

## (OPTIONAL: CONTACT DETAILS)
If you are planning on making your github repo public you may wish to include some contact information such as a link to your twitter or an email address. 

