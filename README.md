# Weather Data Analysis and Forecasting

## Project Overview

This project analyzes historical weather data for Mohali, India, and develops machine learning models to predict next-day weather conditions. It explores weather patterns over a 10-year period (2016–2025) and evaluates the performance of regression and classification models.

## Objectives

- Analyze temperature, rainfall, humidity, and wind patterns.
- Explore monthly trends, seasonal variations, rainfall distribution, and correlations.
- Develop a regression model for next-day temperature prediction.
- Develop a classification model for next-day rainfall prediction.
- Compare machine learning approaches using appropriate evaluation metrics.
- Explore whether nearby-city weather data can improve prediction performance.

## Dataset

- **Location:** Mohali, India
- **Period:** January 2016 – December 2025
- **Records:** 3,653 daily observations
- **Source:** Open-Meteo Historical Weather API

### Variables

- Date
- Weather code
- Mean, maximum, and minimum temperature
- Rainfall
- Maximum wind speed
- Mean relative humidity

## Methodology

1. Data collection using the Open-Meteo API.
2. Data cleaning and preprocessing.
3. Exploratory Data Analysis (EDA).
4. Feature preparation and chronological train-test splitting.
5. Machine learning model development.
6. Model evaluation and comparison.
7. Next-day weather prediction demonstration.

## Machine Learning

### Temperature Prediction

A regression model predicts the next day's mean temperature.

Evaluation metrics:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

### Rainfall Prediction

A classification model predicts whether rainfall will occur the next day.

Evaluation metrics:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Project Structure

```text
Weather_Data_Analysis_and_Forecasting/
├── data/
│   └── mohali_weather_2016_2025.csv
├── notebooks/
│   └── weather_analysis.ipynb
├── scripts/
│   └── download_mohali_weather.py
├── results/
└── README.md
```

## Data Collection

The weather dataset can be downloaded using:

```bash
python scripts/download_mohali_weather.py
```

The script retrieves historical weather data from Open-Meteo and saves it as a CSV file.

Open-Meteo Historical Weather API: https://open-meteo.com/en/docs/historical-weather-api

No API key is required for this data source.

## Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Google Colab
- Open-Meteo API

## Project Status

The data collection script and exploratory analysis are completed. Model evaluation and nearby-city analysis are included in the project notebook.
- `data/` — Weather datasets
- `notebooks/` — Data analysis and machine learning notebooks
- `src/` — Python scripts
- `results/` — Graphs, tables, and model results
