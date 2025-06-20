# Music-Popularity-Prediction
This project aims to classify songs as popular or non-popular based on various audio features using a Random Forest Classifier. The dataset is derived from Spotify data freely available online.

## Dataset
The dataset includes a wide range of audio and metadata features for each song:

- `acousticness`
- `danceability`
- `duration_ms`
- `energy`
- `explicit`
- `instrumentalness`
- `liveness`
- `loudness`
- `speechiness`
- `valence_yr`
- `popularity_yr`
- `mode`
- `key_0_yr` to `key_6_yr`

The original popularity column is used to generate binary labels:
- `1` → **Popular**
- `0` → **Non-popular**

## Objective
Build a classification model that can predict whether a song is popular or not, based on its audio characteristics.

## Approach
### 1. Data Preprocessing
- Cleaned and prepared the dataset.
- Converted the `popularity` column into binary labels.
- Handled categorical and one-hot encoded features.

### 2. Model Building
- Used a **Random Forest Classifier**.
- Trained the model on audio features.
- Evaluated using:
  - Accuracy
  - Confusion matrix
  - Classification report
  - ROC AUC Score
## Results
The Random Forest model demonstrated promising performance with ROC AUC score of 0.945 in distinguishing popular songs from non-popular ones based on audio characteristics alone.

