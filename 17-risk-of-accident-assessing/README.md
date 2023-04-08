# Assessing a risk of road accident 

## Data

Data is stored in a database with the following tables of interest:

### Table `Collisions`

- `CASE_ID` — accident identification number in the database;
- `COLLISION_DATE` — date of accident;
- `COLLISION_TIME` — time of accident;
- `INTERSECTION` — if the accident took place on road an intersection;
- `WEATHER_1` — weather type;
- `COLLISION_DAMAGE` — severity of the incident;
- `PRIMARY_COLL_FACTOR` — main factor of the accident;
- `ROAD_SURFACE` — road condition;
- `LIGHTING` — lighting;
- `COUNTY_CITY_LOCATION` — identifier of geographical area where the accident occurred;
- `DISTANCE` — distance from main road (m);
- `LOCATION_TYPE` — road type;
- `PARTY_COUNT` — number of participants;
- `PCF_VIOLATION_CATEGORY` — category of violation;
- `TYPE_OF_COLLISION` — type of accident;
- `MOTOR_VEHICLE_INVOLVED_WITH` — additional participants in the accident;
- `ROAD_CONDITION_1` — road condition;
- `CONTROL_CONDITION_1` — car control device.

### Table `Parties`

- `CASE_ID` — accident identification number in the database;
- `PARTY_NUMBER` — number of accident's party;
- `PARTY_TYPE` — type of accident's party;
- `AT_FAULT` — party's guilty, true or false;
- `INSURANCE_PREMIUM` — insurance amount (thousands $);
- `PARTY_DRUG_PHYSICAL` — party's physical condition;
- `PARTY_SOBRIETY` — party's sobriety;
- `CELLPHONE_IN_USE` — presence of a telephone in the car (the ability to talk on the speakerphone) (boolean type).

### Table `Vehicles`

- `ID`— number in table;
- `CASE_ID` — accident identification number in the database;
- `VEHICLE_TYPE` — car body type;
- `VEHICLE_TRANSMISSION` — gearbox type;
- `VEHICLE_AGE` — vehicle age (in years).

## Task

Create a system that could assess the risk of a road accident along the selected route; find out whether it's possible to predict an accident based on the historical data of one of the regions.

Ideas from the customer:

- Create an accident prediction model (target value is `AT_FAULT` in `parties` table);
    - For the model, select the type of culprit — only the car (`car`);
    - Select cases where the accident resulted in any damage to the vehicle, except for the type of `SCRATCH` (`scratch`);
    - For modeling, use `2012` as a limit as the most recent;
    - A prerequisite is to take into account the age factor of the car

- Based on the model, explore the main factors of the accident

- To understand whether the results of modeling and analysis of the importance of factors will help answer the questions:
    - Is it possible to create an adequate driver risk assessment system when issuing a car?
    - What other factors need to be taken into account?
    - Does the car need to be equipped with any sensors or a camera?

## Used Tools & Libraries
`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `sqlalchemy`, `lightgbm`, `catboost`
