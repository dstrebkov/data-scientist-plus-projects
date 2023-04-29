# Contract termination prediction

## Data

The data is stored in a PostgreSQL database. It consists of several tables:

- `contract` — information about contracts;
- `personal` — personal data of clients;
- `internet` — information about Internet services;
- `phone` — information about telephony services.

__________________

Table `contract` stores the following data:

- `customerID` — subscriber ID;
- `BeginDate` — start date of the contract;
- `EndDate` — contract end date;
- `Type` — type of payment: once a year or two or monthly;
- `PaperlessBilling` — electronic payslip;
- `PaymentMethod` — payment type;
- `MonthlyCharges` — expenses per month;
- `TotalCharges` — subscriber's total expenses.

Table `personal` stores the following data:

- `customerID` — user ID;
- `gender` — gender;
- `SeniorCitizen` — whether the subscriber is a pensioner;
- `Partner` — whether the subscriber has a spouse;
- `Dependents` — whether the subscriber has children.

Table `internet` stores the following data:

- `customerID` — user ID;
- `InternetService` — connection type;
- `OnlineSecurity` — blocking dangerous sites;
- `OnlineBackup` — cloud file storage for data backup;
- `DeviceProtection` — antivirus;
- `TechSupport` — dedicated technical support line;
- `StreamingTV` — streaming television;
- `StreamingMovies` — a catalog of movies.

Table `phone` stores the following data:

- `customerID` — user ID;
- `MultipleLines` — connect the phone to several lines at the same time.

## Task

Some telecom operator wants to deal with the outflow of customers. To do this, its employees will begin to offer promotional codes and special conditions to everyone who plans to refuse communication services. In order to find such users in advance, the operator needs a model that will predict whether the subscriber will terminate the contract. The operator's team collected personal data about some customers, information about their tariffs and services. So, the task is to train a model for predicting customer churn on this data.

The ROC-AUC metric value must be at least `0.85`. For model interpretability, additionally display the accuracy value.

## Used Tools & Libraries
`SQL`, `pandas`, `numpy`, `matplotlib`, `seaborn`, `sqlalchemy`, `sklearn`
