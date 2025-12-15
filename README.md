Advanced Time Series Forecasting using NeuralProphet

Project Overview
This project implements an advanced time series forecasting system using daily sales data.
The objective is to analyze historical sales patterns and generate accurate future forecasts by capturing trend and seasonality.

The project compares the performance of NeuralProphet models with a classical SARIMAX benchmark to identify the best forecasting approach.

Folder Structure

advanced-time-series-forecasting-neuralprophet/

data

full_data.csv

train_data.csv

test_data.csv

notebooks

01_data_preprocessing.ipynb

02_modeling_and_evaluation.ipynb

outputs

forecast.png

metrics.csv

report

README.md

Data Description

Type: Daily sales time series data

Columns:

ds : Date

y : Sales value

The dataset contains clear trend, weekly seasonality, and yearly seasonality patterns.

Notebooks Description

01_data_preprocessing.ipynb

Generates a synthetic daily sales dataset

Introduces trend and seasonality

Splits data into training and testing sets

Saves prepared datasets into the data folder

02_modeling_and_evaluation.ipynb

Trains NeuralProphet baseline model

Trains tuned NeuralProphet model

Trains SARIMAX benchmark model

Evaluates models using MAE, RMSE, and MAPE

Saves forecast visualization and evaluation metrics

Models Used

NeuralProphet Baseline

NeuralProphet Tuned

SARIMAX Benchmark

Evaluation Metrics

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

Mean Absolute Percentage Error (MAPE)

Evaluation results are saved in outputs/metrics.csv.

Results Summary

NeuralProphet baseline achieved the best overall performance

The model effectively captures trend and seasonal patterns

SARIMAX showed comparatively higher error values

Forecast visualization is saved as outputs/forecast.png.

Conclusion

NeuralProphet proves to be a robust and reliable model for forecasting daily sales data with strong seasonality.
This project demonstrates how neural-based forecasting models outperform traditional statistical approaches for complex time series data.