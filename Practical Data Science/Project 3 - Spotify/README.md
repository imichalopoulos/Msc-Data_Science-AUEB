# Ioannis Michalopoulos - MSc Data Science, Athens University Of Economics And Business Department of Informatics
# Spotify Valence Prediction

## Overview
This project analyzes which Spotify audio features influence **Valence**, a measure of musical positivity. Regression models are used to identify important predictors and to build a model capable of predicting valence from audio features.

---

## Dataset
The dataset contains Spotify track-level audio features such as:
- Danceability, Energy, Loudness
- Acousticness, Speechiness, Instrumentalness
- Liveness, Tempo, Duration
- Musical attributes (key, mode, time signature)

Categorical features are encoded using one-hot encoding.

---

## Methodology
- Exploratory data analysis and correlation analysis
- Feature selection using correlation strength and stepwise selection
- Data split into **training and test sets**
- Regression modeling with:
  - **Ridge Regression** (regularization and interpretability)
  - **Random Forest Regressor** (non-linear relationships)

---

## Hyperparameter Optimization
- **GridSearchCV** was used to tune the Ridge Regression regularization parameter (`alpha`)
- **Optuna** was used for automated hyperparameter optimization using trial-based search
- Cross-validation and **Mean Absolute Error (MAE)** guided model selection

---

## Results
- Energy, danceability, and acousticness were identified as key predictors of valence
- Final model performance was evaluated on a **hold-out dataset**
- The Random Forest model achieved an MAE of approximately **0.13**


