## Project description

This Project is done on behalf Sweet Lift Taxi company to attract more drivers during peak hours. The company has collected historical data on taxi orders at airports. The goal of the project is to create a model that predicts the amount of taxi orders for the next hour with an RMSE of not more than 48 on our test set.


## Description of the data

- `num_orders` - Number of orders
- `datetime` - Date of ride


## **Project Insight**

The mean `num_orders` shows an upward trend in the last 5 months between 2018-03-01 and 2018-08-31.
The data was prepared by creating several date and time-series related features, such as, `month`, `day`, `dayofweek`, `hour`, 
`lag_*`, `roll_mean` and `roll_std`.
We analyzed the Time series data and saw that the peak day for taxi trips was Thursdays, 30th, and the peak hours were between 6am and 3pm
CatBoostRegressor emerged as the best model with the lowest RMSE. However, it also took the longest to train the model.
