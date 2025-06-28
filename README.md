# 🛒 Big Mart Sales Prediction using Machine Learning

This repository contains a machine learning project that predicts sales for Big Mart products using historical sales data. The project involves cleaning real-world data, analyzing trends, and building a regression model to forecast sales based on product and outlet characteristics.

---

## 📌 Objective

To build an ML model that predicts **Item Outlet Sales** using product features and store attributes. This helps Big Mart in:
- Better inventory planning
- Strategic marketing
- Improved supply chain management

---

## 📊 Dataset Description

- **Source**: [Kaggle - Big Mart Sales Dataset](https://www.kaggle.com/datasets/brijbhushannanda1979/bigmart-sales-data)
- **Shape**: 8,523 rows × 12 columns

### 🔑 Feature Details:
| Feature | Description |
|---------|-------------|
| `Item_Identifier` | Unique product ID |
| `Item_Weight` | Weight of product |
| `Item_Fat_Content` | Low Fat/Regular |
| `Item_Visibility` | % of product visible in store |
| `Item_Type` | Type/category of product |
| `Item_MRP` | Maximum Retail Price |
| `Outlet_Identifier` | Unique store ID |
| `Outlet_Establishment_Year` | Year store was established |
| `Outlet_Size` | Size of the store |
| `Outlet_Location_Type` | Urban/Tier 2/3 classification |
| `Outlet_Type` | Grocery store, Supermarket type |
| `Item_Outlet_Sales` | 💡 Target variable – Product sales |

---

## 📊 Exploratory Data Analysis

- Distribution plots for numeric features: `Item_Weight`, `Item_MRP`, `Item_Visibility`, `Item_Outlet_Sales`
- Countplots for categorical variables: `Item_Fat_Content`, `Item_Type`, `Outlet_Size`
- Year-wise outlet establishment trends

---

## 🧹 Data Cleaning & Preprocessing

- Filled missing `Item_Weight` using **mean**
- Imputed missing `Outlet_Size` based on **mode by outlet type**
- Standardized categorical values like `Item_Fat_Content` (`LF` → `Low Fat`)
- Applied **Label Encoding** to convert categorical variables into numeric form

---

## 🧠 Model Building

### 🔍 Model Used:  
**XGBoost Regressor** – chosen for its robustness in handling structured data.

### 📉 Train-Test Split:
- 80% training, 20% testing using `train_test_split`

### 🧪 Model Evaluation:
- **R² Score on Training Set**: ~0.63  
- **R² Score on Testing Set**: ~0.57  
(*indicates model slightly overfits but captures major trends*)

---

## 📁 Project Workflow

1. **Import Libraries**: Load pandas, numpy, seaborn, matplotlib, XGBoost, sklearn
2. **Load Dataset**: Read and explore the CSV data
3. **Clean & Preprocess**: Handle missing values, fix labels, encode categories
4. **EDA**: Visualize trends using plots
5. **Train-Test Split**: Separate the data
6. **Model Training**: Train XGBoost on the training data
7. **Evaluate Model**: Check R² scores and prediction quality
