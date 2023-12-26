## Project description

Rusty Bargain used car sales service want to develop an app to attract new customers. In that app, clients can quickly find out the market value of a car that they are interested in purchasing. Rusty bargain have given us access to historical data: technical specifications, trim versions, and prices. Our goal is to build to build a model that determines the value of each car.

Rusty Bargain is interested in:
- the quality of the prediction
- the speed of the prediction
- the time required for training



## Description of the data

- `DateCrawled` — date profile was downloaded from the database
- `VehicleType` — vehicle body type
- `RegistrationYear` — vehicle registration year
- `Gearbox` — gearbox type
- `Power` — power (hp)
- `Model` — vehicle model
- `Mileage` — mileage (measured in km due to dataset's regional specifics)
- `RegistrationMonth` — vehicle registration month
- `FuelType` — fuel type
- `Brand` — vehicle brand
- `NotRepaired` — vehicle repaired or not
- `DateCreated` — date of profile creation
- `NumberOfPictures` — number of vehicle pictures
- `PostalCode` — postal code of profile owner (user)
- `LastSeen` — date of the last activity of the user
- `Price` — price (Euro)

## **Project Insight**

Several models were built to determine the value of the cars. Linear Regression has the best training time (90.9 ms) while the worst is Random Forest (40700 ms). Also, Linear Regression has the best prediction time of 5.96 ms while the Random Forest Model has the worst, 886 ms.

Random Forest has the best RMSE of 1457. However, the time taken for training and prediction is highest. The CatBoost model takes about half the time of the Random Forest model for training, and about four times less than the Random Forest Model for making predictions. Moreover, the RMSE of the CatBoost Model is 1489. Therefore, we will recommend with the CatBoost model.
