# Home Credit Default Risk
## *Can you predict how capable each applicant is of repaying a loan?*

![Image description](hc_logo.png) <br />

## Task 
Home Credit is an Internation non-banking financial institution headquartered in Netherlands. It strives to broaden the financial inclusion to offer safe and comfortable borrwing experience. The company mainly focuses on client with little to no credit history. Proving loan to people with hardly any credit history comes with a lot of risks - mainly the defaulting of the loans! 

In a kaggle competition, Home Credit provided transactional information, annual income, family status, housing type, etc. in order to predict their clients' repayment abilities. So this project is a supervised binary classification task with 'Default' as our target. 

## Evaluation 

The model was evaluated using the Area Under the Receiver Operating Characteristic curve (AU-ROC or AUC).


## Approach

Datasource: https://www.kaggle.com/c/home-credit-default-risk/data
Data visualization: Tableau 
Exploratory analysis and model building: Python, PySpark on the Databricks platform 

Models Built: 
1) Logistic Regression with SMOTE Resampling--> AUROC 0.63
2) Random Forest --> AU-ROC 0.65
3) Catboost --> AU-ROC 0.69 

## Results 
