# 🏠 Housing Price Prediction – Linear Regression from Scratch  

[![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)  
[![NumPy](https://img.shields.io/badge/NumPy-1.20%2B-orange.svg)](https://numpy.org/)  
[![Pandas](https://img.shields.io/badge/Pandas-1.3%2B-green.svg)](https://pandas.pydata.org/)  
[![Matplotlib](https://img.shields.io/badge/Matplotlib-3.4%2B-yellow.svg)](https://matplotlib.org/)  
[![Seaborn](https://img.shields.io/badge/Seaborn-0.11%2B-red.svg)](https://seaborn.pydata.org/)  

This project implements **Linear Regression from scratch (without sklearn’s LinearRegression)** to predict **house prices** using both numerical and categorical features.  
It includes **data preprocessing, outlier handling, scaling, one-hot encoding, closed-form regression, visualization, and interactive user prediction.**

---

## 📌 Features  

- ✅ Load & Explore Housing Dataset  
- ✅ Outlier Removal using IQR  
- ✅ Manual Data Preprocessing:  
  - Standard Scaling for numerical features  
  - One-Hot Encoding for categorical features  
- ✅ Linear Regression using **Normal Equation**:  

\[
\beta = (X^TX)^{-1}X^Ty
\]

- ✅ Model Evaluation (MSE & R² Score)  
- ✅ Visualizations for insights  
- ✅ Interactive CLI input for house price prediction  

---

## 📊 Dataset  

Dataset: **Housing.csv**  

Features include:  

- **Numerical** → `area`, `bedrooms`, `bathrooms`, `stories`, `parking`  
- **Categorical** → `mainroad`, `guestroom`, `basement`, `hotwaterheating`, `airconditioning`, `prefarea`, `furnishingstatus`  
- **Target** → `price`  

---

## ⚙️ Workflow  

1. **Data Cleaning & Outlier Removal** → IQR method (15th–85th percentile)  
2. **Train-Test Split** → Custom implementation (`test_train()` function)  
3. **Transformation** →  
   - Numerical → Scaled using `(x - mean)/std`  
   - Categorical → One-hot encoding  
4. **Model Training** → Calculate weights & bias using closed-form regression  
5. **Prediction** → Implemented manually  
6. **Evaluation** → MSE & R² Score  
7. **Visualization** → Distribution plots, scatter plots, error plots  

---

## 📈 Visualizations  

- **Price Distribution**
- **Predicted vs Actual Prices**
- **Prediction Errors**

Example Plot (Predicted vs Actual):  

![Example Plot](https://user-images.githubusercontent.com/0000000/predicted-vs-actual.png)  

---

## 🧮 Mathematical Formula  

\[
y = X\beta + \epsilon
\]

Where:  
- \(X\) → Feature matrix (with bias column of ones)  
- \(\beta\) → Coefficients (weights)  
- \(y\) → Target variable (log-transformed price in training)  

---

## 🚀 Usage  

### 1️⃣ Clone the Repo  

```bash
git clone https://github.com/yourusername/housing-price-prediction.git
cd housing-price-prediction
