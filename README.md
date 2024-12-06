# Project 03 - Sunspots Forecasting on Daily, Monthly and Yearly Data

## Project Description
This project uses historical sunspot data to forecast future sunspot activity. The dataset includes daily, monthly, and yearly sunspot counts, and the model is developed using Facebook's Prophet library for time series forecasting. The project focuses on preprocessing the data, building predictive models, and evaluating their performance on unseen data.

## Features
- **Data Preprocessing:**
  - Handled missing values and transformed time columns into a suitable datetime format.
  - Supported daily, monthly, and yearly data preprocessing.
- **Exploratory Data Analysis (EDA):**
  - Visualized sunspot activity trends over time.
- **Modeling:**
  - Utilized Facebook's Prophet model with linear and logistic growth.
  - Incorporated custom seasonality to model solar cycles (11 years).
  - Tuned hyperparameters like changepoint prior scale, Fourier orders, and the number of changepoints.
- **Evaluation Metrics:**
  - Mean Absolute Error (MAE)
  - Mean Absolute Percentage Error (MAPE)
  - R² Score

## Dataset
The dataset includes sunspot observations at different time intervals
### Columns:
- **Daily Data:** Year, Month, Day, Fractional Year, Sunspot Number, Standard Deviation, Observations, Indicator.
- **Monthly Data:** Year, Month, Fractional Year, Sunspot Number, Standard Deviation, Observations, Indicator.
- **Yearly Data:** Year, Sunspot Number, Standard Deviation, Observations, Indicator.

## Usage

### Data Preprocessing:
- Preprocess the data by calling `data_preprocessing()` with the appropriate time unit (`'daily'`, `'monthly'`, or `'yearly'`).

### Forecasting:
- Use Facebook Prophet to build models for forecasting future sunspot counts.
- Add custom seasonality and tune parameters for improved forecasts.

### Evaluation:
- Evaluate the model using the following metrics:
  - **Mean Absolute Error (MAE)**
  - **Mean Absolute Percentage Error (MAPE)**
  - **R² Score**

### Visualizations:
- Visualize historical data and forecasted trends.

## Results

### Evaluation Metrics:
- **Mean Absolute Error (MAE):** (e.g., 12.34)
- **Mean Absolute Percentage Error (MAPE):** (e.g., 5.67%)
- **R² Score:** (e.g., 0.89)

### Forecasts:
- Predictions for the next 1, 10, and 20 years.
- Included predictions for daily, monthly, and yearly data.
