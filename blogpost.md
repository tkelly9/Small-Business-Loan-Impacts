## Regression Models

#### Univariate Linear Regression Model

Linear Regression model and correlation matrix show that the number of full-time employees at the time of the loan closure is positively correlated with the number of jobs retained as a direct result of the loan. The target variable for the regression models is represented by the Job Benefit variable, which is the sum of Jobs Created and Jobs Retained as a result of the loan. The Job Benefit Variable represents the overall economic impact of the loan.

#### Correlation Matrix with Variables Used in Regression Models
 <img width="386" alt="Screen Shot 2022-05-14 at 7 29 16 PM" src="https://user-images.githubusercontent.com/74617235/168451276-3b1641a1-b1ce-41d1-a9cd-7d5e8504ab5c.png">
 

#### Univariate Linear Regression model shows that the number of full-time employees at the time of the loan closure accounts for about 60% of the variation in the job benefit resulting from the loan.

<img width="554" alt="Screen Shot 2022-05-14 at 8 09 19 PM" src="https://user-images.githubusercontent.com/74617235/168452062-eea63e15-7a4b-4f27-b18f-b151237978c2.png">


R<sup>2</sup> Value: 0.603

#### Multivariate Linear Regression Model

Multivariate linear regression model results indicate that Full Time Employees, Metro Type, Community Development Financial Institutions (CDFI) Type, and SPY Stock Close price are the strongest predictors for the number of Jobs Created and Jobs Retained. 

<img width="794" alt="Screen Shot 2022-05-14 at 9 52 48 PM" src="https://user-images.githubusercontent.com/74617235/168453868-90be54ca-1630-4d74-a863-2b3f5b4a28b1.png">

R<sup>2</sup> Value: 0.647

## Classification Models

### Classifications models that were used to predict whether jobs were created as a direct result of the SSBCI loans: 
* Logistic Regression 
* Support Vector Classifier
* Gradient Boosting Classifier 


#### Model Metrics
<img width="793" alt="Screen Shot 2022-05-14 at 10 06 54 PM" src="https://user-images.githubusercontent.com/74617235/168454214-a7479326-f2bc-415f-90e8-e4c5d48c65cc.png">

Accuracy, Precision, Recall, and F1 score were used to determine which model had the best predictive performance. Based on the metrics listed, we selected the Gradient Boosting Classifier as the model to use when predicting whether jobs were created as a direct result of the loans.

#### ROC Curves
<img width="330" alt="Screen Shot 2022-05-15 at 11 05 26 AM" src="https://user-images.githubusercontent.com/74617235/168479772-303d6d65-99a0-403c-b372-779dbed8e75f.png"> <img width="330" alt="Screen Shot 2022-05-15 at 11 08 27 AM" src="https://user-images.githubusercontent.com/74617235/168479843-2c884418-49b8-4ab2-9aec-e6a114aa4b17.png"> <img width="330" alt="Screen Shot 2022-05-15 at 11 09 45 AM" src="https://user-images.githubusercontent.com/74617235/168479921-56e3d0ff-5ea5-4376-b942-905692f36a7c.png">




#### Shapley values were used for feature selection for the Gradient Boosting Classifier. Below are the Shapley values:
<img width="541" alt="Screen Shot 2022-05-14 at 10 12 07 PM" src="https://user-images.githubusercontent.com/74617235/168454328-ed63857d-de56-47d0-8e2a-85c53c5e41f5.png">


* Feature 0: SSBCI Original Funds
* Feature 1: Revenue
* Feature 2: Full Time Employees
* Feature 3: Jobs Retained
* Feature 4: Loan Investment Amount
* Feature 5: SPY Close Price

The plot indicates that Loan Investment Amount had the highest impact on whether jobs were created as a result of the loan.
