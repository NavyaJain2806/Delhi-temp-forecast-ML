# Project Statement

## Problem Statement

Accurate short‑term temperature forecasting is essential for planning daily activities, managing energy usage, and mitigating heat‑related risks in a dense urban city like New Delhi. This project aims to build a data‑driven system that predicts daily temperatures for a future month (October 2025) using past multi‑year temperature records. The goal is to design, implement, and evaluate machine learning models that can learn temporal patterns in historical data and provide reliable forecasts with low prediction error.

## Scope of the Project

- Use historical daily temperature data for New Delhi from 2020 up to September 2025.  
- Perform end‑to‑end processing: data loading, cleaning, feature engineering, model training, evaluation, and visualization in a single, reproducible notebook.  
- Focus on regression‑based time‑series forecasting for one target variable: daily maximum temperature.  
- Compare at least two models (Linear Regression and Random Forest) to analyse which approach provides better accuracy and generalisation on unseen October 2025 data.  
- Present results in a form suitable for academic evaluation, including tables, plots, and a clear discussion of model performance.

## Target Users

- **Students and educators** in data science, machine learning, and statistics who need a compact but complete example of time‑series forecasting.  
- **Researchers and analysts** exploring baseline ML approaches for city‑level climate or energy‑demand studies in New Delhi.  
- **Planners and enthusiasts** interested in understanding historical temperature behaviour and simple predictive modelling for urban heat conditions.

## High‑Level Features

- **Data Input & Preprocessing**  
  - Reads historical and October 2025 temperature data from CSV files stored in Google Drive.  
  - Parses date columns, sorts records chronologically, and handles missing values created by lag features.

- **Feature Engineering & Time‑Series Design**  
  - Derives calendar features (year, month, day) from the datetime column.  
  - Creates a “previous‑day temperature” feature to capture short‑term temporal dependence.  

- **Model Training & Comparison**  
  - Trains a Linear Regression model as a simple baseline.  
  - Trains a Random Forest regressor with a small hyperparameter search to capture non‑linear relationships.  
  - Evaluates both models using MAE, RMSE, MAPE, and accuracy metrics.

- **Reporting, Visualization & Interpretation**  
  - Generates a day‑wise comparison table showing actual temperature, both model predictions, and their errors.  
  - Plots long‑term historical temperature trends (2020–Sept 2025) for context.  
  - Plots actual vs predicted temperatures for October 2025 for both models on a single graph.  
  - Summarises which model performs better overall and highlights how much improvement is gained over the simpler baseline.
