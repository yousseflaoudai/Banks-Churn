
## MACHINE LEARNING WITH PYTHON LABS 

#### Professor: Hanna Abi Akl


#### Team: Mamadou Diallo, Duy Khanh NGUYEN, Youssef LAOUDAI

### Introduction

We are undertaking a project that aims to predict the probability of bank churn - the likelihood that customers will leave a financial institution. As it is more cost-effective for banks to retain existing customers than to acquire new ones, this project focuses on exploring effective customer retention strategies in the highly competitive banking sector. We will utilize a dataset of 10,000 customers and evaluate their behavior across 14 variables. The study's results may provide valuable insights for banks looking to implement measures to retain their customer base.

### Dataset: 
The dataset can be accessed on Kaggle at: Churn_Modelling.csv | Kaggle
Dataset Description
The dataset contains 10,000 entries and includes the following information:

•	_RowNumber_: a unique identifier for each entry

•	CustomerId: the ID of the customer, which is also a unique identifier for each entre

•	Surname: the customer's last name

•	CreditScore: the customer's credit score

•	Geography: information about the customer's location

•	Gender: the customer's gender

•	Age: the customer's age

•	Tenure: the number of years the customer has been with the bank

•	Balance: the customer's account balance

•	NumOfProducts: the number of products the customer has with the bank

•	HasCrCard: whether the customer has a credit card with the bank

•	IsActiveMember: whether the customer is an active member of the bank

•	EstimatedSalary: the estimated salary of the customer

•	Exited: whether the customer has left the bank (1) or not (0)

### Objectives

The primary goal of this project is to identify indicators of customer disengagement and predict the likelihood of customer attrition to enable banks to develop effective strategies for retaining their clients. To achieve this, the project has the following objectives:

Identify the factors that contribute to customer disengagement
Develop a predictive model that enables banks to make informed decisions to retain their customers more efficiently.
Approach:

 Our project will follow these steps to achieve the objective:

#### 1.	Data Processing and Exploratory Data Analysis:
Data Processing and EDA are crucial to examine the dataset's structure and detect any patterns. This step helps to identify trends and patterns in the data that can assist in later stages. If there are missing values or inconsistent data, data cleaning is performed to prepare the dataset. Additionally, correlation analysis is implemented to determine the relationships between variables, especially the target variable (Exited), to identify which variables are the most important for predicting customer churn.

#### 2.	Feature Engineering:
 Since the dataset is already clean and properly structured, there is no need for specific feature engineering steps. However, the K-Nearest Neighbors and Random Forest algorithms incorporate feature engineering techniques as part of their algorithms.

#### 3.	Learning Algorithms:
 Several algorithms, including Logistic Regression, K-Nearest Neighbors, and Random Forest, are applied. These algorithms are trained on the dataset to predict whether a customer would leave the bank (1) or not (0).
#### 4.	Model Evaluation:
 The performance of each algorithm is evaluated using various metrics such as accuracy, precision, recall, and F1 score. These metrics provide insights into the effectiveness of the algorithm in correctly identifying customer churn. Based on this evaluation stage, the best-performing algorithm is selected.

Finally, the naive method and cross-validation are applied to some algorithms to test their performance on a new set of data. These methods are used to increase the model's accuracy and ensure that the chosen algorithm can generalize well to new data and is not overfitting to the training dataset.


### The Results:

After applying three models, namely Logistic Regression, K-Nearest Neighbors, and Random Forest, it was found that the Random Forest and Logistic Regression algorithms provide good predictions with accuracies of 85.8% and 69.2%, respectively. On the other hand, K-Nearest Neighbors has a high accuracy of 76.4%, but the area under the ROC curve is very low at 0.519.


### Conclusion:

 In conclusion, the Random Forest algorithm provides the most convincing results among the three models. However, the logistic regression model also showed good performance. Therefore, these algorithms can effectively predict customer disengagement. Nevertheless, the number of customers who disengage from the data is low, so the models could be further improved by training them multiple times and evaluating the stability of the chosen algorithm with good performances.




