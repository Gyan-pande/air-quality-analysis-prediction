Air Quality Analysis & Prediction Using Machine Learning
Project Overview

This project performs exploratory data analysis and machine-learning-based prediction on historical air-quality observations.

The project analyzes pollutant concentrations, sensor measurements, temperature, humidity, and time-based patterns. Machine learning models are then used to predict carbon monoxide (CO) concentration.

This project was developed as part of the IBM SkillsBuild Data Analytics with AI Academic Internship Program.

Objectives

Analyze historical air-quality data.

Clean and preprocess real-world environmental data.

Identify temporal pollution patterns.

Study relationships between pollutants and weather variables.

Visualize air-quality trends.

Build machine-learning models for CO concentration prediction.

Compare Linear Regression and Random Forest Regression.

Identify the most important features influencing prediction.

Dataset

The project uses the Air Quality Dataset from the UCI Machine Learning Repository.

Dataset page:

https://archive.ics.uci.edu/dataset/360/air+quality

The dataset contains 9,358 hourly observations collected from an air-quality multisensor device in an Italian urban environment.

The dataset contains measurements related to:

Carbon Monoxide (CO)

Non-Methanic Hydrocarbons (NMHC)

Benzene (C6H6)

Nitrogen Oxides (NOx)

Nitrogen Dioxide (NO2)

Sensor responses

Temperature

Relative Humidity

Absolute Humidity

The original dataset uses -200 to represent missing values. These values are converted to missing values during preprocessing.

Technologies Used

Python

Jupyter Notebook

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

Machine Learning Models
1. Linear Regression

Linear Regression is used as a baseline model to estimate the relationship between the input environmental variables and CO concentration.

2. Random Forest Regression

Random Forest Regression is used to capture nonlinear relationships between pollutant concentrations, sensor measurements, weather variables, and CO concentration.

Evaluation Metrics

The models are evaluated using:

Mean Absolute Error (MAE)

Root Mean Squared Error (RMSE)

R² Score

A lower MAE and RMSE indicate lower prediction error, while a higher R² indicates better explanatory performance.

Project Workflow
Dataset
   ↓
Data Loading
   ↓
Data Cleaning
   ↓
Missing Value Treatment
   ↓
Date/Time Processing
   ↓
Feature Engineering
   ↓
Exploratory Data Analysis
   ↓
Data Visualization
   ↓
Train/Test Split
   ↓
Machine Learning
   ↓
Model Evaluation
   ↓
Feature Importance
   ↓
Prediction & Conclusions

Setup Instructions
Step 1: Install Python

Python 3.9 or newer is recommended.

Step 2: Install dependencies

Open a terminal in the project folder and run:

pip install -r requirements.txt

Step 3: Download the dataset

Download AirQualityUCI.csv from the UCI Machine Learning Repository:

https://archive.ics.uci.edu/dataset/360/air+quality

Place the CSV file in the same directory as the Jupyter Notebook.

Step 4: Start Jupyter Notebook
jupyter notebook


Open:

YourName_AirQualityAnalysisPrediction.ipynb

Step 5: Run the notebook

Run the notebook cells from top to bottom.

Expected Results

The project produces:

Air-quality trend visualizations

Daily and monthly pollution patterns

Hourly CO analysis

Pollutant correlation heatmap

Temperature/humidity relationship analysis

Linear Regression results

Random Forest results

Actual vs predicted CO visualization

Feature-importance analysis

Limitations

This dataset represents measurements from a specific monitoring environment and historical period. Therefore, the model should not be interpreted as a universal predictor for every city or current air-quality condition.

The project predicts CO concentration rather than claiming to calculate an official AQI because the dataset does not provide all pollutant measurements required for a standardized AQI calculation.

Future Scope

Future versions could:

Use real-time air-quality APIs.

Include PM2.5 and PM10 measurements.

Predict AQI categories.

Use advanced time-series models.

Develop a web dashboard.

Deploy the model as an online prediction service.

Add anomaly detection for unusual pollution events.

Author

Dnyaneshwar Pande

IBM SkillsBuild Data Analytics with AI Academic Internship
