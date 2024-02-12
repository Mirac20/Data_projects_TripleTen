## Project description

This project is done for the mobile carrier, Megaline. They found out that many of their subscribers use legacy plans. They want to develop a model that would analyze subscribers' behavior and recommend one of Megaline's newer plans: Smart or Ultra.
Data is given from the mobile carrier about subscribers who have already switched to the new plans. For this classification task, we would be developing a model that will pick the right plan. 
We would be developing a model with the highest possible accuracy. The threshold for accuracy is 0.75. We check the accuracy using the test dataset.


## Description of the data

Every observation in the dataset contains monthly behavior information about one user. The information given is as follows:
- `сalls` — number of calls,
- `minutes` — total call duration in minutes,
- `messages` — number of text messages,
- `mb_used` — Internet traffic used in MB,
- `is_ultra` — plan for the current month (Ultra - 1, Smart - 0).

  ## General Conclusion

- Three models - DecisionTreeClassifier, LogisticRegression, and RandomForestClassifier were built and tested with 10 different hyperparameters that are specific to the respecitive models. RandomForestClassifier performed best with an accuracy of ~81%.
- The results on the test set deteriorated slightly due to overfitting, and we obtained a test set accuracy of ~79%.
- Asuming the model picks the Smart plan user all the time, this will occur with a 69% probablity. Our model out performs the baseline model, which confirms that it is working correctly.

