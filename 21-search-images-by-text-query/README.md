# Search images by text query

## Data

The `train_dataset.csv` file contains the information needed for training:

- image file name;
- description ID;
- description text

Up to `5` descriptions can be available for one picture. The description ID has the format `<image file name>#<description serial number>`.
The `train_images` folder contains images for training the model.

In the `CrowdAnnotations.tsv` file, data on matching images and descriptions obtained using crowdsourcing. Column numbers and corresponding data type:

- The name of the image file;
- Description ID;
- Percentage of people who said the description matched the image;
- The number of people who confirmed that the description matches the image;
- The number of people who confirmed that the description does not match the image.

The `ExpertAnnotations.tsv` file contains data on the correspondence between the image and description, obtained as a result of a survey of experts. Column numbers and corresponding data type:

- The name of the image file.
- Description ID.

`3`, `4`, `5` — evaluations of three experts.

Experts rate on a scale from `1` to `4`, where `1` - the image and the request do not match at all, `2` - the request contains elements of the image description, but in general the request does not match the text, `3` - the request and the text match up to some details, `4` - the request and the text match completely.

The `test_queries.csv` file contains the information needed for testing:

- the query ID;
- the query text
- the relevant image.

Up to `5` descriptions can be available for one picture. The description ID has the format `<image file name>#<description serial number>`.
The `test_images` folder contains images for testing the model.

## Task

Build a model that is capable to get a textual description of some scene, and return several photos with the same or similar scene.

## Used Tools & Libraries
`pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`, `pytorch`, `transformers`, `torchvision`
