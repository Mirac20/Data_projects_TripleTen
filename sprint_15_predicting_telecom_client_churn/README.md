## Project description

The telecom operator Interconnect would like to be able to forecast their churn of clients. If it's discovered that a user is planning to leave, they will be offered promotional codes and special plan options. Interconnect's marketing team has collected some of their clientele's personal data, including information about their plans and contracts.



## Description of the data

- `customerID` - Unique ID
- `gender` - Gender
- `SeniorCitizen` - Whether senior citizen or not
- `Partner` - Has partner or not
- `Dependents` - Number of dependents
- `BeginDate` - Joining date
- `EndDate` - Ending date
- `Type` - Plan type
- `PaperlessBilling` - Type of paperpless billing
- `PaymentMethod` - Payment method
- `MonthlyCharges` - Monthly charges
- `TotalCharges` - Total charges
- `MultipleLines` - Whether has multiple lines
- `InternetService` - Whether has internet service
- `OnlineSecurity` - Whether has online security
- `OnlineBackup` - Whether has online backup
- `DeviceProtection` - Whether has device protection
- `TechSupport` - Whether has tech support
- `StreamingTV` - Whether has streaming TV
- `StreamingMovies` - Whether has streaming movies
- `is_churned` - Whether churned
- `num_days` - Number of days in the system
- `year` - Year
- `num_services` - Number of services availed


## General Conclusion

Within the scope of this project, I created several predictive models using gradient boosting models, such as Light Gradient Boosting classifier model, CatBoost model, LightGBM Gradient Boosted DART Classifier, Decision Tree classifier, Random Forest classfier. The Logistic Regression model was used as our baseline model. It had a ROC-AUC score of 0.747 on the Test Set.
To improve the score of our models we did the following:
Performed Ordinal Encoding on the categorical features, and amended the class imbablance by adjusting the weights
after performing these steps above, the best score (0.82) on the training set belonged to the CatBoost model. We tested it on the test set and got an AUC-ROC score of 0.76.

