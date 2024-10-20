# Innoverge_IBMZ
HealthWatch: Predictive Analytics for Public Health

HealthWatch is a machine learning-based platform designed to predict high-risk regions for disease outbreaks and forecast future trends using diverse datasets, including healthcare infrastructure, disease incidence, environmental factors, and socio-economic conditions.
Table of Contents

    Project Overview
    Features
    Datasets
    Machine Learning Models
    Installation
    Usage
    
Project Overview

HealthWatch integrates multiple data sources to deliver insights into public health risks across regions. By leveraging classification and time-series forecasting models, the platform provides early warning systems for disease outbreaks and assists policymakers in allocating healthcare resources more efficiently.
Problem Statement

Predict and prevent public health crises by identifying high-risk regions based on factors such as healthcare availability, pollution, and disease incidence. Use time-series forecasting to provide actionable insights for future disease trends.
Features

    Classification Model: Predicts high-risk regions for diseases like HIV, TB, and diabetes based on environmental, healthcare, and socio-economic factors.
    Time-Series Forecasting: Forecasts future disease outbreaks using historical data and LSTM (Long Short-Term Memory) neural networks.
    Data Visualization: Visual representations of health risk scores, disease predictions, and future trends.
    Scalable: Adaptable for various regions by integrating new datasets and conditions.

Datasets

We used a variety of datasets to build the models:

    Hospitals Count in India
    HIV Data
    Country Health Indicators
    COVID, Flu, Cold Symptoms
    Healthcare Facility Ratings
    Income and Population Density
    Diabetes, Alcohol, TB, Tobacco, Hepatitis Incidence
    Air and Water Pollution Levels
    Geographical Data
    Food Malnutrition Data

Machine Learning Models

    Random Forest Classifier:
        Used for identifying high-risk regions by classifying areas based on integrated data from healthcare, socio-economic, and environmental sources.
        Key features: hospital_per_capita, pollution_index, and income_levels.

    LSTM for Time-Series Forecasting:
        Predicts future disease outbreaks by analyzing historical disease incidence.
        Provides forecasts for diseases like TB, diabetes, and hepatitis.

Installation

To set up the project locally, follow these steps:

    Clone the repository:

    bash

git clone https://github.com/yourusername/HealthWatch.git

Install required dependencies:

bash

pip install -r requirements.txt

Download the datasets and place them in the data folder. Ensure filenames match those referenced in the code.

Run the project:

bash

    python main.py

Usage
Prediction of High-Risk Regions

The model predicts regions with high disease risks based on healthcare, environmental, and socio-economic data. Simply provide the relevant data to get predictions.
Time-Series Forecasting

The forecasting model can be used to predict future disease outbreaks. The time-series data (e.g., historical disease rates) is input, and the LSTM model provides predictions for the upcoming periods.
Data Visualization

Visualize the predicted results and trends using:

bash

python visualize.py
