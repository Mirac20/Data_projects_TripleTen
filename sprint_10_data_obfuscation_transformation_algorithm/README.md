## Project description

This project is done for Sure Tomorrow Insurance company, my task is to used Machine Learning to :

- find customers that are similar to other customers to help the company's marketing department in placing targeted ads.
- predict whether a new customer is likely to receive an insurance benefit.
- predict the number of insurance benefits a new customer is likely to receive.
- protect clients' personal data by developing a data transformation algorithm without breaking the model

## Description of the data

- `gender` - Gender
- `age` - Age of insured
- `salary` - Salary of insured
- `number of family members` - Number of dependents

## **Project Insight**

To predict whether a new customer is likely to receive an insurance benefit. We had to compare the performance of our model with a dummy model and see if it does better. We built a KNN-based classifier and measured its quality with the F1 metric for k = 1 - 10 for both the original data and the scaled one. The F1 score was significantly higher on the scaled dataset, and Nearest Neighbor K = 1 performed best. Therefore KNN is quite good for this task. Also, we found out that the random model performs worse than the actual KNN model.

A Linear Regression model was used to predict the number of insurance benefits a new customer is likely to receive. The RMSE for both the original data and the scaled data are the same. They both had RMSE values of 0.34. This indicates that scaling the data does not have any effect on predicting targets using a Linear Regression model.

Lastly, to obfuscate data, we multiply the numerical features by an invertible matrix P Also, to compute the weights in linear regression, we multiply the original weight with P inverse.


