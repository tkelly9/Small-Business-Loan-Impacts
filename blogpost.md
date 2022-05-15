## Regression Models

#### Univariate Linear Regression Model

Linear Regression model and correlation matrix show that the number of full-time employees at the time of the loan closure is positively correlated with the number of jobs retained as a direct result of the loan.

#### Correlation Matrix with Variables Used in Regression Models
 <img width="386" alt="Screen Shot 2022-05-14 at 7 29 16 PM" src="https://user-images.githubusercontent.com/74617235/168451276-3b1641a1-b1ce-41d1-a9cd-7d5e8504ab5c.png">
 

#### Univariate Linear Regression model shows that the number of full-time employees at the time of the loan closure is positively correlated with the sum of jobs retained and created as a direct result of the loan.

<img width="554" alt="Screen Shot 2022-05-14 at 8 09 19 PM" src="https://user-images.githubusercontent.com/74617235/168452062-eea63e15-7a4b-4f27-b18f-b151237978c2.png">


R<sup>2</sup> Value: 0.603

#### Multivariate Linear Regression Model

Multivariate linear regression model results indicate that SSBCI Original Funds, Concurrent Private Financing, Guaranteed Amount, Full Time Employees, and Jobs Created are the strongest predictors for the number of Jobs Retained. 


![Screen Shot 2022-05-10 at 4 17 36 PM (2)](https://user-images.githubusercontent.com/74617235/167714904-865bbd48-c168-4e5d-851f-e99e13841f17.png)

R<sup>2</sup> Value: 0.637

## Classification Models

### Classifications models that were used to predict whether jobs were created as a direct result of the SSBCI loans: 
* Logistic Regression 
* Support Vector Classifier
* Gradient Boosting Classifier 

### Model Metrics

![Screen Shot 2022-05-10 at 4 20 31 PM (2)](https://user-images.githubusercontent.com/74617235/167715962-8da1a602-7f61-4b3b-bbfb-d760e8d4f809.png)

Accuracy, Precision, Recall, and F1 score were used to determine which model had the best predictive performance. Based on the metrics listed, we selected the Gradient Boosting Classifier as the model to use when predicting whether jobs were created as a direct result of the loans.


### Shapley values were used for feature selection for the Gradient Boosting Classifier. Below are the Shapley values:
![image](https://user-images.githubusercontent.com/74617235/167889123-769deb7d-9044-4ed9-b9ae-59bdb14e5f93.png)

* Feature 0: Loan Investment Amount
* Feature 1: Revenue
* Feature 2: Full Time Employees
* Feature 3: SSBCI Original Funds
* Feature 4: Jobs Retained
* Feature 5: Concurrent Private Financing
