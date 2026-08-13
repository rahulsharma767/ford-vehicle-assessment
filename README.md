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

🔎 Exploratory Data Analysis

The project performs EDA to understand:

Dataset structure
Missing values
Numerical feature distributions
Categorical feature distributions
Price distribution
Relationships between vehicle features and price
Correlation between numerical variables
Outliers and data patterns

Visualizations are created using Python data-analysis and visualization libraries.

⚙️ Data Preprocessing

The categorical variables include:

model
transmission
fuelType

Two approaches were explored:

1. One-Hot Encoding

Categorical variables were converted into binary indicator columns using:

pd.get_dummies()
2. Label Encoding

Categorical variables were converted into numerical representations using:

LabelEncoder()

The project compared the performance of these approaches.

🤖 Machine Learning Model

The project uses:

Linear Regression

from Scikit-learn.

The dataset is divided into training and testing sets using:

train_test_split(
    test_size=0.2,
    random_state=42
)

Feature scaling is performed using:

StandardScaler()
📈 Model Evaluation

The models were evaluated using the R² score.

The One-Hot Encoding approach achieved approximately:

R² ≈ 0.846

The Label Encoding approach achieved approximately:

R² ≈ 0.736

The One-Hot Encoding approach performed better on the evaluated test set.

The currently deployed Streamlit application uses the Label Encoding model saved in model.joblib.

💾 Model Serialization

The trained Machine Learning model is saved using Joblib:

joblib.dump(model_data, "model.joblib")

The application loads the trained model using:

joblib.load("model.joblib")

This allows the Streamlit application to use the already-trained model without retraining it every time the application starts.

🖥️ Streamlit Application

The project includes an interactive Streamlit web application.

Application Features
Customer information section
Vehicle information section
Ford model selection
Manufacturing year input
Mileage input
Transmission selection
Fuel type selection
Engine size input
Tax input
MPG input
Insurance coverage selection
Policy duration selection
Machine Learning vehicle valuation
Assessment ID generation
Vehicle assessment summary
🏗️ Application Workflow
Ford Vehicle Dataset
        ↓
Data Cleaning
        ↓
Exploratory Data Analysis
        ↓
Feature Engineering
        ↓
Categorical Encoding
        ↓
Feature Scaling
        ↓
Train/Test Split
        ↓
Linear Regression
        ↓
Model Evaluation
        ↓
Joblib Model Serialization
        ↓
Streamlit Application
        ↓
User Vehicle Details
        ↓
Preprocessing
        ↓
ML Prediction
        ↓
Estimated Vehicle Value
🛠️ Technologies Used
Programming Language
Python
Machine Learning
Scikit-learn
Linear Regression
LabelEncoder
StandardScaler
Train/Test Split
R² Score
Data Analysis
Pandas
NumPy
Visualization
Matplotlib
Seaborn
Application
Streamlit
Model Deployment
Joblib
GitHub
Streamlit Community Cloud
📁 Project Structure
ford-vehicle-price-prediction/
│
├── app.py
├── ford.csv
├── model.joblib
├── requirements.txt
└── README.md
