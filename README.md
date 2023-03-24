# Banks-Churn

For a bank it is more expensive to  attract new customers than to convince old ones to stay. Therefore, it is better to implement effective strategies to retain their customers in this very competitive sector. The objective of this project is to predict the churn risk of a bank so that it can implement measures to retain them. The data comes from https://www.kaggle.com/aakash50897/churn-modellingcsv. The study is based on the data of 10,000 customers of a bank evaluated on 14 variables.



## The package

### Ignore the warnings
from warnings import simplefilter

simplefilter(action='ignore', category=FutureWarning)


### Data Processing
import pandas as pd


#### Tables, Matrices, Maths
import numpy as np

### Visualisation
import matplotlib.pyplot as plt

%matplotlib inline

import seaborn as sns

sns.set(style="white")

### Building models

from sklearn.model_selection import train_test_split, GridSearchCV, cross_val_score
from sklearn.feature_selection import RFE
from sklearn.metrics import accuracy_score, recall_score, precision_score, confusion_matrix, f1_score, roc_curve, auc


### Models
from sklearn.linear_model import LogisticRegression
from sklearn.neighbors import KNeighborsClassifier
from sklearn.ensemble import RandomForestClassifier

## Framework

In order to identify signs of customer disengagement, it is important to have a first empirical approach of the customer's practices. To do this, we acquire a set of data describing the customer's activities and profile. Thus our objectives are the following:
 
* Determine the risk of customer disengagement
* Choose an efficient model that will allow banks to make decisions in order to retain their customers
## Data processing and description

### Data Description
customers = pd.read_csv("C:/Users/Kennick/Documents/Python/ML_Project/Churn_Modelling.csv")

customers.head(10)

The context of this study remains rather general as the data's interpretation leaves us confused. For example, a customer who has left a bank still has a remaining positive balance.

We observe 10,000 individuals described by 14 variables.

customers.shape

customers.columns

### Missing Values

customers.isnull().sum()/len(customers)
