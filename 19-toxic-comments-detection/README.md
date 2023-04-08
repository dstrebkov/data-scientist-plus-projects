# Toxic comments classification

## Data

Dataset consists of `2` columns:

- `text` column with the text of the comment;
- `toxic` column determining whether the comment was toxic or not (target feature).

## Task

Having a labeled English comments dataset with toxity markup, create a model to classify them into `toxic` and `non-toxic` classes.

Try to improve model's `F1`-measure by using additional linguistic features derived from:

- syntactic parser (`spacy`) results (so-called _syntactic bigrams_);

- open-sourced sentiment lexicons [_AFINN_](http://corpustext.com/reference/sentiment_afinn.html) and [_NRC Lexicon_](https://saifmohammad.com/WebPages/NRC-Emotion-Lexicon.htm).

## Used Tools & Libraries
`pandas`, `numpy`, `matplotlib`, `seaborn`, `nltk`, `spacy`, `lightgbm`, `afinn`, `nrclex`
