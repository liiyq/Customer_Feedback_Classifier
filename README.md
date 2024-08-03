# Needle in a Haystack

## Overview
This project identifies non-complaint customer tweets using an LSTM model.

## Data
- `complaint.txt`: Contains samples of complaint tweets.
- `noncomplaint.txt`: Contains samples of non-complaint tweets.
- `customertweets.csv`: Contains tweets that may be complaints or non-complaints. The task is to find non-complaints.

## Model
The project uses an LSTM model to classify tweets. The model is trained on preprocessed text data with TF-IDF vectorization.
