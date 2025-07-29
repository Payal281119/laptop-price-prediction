# 💻 Laptop Price Prediction for SmartTech Co.

A machine learning-powered solution to predict **laptop prices** based on technical specifications, brand, and hardware features. Built for **SmartTech Co.**, this model helps optimize pricing decisions, improve market competitiveness, and understand key price drivers using interpretable ML techniques.

---

## 🔍 Business Problem

- **High variation in specs** leads to inconsistent pricing.
- **Frequent model launches** require real-time price updates.
- **Low model transparency** creates trust issues in decision-making.
- **Unclear brand impact** complicates market positioning.

---

## 🎯 Project Objective

- 🎯 **Accurate Pricing**: Build a predictive model to estimate laptop prices from key features.
- 🎯 **Market Positioning**: Discover which specifications most influence pricing.
- 🎯 **Brand Insight**: Analyze how brands impact laptop pricing to assist strategy.

---

## 📄 Project Overview

- **Goal**: Use ML to predict laptop prices from structured data  
- **Data Source**: Internal SmartTech Co. dataset of laptops  
- **Approach**: Clean, transform, and feed structured laptop data into regression models  
- **Use Case**: Assist product teams in dynamic pricing for new and existing laptop models  
<br>

---

## 🚧 Key Challenges

- 📦 **High Feature Variety**: Different models and brands have vastly different configurations  
- ⏱️ **Real-Time Readiness**: Model must handle new laptop specs not seen before  
- 🧠 **Interpretability**: Price decisions must be explainable to stakeholders  
<br>

---

## 🛠️ Tools & Technologies

- **Python 3.x**
- **Jupyter Notebook**
- **Pandas / NumPy** – Data cleaning & transformation  
- **Seaborn / Matplotlib** – Data visualization  
- **Scikit-learn** – Model development (regression algorithms)  
- **Models**:  
  - Linear Regression  
  - Decision Tree Regressor  
  - Random Forest Regressor  
  - KNN (K-Nearest Neighbors)  
  - SVR (Support Vector Regressor)  
- **Evaluation Metrics**:  
  - R² Score  
  - RMSE  
  - MSE  

---

## 🧹 Data Cleaning & Feature Engineering

- Removed unnecessary columns (e.g., `Unnamed: 0`)
- Parsed `RAM`, `Storage`, and `Screen Resolution` into separate usable fields
- Cleaned inconsistent strings (e.g., CPU/OS names)
- Scaled numerical features
- Encoded categorical features (Label/One-Hot Encoding)
- Handled missing values, duplicates, and outliers

---

## 🤖 Model Building & Evaluation

### ✅ Best Performing Model: **Random Forest Regressor**
- **MSE**: 202,591,302  
- **RMSE**: ₹14,233  
- **R² Score**: 0.82  
- **Example**:  
  - Predicted: ₹96,469  
  - Actual: ₹93,635  
  - Error: ₹2,834 ✅ *(Low error, high accuracy)*

### 🚫 Weakest Model: **KNN**
- **RMSE**: ₹16,581  
- **R² Score**: 0.75  
- **Error Example**: ₹1,35,950 ❌ *(Poor generalization)*

---

## 📊 Insights & Interpretation

### ✅ What features impact laptop price the most?
- **CPU**
- **RAM**
- **SSD**
- **Brand (Company)**

### 🧠 Does brand affect price?
Yes — brand is a significant factor captured during training and impacts perceived value.

### 🚀 How does the model handle new laptops?
- **Random Forest** generalized well (only ₹2,834 error on a new model)
- **KNN** performed poorly on unseen configurations

---

## 🧪 Test Scenarios

| Scenario                                  | Result                                |
|------------------------------------------|----------------------------------------|
| Predict high-end laptops                 | ✅ High accuracy (low error)           |
| Predict lesser-known brands              | ⚠️ Partially accurate (depends on training data) |
| Predict newly launched laptops           | ✅ Good performance (RF model)         |
| Model explainability                     | ✅ Easy with Random Forest feature importances |

---

## 🖥️ Execution Instructions

1. Open `ML_project.ipynb` in Jupyter Notebook or Google Colab  
2. Install required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `sklearn`  
3. Run all cells step-by-step:  
   - Data Cleaning  
   - Feature Engineering  
   - Model Building  
   - Evaluation & Insights  

---
