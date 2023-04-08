# Determining age of buyers by their photos

## Data

Data taken from the [ChaLearn Looking at People](http://chalearnlap.cvc.uab.es/dataset/26/description/) website: folder with images and a CSV file `labels.csv` with the following two columns:

- `file_name` — name of the while with person's photo;
- `real_age` — age of person (target variable).

## Task

Build a model that will determine the approximate age of a person from a photograph by using a labeled dataset of people photographs.

In particular, it is needed to:

- perform an EDA of provided photographs dataset;
- prepare data for training;
- train the NN model and estimate its quality;
- resulting value of the `MAE` metric should not be higher than `8`.

## Used Tools & Libraries
`pandas`, `matplotlib`, `seaborn`, `keras`
