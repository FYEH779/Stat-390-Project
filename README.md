# Stat-390-Project

## Introduction and Project Overview
This project explores the effectiveness of various time series forecasting models in predicting COVID-19 new case trends, providing insights into their strengths and weaknesses. The ARIMA and Auto-ARIMA models were effective in capturing short-term linear trends in stationary data but struggled with overfitting. The best results were observed with Prophet Multiple, which effectively utilized multiple seasonality patterns and specific predictors like the reproduction rate, yet failed to accurately capture fluctuations. This project highlighted the importance of data quality and feature engineering in time series analysis. With improved data quality, the model performances improve significantly, as shown using data before July 2022 on XGBoost and LSTM.

## Methodologies
- **Data Preparation**: The original dataset includes COVID-19 data for more than 200 countries. A subset was created containing 10 European countries and processed to handle missing values. Outliers were processed differently for each model 
- **Models Used**:
  - ARIMA Auto-ARIMA: For capturing linear trends
  - Prophet (Single and Multivariate): For handling seasonality and incorporating additional regressors
  - XGBoost: For managing large, complex datasets
  - LSTM: For capturing long-term dependencies.
- **Performance Metrics**: Models were primarily evaluated using the Root Mean Squared Error (RMSE) metric.

## Repository Structure
- 'owid-covid-data.xlsx/': Contains the COVID-19 dataset used for the analysis.
- 'data_clean/': Contains processed data for model-specific implementations
- 'notebooks/': Jupyter notebooks with detailed analysis and model evaluation

## Running the Code
1. Run notebook on data prep
2. Run the models to replicate the forecasting results

