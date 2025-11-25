# DelhiTemp ML Forecast

## Overview
This project constructs a time‑series temperature forecasting system for New Delhi based on historical daily temperature data. It accesses two CSV files from Google Drive, engineers date‑based and previous‑day temperature features, and trains both Linear Regression and Random Forest models to predict daily temperatures for October 2025. The predictions will be compared with the actual values through standard regression metrics and visual plots.

## Features
Loads historical and October 2025 temperature data from CSV files in Google Drive
- Parses date columns and creates year, month, day and previous‑day temperature features
• Trains and evaluates Linear Regression and tuned Random Forest models
- Calculates MAE, RMSE, MAPE, and accuracy for both models
- Provides a day‑wise comparison table for actual values, predictions, and errors
- Plots historical temperature trend — 2020–Sept 2025
- Plots actual vs predicted temperatures for October 2025 for both models

## Technologies / Tools Used
- Python 3
- Google Colab + Google Drive
- pandas, NumPy
- scikit‑learn (LinearRegression, RandomForestRegressor)
- Matplotlib

## Steps to Install & Run the Project
1. Open the notebook (`Delhi_temp_prediction.ipynb`) in Google Colab.
2. Upload `dataset1.csv` (historical data) and `dataset2.csv` (October 2025 data) in your drive.
3. In the notebook run all cells from top to the bottom:
    - Mount Google Drive
    - Load data and create features
    - Train models and evaluate them
    - Display tables and plots
  
## Testing Instructions
1. Confirm that:
  - `dataset1.csv` includes a `datetime` column and a `temp` column for 2020–Sept 2025.
  - `dataset2.csv` includes a `datetime` column and a `temp` column for October 2025.

2. After running the notebook:
   - Check the **day‑wise comparison table** to make sure each October date has actual, Linear Regression and Random Forest predictions and errors.
   - Check the **metrics table** to compare MAE, RMSE, MAPE and accuracy for both models. 
   - Observe the **comparison plot** to visualize which model follows the actual curve more closely.

## Screenshots
### 1. Historical Temperature Trend (2020–Sept 2025)
![Day-wise Prediction Table](https://github.com/user-attachments/assets/1996b0e1-fff6-4c0e-b7d6-5af83a4d7e2a)

### 2. Day‑wise Prediction Table (sample, first 10 days)
![Historical Temperature Trend](https://github.com/user-attachments/assets/11e59bc6-dd34-4315-aaac-cbd8890c52df)

### 3. Model Evaluation Metrics (Linear Regression vs Random Forest)
![Actual vs Predicted Temperature](https://github.com/user-attachments/assets/242f9e40-ce07-4c40-b9eb-372b759b1566)

### 4. Actual vs Predicted Temperature: October 2025
![Model Evaluation Metrics](https://github.com/user-attachments/assets/e154ca04-6472-43ec-a79f-ef03ba19bc53)
