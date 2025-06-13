# Telecom-Customer-Retention
Telecom Customer Retention system using python

---

---

## 🗂️ Dataset Overview

* **File**: `telecom_chrn.csv`
* **Columns**: 21
* **Target Variable**: `Churn` (Yes/No)
* **Features include**: Age, contract type, monthly charges, support calls, and more.

---

## 🎯 Project Objectives

* 🧠 **Predict**: Identify customers likely to churn.
* 🔍 **Analyze**: Understand the driving factors behind churn.
* 💡 **Act**: Suggest strategies to retain those at risk.

---

## ⚙️ Methodology

### 📌 1. Data Preparation

* **Tools Used**: `Pandas`, `NumPy`, `Matplotlib`, `Seaborn`, `Missingno`
* **Steps**:

  * Loaded and cleaned the data
  * Handled missing values
  * Converted categorical text into numerical codes
  * Visualized distributions and correlations

### ✂️ 2. Feature Selection

Removed low-impact features such as:

* `Partner`, `PhoneService`, `OnlineBackup`, `TechSupport`, `OnlineSecurity`

### 🤖 3. Model Building

* **Model**: XGBoost Classifier
* **Hyperparameters**:

  * `learning_rate = 0.1`
  * `max_depth = 5`
* **Evaluation**: Accuracy and AUC-ROC

### 🏁 4. Results

* ✅ **Accuracy**: 80.36%
* 📈 **AUC Score**: 0.844985
* Indicates strong performance in identifying potential churners

---

## 🧩 Target Stakeholders & Applications

| Stakeholder                             | Role & Application                                             |
| --------------------------------------- | -------------------------------------------------------------- |
| **Customer Retention Teams**            | Design promotions or support initiatives for at-risk customers |
| **Marketing Teams**                     | Launch personalized campaigns and loyalty programs             |
| **Customer Support Teams**              | Prioritize calls and services to customers likely to churn     |
| **Business Analysts & Data Scientists** | Interpret results, refine the model, and provide insights      |
| **Management / Executives**             | Allocate resources, track retention goals, and measure ROI     |

---

## 🧰 Tech Stack

### 👨‍💻 Programming Language

* **Python**: For data processing, analysis, and model development

### 📦 Libraries Used

* **Pandas**: Data loading & manipulation
* **NumPy**: Numerical computations
* **Matplotlib & Seaborn**: Visualizations
* **Missingno**: Missing value analysis
* **Scikit-learn**:

  * `StandardScaler` for feature scaling
  * `train_test_split`, `GridSearchCV` for training & tuning
  * `metrics` for evaluation
* **XGBoost**: Model training and optimization

### 🧪 Environment

* **Notebook**: `Telecom_Churn_Case_Study.ipynb`
* **Platform**: Google Colab

---

## 📁 Project Structure

```
telecom-churn-prediction/
│
├── data/
│   └── telecom_chrn.csv
├── notebooks/
│   └── Telecom_Churn_Case_Study.ipynb
├── models/
├── visuals/
├── src/
├── requirements.txt
└── README.md
```

---

## 📌 Future Enhancements

* Deploy model as a web service/API
* Implement real-time churn alerts
* Integrate predictions into CRM tools

---
