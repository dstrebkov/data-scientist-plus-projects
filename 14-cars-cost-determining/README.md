# Cars cost determining

## Data

Dataset is represented by the following features:

- `DateCrawled` — date of downloading the car info from the database;
- `VehicleType` — car body type;
- `RegistrationYear` — year of car registration;
- `Gearbox` — gearbox type;
- `Power` — horse power;
- `Model` — car model;
- `Kilometer` — mileage (km);
- `RegistrationMonth` — month of car registration;
- `FuelType` — fuel type;
- `Brand` — car brand;
- `NotRepaired` — was the car under repair or not;
- `DateCreated` — car info creation date;
- `NumberOfPictures` — number of car photos;
- `PostalCode` — postal code of the owner of the profile (user);
- `LastSeen` — date of last user activity;
- `Price` — car price (target feature).

## Task

Build a machine learning model to determine the cost of used cars. The customer considers important:

- prediction quality;
- prediction speed;
- model learning time.

## Used Tools & Libraries
`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `catboost`, `lightgbm`
