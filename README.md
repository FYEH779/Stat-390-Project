# Stat-390-Project
## Introduction and Project Overview
In this project, we explored 6 different models and their effectiveness in predicting COVID-19 new cases in ten European countries. Our objective was to evaluate the effectiveness of six models: ARIMA, auto-ARIMA, Prophet (both Univariate and Multivariate), XGBoost, and LSTM. My best results were observed with XGBoost, which successfully captured trends across all ten countries and also kept test set RMSE values pretty low. This project really emphasized the importance of data quality and feature engineering when approaching different models

## Methodologies
Data Preparation: Our original dataset contained up-to-date COVID data for over 200 countries, so my first step was to select a date range with a meaningful amount of new cases, as well as subset my ten selected countries. I then dealt with missing values. Outliers were dealt with depending on the model.

Models Used:  
* ARIMA Auto-ARIMA: good at capturing linear trends
* Prophet (Single and Multivariate): these could handle seasonality, holidays, lockdowns, and incorporating additional regressors
* XGBoost: model for managing large, complex datasets
* LSTM: model for capturing long-term dependencies.

Performance Metrics: Models were primarily evaluated using the RMSE metric, and I also used how well the trend was captured to determine overall "successs".

## Repository Structure
* 'owid-covid-data.xlsx/': Contains the COVID-19 dataset used for the analysis.
* 'general_data_prep.ipynb': Contains the general data cleaning and prep applied to all models.
* 'model_X_model_name.ipynb': Each file is the notebook that contains model specific prep, tuning, and fitting.

## Running the Code
Each model notebook can be run to replicate forecasting results.