# 📊 Comprehensive Regression Analysis

## 📌 Project Overview
This project is part of the **Introduction to Machine Learning** course and focuses on building, training, and evaluating **regression models** on a Gas Turbine dataset.  
The goal is to **predict the Turbine Energy Yield (TEY)** based on environmental and operational parameters using different regression techniques.

---

## 👥 Team
- **Team Name:** TEAM ASPIRERS  
- **Members:**
  - Partha Mete 
  - Sudam Kumar Paul 

---

## 📂 Dataset
We use the **Gas Turbine CO & NOx Emission Dataset (2015)**.

- **Website:** Kaggle.
- **Target Variable:** `TEY` (Turbine Energy Yield in MWh)  
- **Features include:**
  - `AT` → Ambient Temperature (°C)  
  - `AP` → Ambient Pressure (mbar)  
  - `AH` → Ambient Humidity (%)  
  - `AFDP` → Air Filter Difference Pressure (mbar)  
  - `GTEP` → Gas Turbine Exhaust Pressure (mbar)  
  - `TIT` → Turbine Inlet Temperature (°C)  
  - `TAT` → Turbine After Temperature (°C)  
  - `CDP` → Compressor Discharge Pressure (mbar)  
  - `CO` → Carbon Monoxide Content (mg/m³)  
  - `NOX` → Nitrogen Oxides Content (mg/m³)  

📌 The dataset (`gt_2015.csv`) must be placed in Google Drive or the project directory.

---

## ⚙️ Steps & Methodology

### 1. **Data Preprocessing & EDA**
- Handling missing values, scaling features  
- Correlation heatmaps, multicollinearity check (VIF)  
- Distribution plots, boxplots, scatterplots  
- Outlier analysis  

### 2. **Models Implemented**
- **Linear Regression**
  - From scratch (Normal Equation)  
  - With Scikit-learn  
- **Polynomial Regression** (degree 2, 3, 4 with GridSearchCV)  
- **Gradient Descent Implementations**
  - Batch Gradient Descent (BGD)  
  - Mini-Batch Gradient Descent (MBGD)  
  - Stochastic Gradient Descent (SGD)  
- **Regularization Techniques**
  - Ridge Regression  
  - Lasso Regression  
  - ElasticNet Regression  
  - Early Stopping (with SGDRegressor)  


### 3. **Evaluation Metrics**
- RMSE (Root Mean Squared Error)  
- MAE (Mean Absolute Error)  
- R² (Coefficient of Determination)  

### 4. **Visualization**
- Regression plots (Actual vs Predicted)  
- Residual plots (Scatter, KDE, QQ plot)  
- Cost curves for gradient descent methods  
- Bar plots for train/test performance metrics  

---

## 📊 Results Summary
- **Polynomial Regression (degree 2)** achieved the **best performance** with highest R² (~0.97).  
- **Gradient Descent methods** converged successfully, with MBGD and BGD providing stable results.  
- **Regularization (Ridge, Lasso, ElasticNet)** helped manage overfitting while maintaining strong predictive power.  

---

## 📌 Key Learnings
- Understanding the impact of multicollinearity in regression
- Comparing regression methods with/without regularization
- Implementing gradient descent variations from scratch
- Importance of feature scaling and model evaluation

