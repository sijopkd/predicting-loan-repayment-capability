# Home Credit Default Risk
## *Can you predict how capable each applicant is of repaying a loan?*

![Image description](hc_logo.png) <br />

## Task 
Home Credit is an Internation non-banking financial institution headquartered in Netherlands. It strives to broaden the financial inclusion to offer safe and comfortable borrwing experience. The company mainly focuses on client with little to no credit history. Proving loan to people with hardly any credit history comes with a lot of risks - mainly the defaulting of the loans! 

In a kaggle competition, Home Credit provided transactional information, annual income, family status, housing type, etc. in order to predict their clients' repayment abilities. So this project is a supervised binary classification task with 'Default' as our target. 

## Evaluation 

The model was evaluated using the Area Under the Receiver Operating Characteristic curve (AU-ROC or AUC).


## Approach

Datasource: https://www.kaggle.com/c/home-credit-default-risk/data <br />
Data visualization: Tableau  <br /> 
Exploratory analysis and model building: Python, PySpark on the Databricks platform <br />

Models Built: 
1) Logistic Regression with SMOTE Resampling--> AUROC 0.63
2) Random Forest --> AU-ROC 0.65
3) Catboost --> AU-ROC 0.69 

## Results 

Even though Catboost model slightly outperformed the other algorithms, the final model picked was Logisitic Regression for the following reasons:

1) Interpretability
2) Ability to modify the posterior probability to reduce False Negatives 
Note: As a financial institution, it is essential to reduce the False Negatives (clients who tend to default the loan, but the model does not predict that they will), since the loss associated with such cases are very high. 
3) Reduced training time
4) Easy to productionize 

## Conclusion

1) The model can be further improved by feature engineering a lot of variables. Due to the limitations in the time, only a few variables were transformed 
2) More boosting alogorithms such as XGBoost and Adaboost could be trained (Could not perform on Databricks platform due to limitations in the community edition) 



