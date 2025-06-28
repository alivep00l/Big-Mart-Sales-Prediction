# 🛒 Big Mart Sales Prediction using Machine Learning

This project involves building a machine learning model to predict sales of various products across different Big Mart outlets. By analyzing historical sales data, the model helps in forecasting future product demand — aiding inventory management and business strategy.

---

## 📌 Project Objective

- Predict the **sales of products** based on product characteristics and store attributes.
- Provide valuable insights to help **optimize product placement**, **restocking**, and **marketing decisions**.

---

## 📊 Dataset Overview

- **Total Rows**: 8,523  
- **Total Features**: 12  
- **Source**: [Kaggle – Big Mart Sales Prediction Dataset](https://www.kaggle.com/datasets/akashdeepkuila/big-mart-sales?resource=download)

### Key Features:
- `Item_Identifier`, `Item_Weight`, `Item_Fat_Content`
- `Item_Visibility`, `Item_Type`, `Item_MRP`
- `Outlet_Identifier`, `Outlet_Size`, `Outlet_Location_Type`, `Outlet_Type`
- `Item_Outlet_Sales` (Target variable)

---

## 🔧 Tools & Technologies Used

- **Python**, **Pandas**, **NumPy**
- **Seaborn** & **Matplotlib** for EDA
- **Scikit-learn**, **XGBoost** for modeling
- **Jupyter Notebook** for implementation

---

## 🧹 Data Preprocessing

- Handled **missing values** in `Item_Weight` and `Outlet_Size`
- **Encoded categorical variables** using Label Encoding and One-Hot Encoding
- **Standardized** inconsistent entries (e.g., fat content labels)
- Removed outliers and treated zero visibility values

---

## 🤖 Machine Learning Models Used

- **Linear Regression**
- **Random Forest Regressor**
- **XGBoost Regressor**

### ✅ Model Performance:
- Achieved **up to 63% R² accuracy**
- Evaluated using **R² score**, **Root Mean Squared Error (RMSE)**, and **Cross-Validation**

---

## 📈 Exploratory Data Analysis

- **Correlation heatmaps**, **distribution plots**, and **boxplots** were used to understand feature relationships
- Sales trends were explored across **store types**, **item categories**, and **MRP ranges**

---

## 📁 Repository Structure

```
Big-Mart-Sales-Prediction/
├── Big Mart Sales Prediction.ipynb
├── README.md
├── Train-Set.csv
├── Test-Set.csv
└── requirements.txt
```

---
