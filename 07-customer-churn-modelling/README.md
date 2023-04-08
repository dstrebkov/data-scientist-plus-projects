# Customer churn modelling

## Data

Columns in the dataset:

- `RowNumber` — row index in dataset;
- `CustomerId` — client unique ID;
- `Surname` — client surname;
- `CreditScore` — credit rating;
- `Geography` — country of residence;
- `Gender` — gender;
- `Age` — age;
- `Tenure` — how many years a person has been a bank customer;
- `Balance` — account balance;
- `NumOfProducts` — number of bank products used by the client;
- `HasCrCard` — whether the client has credit card or not;
- `IsActiveMember` — client activity;
- `EstimatedSalary` — estimated salary;
- `Exited` — whether client has cancelled his banking contract or not.

## Task

Having provided historical data on customer behavior and termination of agreements with the bank, predict whether the client will stop being a client (i.e. will leave the bank) in the nearest future or not.

It is necessary to build a model with the largest value of the `F1`-measure that is possible: the metric is expected to be greater than `0.59`.

Additionally, needed to measure the `AUC-ROC` and compare its value with the `F1`-measure.

## Used Tools & Libraries

`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`
