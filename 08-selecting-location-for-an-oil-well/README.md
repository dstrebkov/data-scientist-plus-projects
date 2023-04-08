# Choosing a location for an oil well

## Data

Dataset consists of oil samples information from three geographic regions: in each of `10,000` fields, where the quality of oil was measured together with the volume of oil reserves. Columns in the dataset are the following:

- `id` — unique oil well ID;
- `f0`, `f1`, `f2` — three features of the fields;
- `product` — volume of oil reserves in the well (in thousands of barrels).

## Task

The company needs to decide where to drill a new oil well.

It is necessary to build a ML model that will help determine the region where oil mining will bring the greatest profit. Also an analysis should be performed to estimate possible profit and risks using _Bootstrap_.

## Used Tools & Libraries

`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `bootstrap`
