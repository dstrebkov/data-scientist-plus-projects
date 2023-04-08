# Analysis of advertisements for the sale of apartments


## Data

Data table consists of the following columns:

- `airports_nearest` — distance to the nearest airport in meters (m);
- `balcony` — number of balconies;
- `ceiling_height` — ceiling height (m);
- `cityCenters_nearest` — distance to city center (m);
- `days_exposition` — how many days the ad was posted (from publication to removal);
- `first_day_exposition` — publication date;
- `floor` — floor;
- `floors_total` — total floors;
- `is_apartment` — is apartment or not (boolean type);
- `kitchen_area` — kitchen area in square meters (m²);
- `last_price` — price at the time of removal from publication;
- `living_area` — living area in square meters (m²);
- `locality_name` — locality name;
- `open_plan` — is free layout or not (boolean type);
- `parks_around3000` — number of parks within a `3` km radius;
- `parks_nearest` — distance to nearest park (m);
- `ponds_around3000` — number of water bodies within a `3` km radius; 
- `ponds_nearest` — distance to the nearest body of water (m);
- `rooms` — number of rooms;
- `studio` — is studio-apartment or not (boolean type);
- `total_area` — area of ​​the apartment in square meters (m²);
- `total_images` — number of photos of the apartment in the ad.

## Task

Task is based on data containing information on the sale of apartments in Saint-Petersburg and neighboring settlements for several years. It is necessary to determine the market value of real estate and set parameters, as well as it is necessary to analyze the data and draw conclusions on a number of indicators. This will help create an automated system that will track anomalies and fraudulent activity. Some of these data were entered by users, and some were obtained automatically on the basis of cartographic data.

## Used Tools & Libraries
`pandas`, `matplotlib`
