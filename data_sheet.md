# Data Source

https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset

## Motivation

### For what purpose was the dataset created?

This dataset was originally created for research into machine learning methods aimed at the case of customers' default payments in Taiwan and compares the predictive accuracy of probability of default among six data mining methods. From the perspective of risk management, the result of predictive accuracy of the estimated probability of default will be more valuable than the binary result of classification - credible or not credible clients. Because the real probability of default is unknown, this study presented the novel Sorting Smoothing Method to estimate the real probability of default. With the real probability of default as the response variable (Y), and the predictive probability of default as the independent variable (X), the simple linear regression result (Y = A + BX) shows that the forecasting model produced by artificial neural network has the highest coefficient of determination; its regression intercept (A) is close to zero, and regression coefficient (B) to one. Therefore, among the six data mining techniques, artificial neural network is the only one that can accurately estimate the real probability of default.
  
### Who created the dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)? Who funded the creation of the dataset?

* I-Cheng Yeh - Department of Information Management, Chung-Hua University, Hsin Chu 30067, Taiwan, ROC

* Che-hui Lien - Department of Management, Thompson Rivers University, Kamloops, BC, Canada

## Composition

- What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)?
<br>Each record instance represent a client record, some demographic details, account balance, repayment history and statement amount
- How many instances of each type are there?
<br> the dataset is not separated into distinct groups or different types. It is believed to represent a population of credit card customers that have either defaulted payments or not
- Is there any missing data?
<br>No
- Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by    doctor–patient confidentiality, data that includes the content of individuals’ non-public communications)?
<br>No PII or SPII included in the data

## Collection process

- How was the data acquired?
<br>The dataset was based on a study in Taiwan which took payment data in October, 2005, from an important bank (a cash and credit card issuer) and the targets were credit card holders of the bank. Among the total 25,000 observations, 5529 observations (22.12%) are the cardholders with default payment. This research employed a binary variable – default payment (Yes = 1, No = 0), as the response variable
- If the data is a sample of a larger subset, what was the sampling strategy?
<br>The entire 25,000 observations were used
- Over what time frame was the data collected?
<br> October 2005

## Preprocessing/cleaning/labelling

- Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? If so, please provide a description. If not, you may skip the remaining questions in this section.
<br>A series of preprocessing steps were performed on the data prior to model training and testing including:
* Splitting of dataset into 70/30 train / test
* Removal of features due to missing values, correlation or information value exceed threhold
- Was the “raw” data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)?
* No
 
## Uses

- What other tasks could the dataset be used for?
* How does the probability of default payment vary by categories of different demographic variables?
* Which variables are the strongest predictors of default payment?
- Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? For example, is there anything that a dataset consumer might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other risks or harms (e.g., legal risks, financial harms)? If so, please provide a description. Is there anything a dataset consumer could do to mitigate these risks or harms?
* Being awrare of the payment conditions and penalties agreements the bank used, as well as any abnormal economic or soietal situations in Taiwan at the time of collection
- Are there tasks for which the dataset should not be used? If so, please provide a description.
* Non banking use cases

## Distribution

- How has the dataset already been distributed?
* The data is published Via 
- Is it subject to any copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)?  

## Maintenance

- Who maintains the dataset?

