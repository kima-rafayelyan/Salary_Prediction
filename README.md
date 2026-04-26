# Salary_Prediction
# 💼 Salary Prediction Model

This project builds and compares two regression models to predict employee salaries based on features such as age, experience, education, and job-related attributes.

---

## 📌 Project Overview

The main objectives of this project are:

- Clean and preprocess salary data  
- Handle missing values  
- Encode categorical variables  
- Train and evaluate two regression models  
- Select and save the best-performing model  

---

## 📂 Dataset

The dataset (`Salary_Data.csv`) contains the following features:

- **Age**
- **Years of Experience**
- **Gender**
- **Education Level**
- **Job Title**
- **Salary** (Target Variable)

---

## ⚙️ Data Preprocessing

The following steps are applied:

- Removed rows with missing **Salary**
- Filled missing numerical values using **mean**
  - Age
  - Years of Experience
- Filled missing categorical values using **mode**
  - Gender
  - Education Level
  - Job Title
- Standardized inconsistent values in **Education Level**
- Applied **One-Hot Encoding** to categorical features

---

## 🤖 Models Used

### 1. Multiple Linear Regression
- Uses all available features
- Captures relationships between multiple variables

### 2. Simple Linear Regression
- Uses only **Years of Experience**
- Serves as a baseline model

---

## 📊 Evaluation Metrics

Models are evaluated using:

- **RMSE (Root Mean Squared Error)**  
  Lower values indicate better performance

- **R² Score (Coefficient of Determination)**  
  Higher values indicate better fit

---

## 🏆 Model Selection

The model with the higher **R² score** is selected as the final model.

---

## 💾 Model Saving

The best model is saved using `joblib`:
```bash
best_salary_model.pkl
