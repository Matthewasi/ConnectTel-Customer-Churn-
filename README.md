# ConnectTel-Customer-Churn-
About the dataset
It includes information about:
•CustomerID: A unique identifier assigned to each telecom customer, enabling tracking and identification of individual customers.
•Gender: The gender of the customer, which can be categorized as male or female. This information helps in analyzing gender-based trends in customer churn.
•SeniorCitizen: A binary indicator that identifies whether the customer is a senior citizen or not. This attribute helps in understanding if there are any specific churn patterns among senior customers.
•Partner: Indicates whether the customer has a partner or not. This attribute helps in evaluating the impact of having a partner on churn behavior.
•Dependents: Indicates whether the customer has dependents or not. This attribute helps in assessing the influence of having dependents on customer churn.
•Tenure: The duration for which the customer has been subscribed to the telecom service. It represents the loyalty or longevity of the customer’s relationship with the company and is a significant predictor of churn.
•PhoneService: Indicates whether the customer has a phone service or not. This attribute helps in understanding the impact of phone service on churn.
•MultipleLines: Indicates whether the customer has multiple lines or not. This attribute helps in analyzing the effect of having multiple lines on customer churn.
•InternetService: Indicates the type of internet service subscribed by the customer, such as DSL, fiber optic, or no internet service. It helps in evaluating the relationship between internet service and churn.
•OnlineSecurity: Indicates whether the customer has online security services or not. This attribute helps in analyzing the impact of online security on customer churn.
•OnlineBackup: Indicates whether the customer has online backup services or not. This attribute helps in evaluating the impact of online backup on churn behavior.
•DeviceProtection: Indicates whether the customer has device protection services or not. This attribute helps in understanding the influence of device protection on churn.
•TechSupport: Indicates whether the customer has technical support services or not. This attribute helps in assessing the impact of tech support on churn behavior.
•StreamingTV: Indicates whether the customer has streaming TV services or not. This attribute helps in evaluating the impact of streaming TV on customer churn.
•StreamingMovies: Indicates whether the customer has streaming movie services or not. This attribute helps in understanding the influence of streaming movies on churn behavior.
•Contract: Indicates the type of contract the customer has, such as a month-to-month, one-year, or two-year contract. It is a crucial factor in predicting churn as different contract lengths may have varying impacts on customer loyalty.
•PaperlessBilling: Indicates whether the customer has opted for paperless billing or not. This attribute helps in analyzing the effect of paperless billing on customer churn.
•PaymentMethod: Indicates the method of payment used by the customer, such as electronic checks, mailed checks, bank transfers, or credit cards. This attribute helps in evaluating the impact of payment methods on churn.
•MonthlyCharges: The amount charged to the customer on a monthly basis. It helps in understanding the relationship between monthly charges and churn behavior.
•TotalCharges: The total amount charged to the customer over the entire tenure. It represents the cumulative revenue generated from the customer and may have an impact on churn.
•Churn: The target variable indicates whether the customer has churned (canceled the service) or not. It is the main variable to predict in telecom customer churn analysis. 




1. Problem Definition
The goal of this project is to predict customer churn of ConnectTel by analyzing historical customer data. By accurately predicting which customers are likely to leave, the company can take targeted actions to retain them, ultimately reducing churn rates and increasing revenue, ConnectTel will benefit by implementing strategies to retain high-value customers, reducing churn rate, optimizing marketing strategies, and improving customer satisfaction to maintain a competitive edge in the industry. 

2. Exploratory Data Analysis (EDA) in Python
At this stage it important to import all necessary libraries:
import pandas as pd 
import seaborn as sns 
import matplotlib.pyplot as plt 
import numpy as np

3. Feature Engineering
a) Encoding Categorical Variables
b) Creating New Features

4. Model Selection, Training, and Validation
a) Train and Test at least 3 supervised learning models 
Trained and tested about 7 machine learning models including KNeigbours, RandomForest, LogisticRegression, DecisionTreen, SVC, XGB and Naive Bayes.
from sklearn.linear_model import SGDClassifier
from sklearn.neighbors import KNeighborsClassifier
from sklearn.ensemble import RandomForestClassifier
from sklearn.linear_model import LogisticRegression
from sklearn.svm import LinearSVC, SVC
from sklearn.naive_bayes import GaussianNB
from sklearn.svm import SVC
from sklearn.tree import DecisionTreeClassifier
from xgboost import XGBClassifier

5. Model Evaluation using:
accuracy score, precision score, recall score, f1_score, roc_auc_score
from sklearn.metrics import confusion matrix
If the ConnectTel wants to ensure that it catches as many potential churners as possible (to minimize customer loss), it should aim for higher recall, even if it means some non-churners are wrongly identified. Naive Bayes 72.92% secondly with 50.94% with 50.94% and last but not the least is DecisionTree with 50.67%. With these metrics provided the ConnectTel should focus on the false negatives to prevent customers from deactivating the services.   
Most customer retention scenarios prioritize decreasing false negatives (identifying all prospective churners), as each missed churn might result in a direct loss of Revenue.


