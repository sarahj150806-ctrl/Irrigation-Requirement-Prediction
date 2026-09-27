# Irrigation-Requirement-Prediction
<img width="1106" height="971" alt="image" src="https://github.com/user-attachments/assets/a7258e9b-e53f-449d-b552-25bf38947622" />

## 📌 Project Overview

This project focuses on predicting the irrigation requirement of an agricultural field as **Low, Medium, or High** based on agricultural and environmental conditions.

The project uses Machine Learning to help classify irrigation requirements using factors such as soil moisture, temperature, humidity, rainfall, crop type, and crop growth stage.

---

## 🎯 Problem Statement

The aim of this project is to classify the irrigation requirement of an agricultural field into **Low, Medium, or High** using different soil, crop, weather, and irrigation-related features.

---

## 📊 Dataset

The project uses a **Predicting Irrigation Need** dataset obtained from Kaggle.

The training dataset contains:

- **630,000 rows**
- **21 columns**

The target variable is:

`Irrigation_Need`

Target classes:

- Low
- Medium
- High

Important features include:

- Soil Type
- Soil pH
- Soil Moisture
- Organic Carbon
- Electrical Conductivity
- Temperature
- Humidity
- Rainfall
- Sunlight Hours
- Wind Speed
- Crop Type
- Crop Growth Stage
- Season
- Irrigation Type
- Water Source
- Field Area
- Mulching Used
- Previous Irrigation
- Region

---

## 🔍 Data Analysis

The dataset was explored and checked for:

- Dataset shape and columns
- Data types
- Missing values
- Duplicate records
- Target class distribution
- Statistical summary
- Feature relationships

Exploratory Data Analysis was performed using visualizations such as:

- Irrigation requirement distribution
- Soil moisture vs irrigation requirement
- Temperature vs irrigation requirement

---

## ⚙️ Data Preprocessing

The data was divided into features (`X`) and target (`y`).

The `id` column was removed because it is only an identifier.

The dataset was split into:

- **80% Training Data**
- **20% Testing Data**

Categorical and numerical features were handled separately.

### Numerical Features
`StandardScaler` was used to standardize numerical features.

### Categorical Features
`OneHotEncoder` was used to convert categorical features into numerical form.

---

## 🤖 Machine Learning Model

A **Logistic Regression** model was used for classification.

The preprocessing and model were combined using a **Scikit-learn Pipeline**.

### Model Workflow

```text
Dataset
   ↓
Data Cleaning
   ↓
EDA
   ↓
Train-Test Split
   ↓
Preprocessing
   ↓
Logistic Regression
   ↓
Model Evaluation
   ↓
Prediction
