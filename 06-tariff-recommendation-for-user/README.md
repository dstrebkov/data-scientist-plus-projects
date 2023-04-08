# Mobile tariff recommendation for a client

## Data

Dataset contains data on the behavior of clients who have already switched to _"Smart"_ and _"Ultra"_ tariffs. Columns in the dataset are the following:

- `сalls` — calls count;
- `minutes` — total duration of calls in minutes;
- `messages` — number of SMS messages;
- `mb_used` — consumed internet traffic in Mb;
- `is_ultra` — tariff used by a client during the month («Ultra» — `1`, «Smart» — `0`).

## Task

Based on the [past study](https://github.com/dstrebkov/data-scientist-plus-projects/tree/main/05-finding-promising-telecom-tariff) made to determine the prospective tariff for a telecom company, it is necessary to build a machine learning model to recommend a tariff to clients based on their customer behavior.

Required to select a model with the highest possible accuracy value, bringing the proportion of correct answers to at least `0.75`.

## Used Tools & Libraries
`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`
