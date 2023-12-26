## Project description

The data is stored in three files:

- gold_recovery_train.csv — training dataset download
- gold_recovery_test.csv — test dataset download
- gold_recovery_full.csv — source dataset download

Data is indexed with the date and time of acquisition (date feature). Parameters that are next to each other in terms of time are often similar.
Some parameters are not available because they were measured and/or calculated much later. That's why, some of the features that are present in the training set may be absent from the test set. The test set also doesn't contain targets.
The source dataset contains the training and test sets with all the features.
You have the raw data that was only downloaded from the warehouse. Before building the model, check the correctness of the data. For that, use our instructions.

## Description of the data

- `rougher.output.recovery`  - Output of the rougher
- `rougher.output.tail_ag`   - Concentration of Silver
- `rougher.output.tail_sol`  - Concentration of solution
- `rougher.output.tail_au`   - Concentration of Gold
- `rougher.input.floatbank11_xanthate` - Floatation bank input
- `secondary_cleaner.output.tail_sol`  - Secondary stage cleaner concentrate
- `final.output.recovery`  - Final output
- `rougher.calculation.au_pb_ratio`  - Gold to Lead ratio
- `primary_cleaner.input.sulfate`   - Concentrate of sulphate
- `primary_cleaner.input.depressant` - Concentrate of depressant


# **Project Insight**

In this project, my task is to design a predictive model that is capable of estimating the quantity of gold extractable from gold ore. The data related to both the extraction and purification processes of gold ore were provided as invaluable resources for training the model. The ultimate expectation of this model is to facilitate a more efficient production process.

After creating the model, and conducting  indepth exploratory analysis, these are the summary of the project:

In this project, I developed a model to forecast the amount of gold that can be extracted, based on the available features. Finally, I created three distinct models using Linear Regression, and Random Forest. A comprehensive examination of these two models revealed that the Random Forest model outperformed the Linear Regression model. When employing hyperparameters such as max_depth = 5, n_estimators = 20, and cv = 5, the model yielded an 7.97 sMAPE value on the test dataset.

