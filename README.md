# ford-vehicle-assessment
Machine Learning-based Ford vehicle price prediction and assessment application built with Python, Scikit-learn, Pandas and Streamlit.
# 🚗 Ford Vehicle Price Prediction & Assessment

A Machine Learning-based web application for predicting the estimated market value of Ford vehicles using historical vehicle data.

The project includes Exploratory Data Analysis (EDA), data preprocessing, categorical encoding, feature scaling, Linear Regression, model evaluation, model serialization using Joblib, and a Streamlit-based interactive application.

---

## 📌 Project Overview

The objective of this project is to build a Machine Learning model that can estimate the price of a Ford vehicle based on its specifications and characteristics.

The application allows users to enter vehicle information such as:

- Ford model
- Manufacturing year
- Mileage
- Transmission
- Fuel type
- Tax
- MPG
- Engine size

The trained Machine Learning model then generates an estimated vehicle value.

The project also provides a professional Streamlit interface designed as a vehicle assessment and insurance-support portal.

> **Note:** The Machine Learning model predicts vehicle price/value. It does not directly predict an insurance premium.

---

## 🎯 Objectives

- Analyze the Ford vehicle dataset.
- Perform Exploratory Data Analysis (EDA).
- Understand relationships between vehicle features and price.
- Handle categorical variables.
- Apply feature scaling.
- Train a Linear Regression model.
- Compare different encoding approaches.
- Evaluate model performance using R² score.
- Save the trained model using Joblib.
- Build an interactive Streamlit application.
- Deploy the application for real-world demonstration.

---

## 📊 Dataset

The project uses a Ford vehicle dataset containing information about Ford cars and their prices.

### Features

| Feature | Description |
|---|---|
| `model` | Ford vehicle model |
| `year` | Manufacturing year |
| `transmission` | Type of transmission |
| `mileage` | Vehicle mileage |
| `fuelType` | Type of fuel |
| `tax` | Vehicle tax |
| `mpg` | Miles per gallon |
| `engineSize` | Engine size |
| `price` | Target variable / vehicle price |

The target variable for the Machine Learning model is:

```text
price
