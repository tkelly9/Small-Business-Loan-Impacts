## Regression Models

#### Univariate Linear Regression Models

Linear Regression model and correlation matrix show that the number of full-time employees at the time of the loan closure is positively correlated with the number of jobs retained as a direct result of the loan.

<img width="546" alt="Screen Shot 2022-05-10 at 5 03 26 PM" src="https://user-images.githubusercontent.com/74617235/167721564-22424222-574f-4656-bf64-0421a5d72a61.png"> 

![Screen Shot 2022-05-10 at 3 40 03 PM (2)](https://user-images.githubusercontent.com/74617235/167709636-9e276e56-a06f-4cfa-8712-445de3a5b74d.png)


R<sup>2</sup> Value: 0.597

#### Multivariate Linear Regression Model

Multivariate linear regression model results indicate that SSBCI Original Funds, Concurrent Private Financing, Guaranteed Amount, Full Time Employees, and Jobs Created are the strongest predictors for the number of Jobs Retained. 


![Screen Shot 2022-05-10 at 4 17 36 PM (2)](https://user-images.githubusercontent.com/74617235/167714904-865bbd48-c168-4e5d-851f-e99e13841f17.png)

R<sup>2</sup> Value: 0.637

## Classification Models

### Classifications models that were used to predict whether jobs were created as a direct result of the SSBCI loans: 
* Logistic Regression 
* Support Vector Classifier
* Gradient Boosting Classifier 

### Shapley values were used for feature selection. Below are the Shapley values:
![image](https://user-images.githubusercontent.com/74617235/167889123-769deb7d-9044-4ed9-b9ae-59bdb14e5f93.png)

* Feature 0: Loan Investment Amount
* Feature 1: Revenue
* Feature 2: Full Time Employees
* Feature 3: SSBCI Original Funds
* Feature 4: Jobs Retained
* Feature 5: Concurrent Private Financing

### Model Metrics

![Screen Shot 2022-05-10 at 4 20 31 PM (2)](https://user-images.githubusercontent.com/74617235/167715962-8da1a602-7f61-4b3b-bbfb-d760e8d4f809.png)

Accuracy, Precision, Recall, and F1 score were used to determine which model had the best predictive performance. Based on the metrics listed, we selected the Gradient Boosting Classifier as the model to use when predicting whether jobs were created as a direct result of the loans.
