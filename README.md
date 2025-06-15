# 📈 Sales Forecasting with Machine Learning (Walmart Dataset)

## 📌 Overview

This project focuses on **forecasting weekly sales** for a major retail chain using machine learning. The aim is to help businesses **predict demand**, manage **inventory**, and plan **promotions and pricing** by learning from historical trends.

We use Walmart's real-world dataset, apply **feature engineering**, and train a **Random Forest model** that achieves strong predictive performance.

---

## 📂 Dataset Source

> 📍 [Kaggle: Walmart Store Sales Forecasting](https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting)

- `train.csv`: Weekly sales per store and department
- `features.csv`: Temperature, Fuel Prices, CPI, Unemployment, MarkDowns, etc.
- `stores.csv`: Store type and size

---

## 🧰 Tech Stack

- **Language:** Python 3
- **IDE:** JupyterLab
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `joblib`

---

## 🛠️ Key Steps

### ✅ 1. Data Cleaning
- Merged all datasets using `Store`, `Dept`, and `Date`
- Handled missing values (MarkDowns)
- Converted `IsHoliday` to binary
- Feature engineered `Year`, `Month`, `Week`, `Day`, and `DayOfWeek`

### ✅ 2. Model Training
- Target: `Weekly_Sales`
- Final Model: **Random Forest Regressor**

### ✅ 3. Model Performance

| Metric       | Value         |
|--------------|---------------|
| R² Score     | **0.8822**    |
| RMSE         | **₹7,838.68** |

🔍 The model explains **88.2%** of the variance in weekly sales — highly accurate for retail forecasting.

---

## 🔍 Feature Importance

The top 5 most influential features:

1. **Dept** – Different categories have distinct sales patterns
2. **Size** – Bigger stores = bigger sales
3. **Store** – Location-specific behavior
4. **Week** – Seasonal demand
5. **CPI** – Economic conditions influence spending

---

## 🚀 How to Run the Project

### 📦 Option A: Run Locally via JupyterLab (Recommended)

### 1. Clone the repository:
git clone https://github.com/saadsanadi-ds/SalesForecasting-Project.git

 cd SalesForecasting-Project

### 2. Open the notebook:
- Launch JupyterLab
- Go to: `notebook/sales_forecasting.ipynb`

### 3. Run all cells:
- The notebook will guide you through data cleaning, model building, and evaluation.

---

## 📁 Project Structure
<pre> SalesForecasting-Project/
├── notebook/
│   └── sales_forecasting.ipynb       ← Main notebook
├── model/
│   └── random_forest_sales_model.joblib  ← Saved model
├── README.md                         ← You’re reading this  </pre>


## ✅ Requirements

- Python 3.x
- JupyterLab
- Libraries: pandas, numpy, scikit-learn, matplotlib, seaborn, joblibib
