# ⚡ Energy Consumption Prediction using Snowflake

An end-to-end machine learning project for predicting household electricity consumption using **Snowflake** and **XGBoost**.

## 📌 Project Overview

This project implements a complete ML pipeline inside Snowflake, starting from raw energy and weather data and ending with automated model inference and deployment.

The project predicts household electricity consumption using historical weather conditions, electricity price, and time-based features.

## 🏗️ Architecture

Kaggle Dataset
        ↓
RAW_ENERGY
        ↓
Feature Engineering
        ↓
ENERGY_FEATURES
        ↓
Train / Validation Split
        ↓
XGBoost Model
        ↓
Snowflake Model Registry
        ↓
ENERGY_CONSUMPTION_XGB V2
        ↓
LANDING_ENERGY
        ↓
ENERGY_LANDING_STREAM
        ↓
Stored Procedure
        ↓
Automated Task
        ↓
ENERGY_GOLD
        ↓
Energy Consumption Prediction

## 🛠️ Technologies Used

- Snowflake
- Snowflake Notebooks
- Snowpark
- Python
- Pandas
- XGBoost
- SQL
- Snowflake Model Registry
- Snowflake Streams
- Snowflake Tasks

## 📊 Dataset

Dataset:

**Journey to Zero - Predict Electricity Consumption**

Source:

https://www.kaggle.com/competitions/predict-electricity-consumption/data

The dataset contains:

- Weather information
- Electricity price
- Timestamp
- Household electricity consumption

### Main Features

- Temperature
- Dew point temperature
- Relative humidity
- Wind direction
- Wind speed
- Atmospheric pressure
- Weather condition
- Electricity price
- Hour
- Day of week
- Month
- Day of year
- Weekend indicator

### Target

`CONSUMPTION`

## 🤖 Machine Learning Model

The project uses an **XGBoost Regressor** for predicting electricity consumption.



The final deployed model is:

```text
Model Name: ENERGY_CONSUMPTION_XGB
Version: V2
