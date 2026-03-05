# Customer Churn Prediction using Machine Learning

## Project Overview

Customer churn is a critical challenge for telecom companies. Retaining existing customers is significantly cheaper than acquiring new ones. This project builds a **machine learning model to predict customer churn** using demographic, service usage, and billing information.

The goal is to identify customers likely to leave the service so companies can take **proactive retention actions**.

---

# Dataset

Dataset used: **Telco Customer Churn Dataset**

Features include:

* Customer demographics
* Subscription details
* Internet services
* Billing information
* Contract type
* Payment methods

Target Variable:

```
Churn
```

Values:

* Yes
* No

---

# Project Workflow

The project follows a standard **end-to-end ML pipeline**:

### 1. Data Loading

* Load telecom churn dataset using Pandas
* Inspect dataset structure and datatypes

### 2. Data Cleaning

* Removed `customerID` column
* Handled missing values in `TotalCharges`
* Converted data types

### 3. Exploratory Data Analysis (EDA)

Performed:

* Class distribution analysis
* Numerical feature analysis
* Categorical feature distribution
* Correlation analysis

Tools used:

* Seaborn
* Matplotlib
* Pandas

---

### 4. Feature Engineering

* Label encoding / one-hot encoding for categorical features
* Feature scaling for numerical variables

---

### 5. Model Building

Machine Learning models used:

* Random Forest Classifier
* Decision Tree Classifier
* XGBoosting

Model training performed using **Scikit-Learn**.

---

### 6. Model Evaluation

Evaluation metrics used:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

These metrics help determine how well the model identifies customers likely to churn.

---

# Technologies Used

Python

Libraries:

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

# Repository Structure

```
customer-churn-prediction-ml
│
├── data
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── notebooks
│   └── Customer_Churn_Prediction.ipynb
│
├── models
│   └── churn_model.pkl
│
├── reports
│   └── figures
│
├── requirements.txt
├── README.md
└── .gitignore
```

---

# Key Insights

* Customers with **month-to-month contracts** are more likely to churn.
* **Higher monthly charges** increase churn probability.
* Customers with **longer tenure** tend to stay.

These insights can help telecom companies design **better retention strategies**.

---

# Future Improvements

Possible extensions:

* Hyperparameter tuning using GridSearchCV
* Feature importance analysis
* Model explainability using SHAP
* Deployment using Flask or FastAPI
* Real-time churn prediction API

---

# How to Run the Project

### Clone the repository

```
git clone https://github.com/sumittapa/customer-churn-prediction-ml.git
```

### Install dependencies

```
pip install -r requirements.txt
```

### Run the notebook

```
jupyter notebook
```

Open:

```
Customer_Churn_Prediction.ipynb
```

---

# Author

**Sumit Tapa**

M.Tech – Mathematical Modeling & Simulation
Interested in Machine Learning, Data Science, and Financial AI Systems
