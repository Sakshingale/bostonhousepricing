# 🏠 Advanced House Price Prediction

## 📌 Project Overview

This project predicts **house prices using advanced machine learning and feature engineering techniques**.  
The dataset contains multiple housing attributes such as **property size, location features, and construction details**.

The goal is to build a **robust regression model** that accurately predicts the **SalePrice** of houses by performing:

- **Data Cleaning**
- **Exploratory Data Analysis (EDA)**
- **Feature Engineering**
- **Feature Selection**
- **Machine Learning Modeling**

This project demonstrates an **end-to-end data science pipeline used in real-world predictive modeling.**

---

# 🏗️ Project Architecture


Raw Data (train.csv, test.csv)
│
▼
Exploratory Data Analysis
│
▼
Data Cleaning
(Missing Value Handling)
│
▼
Feature Engineering
(Encoding, Transformations)
│
▼
Feature Selection
(Lasso Regression)
│
▼
Model Training
(Regression Models)
│
▼
Model Evaluation
(RMSE / R² Score)
│
▼
Final Prediction Model


---

# 📂 Project Structure


Advanced-House-Price-Prediction
│
├── data
│ ├── train.csv
│ ├── test.csv
│ └── X_train.csv
│
├── notebooks
│ ├── Exploratory Data Analysis.ipynb
│ ├── Feature Engineering.ipynb
│ └── Feature Selection.ipynb
│
├── outputs
│ ├── selected_features.csv
│ └── trained_model.pkl
│
├── requirements.txt
├── .gitignore
└── README.md


---

# 📊 Dataset

The dataset is taken from the **Kaggle House Prices Competition**.

It contains:

- **79 explanatory variables**
- Residential homes located in **Ames, Iowa**

### 🎯 Target Variable

**SalePrice**

This variable represents the **final selling price of the house.**

---

# 🔍 Exploratory Data Analysis (EDA)

EDA was performed to understand the **structure and distribution of the dataset.**

Key steps include:

- Checking **dataset shape and data types**
- Identifying **missing values**
- **Distribution analysis** of numerical features
- **Correlation analysis**
- Detecting **outliers**

---

# ⚙️ Feature Engineering

Feature engineering improves **model performance by transforming raw variables.**

Techniques applied:

- Missing value **imputation**
- **Rare category handling**
- **Label encoding**
- **Log transformation** for skewed variables

---

# 🎯 Feature Selection

Feature selection was performed to **reduce dimensionality and keep only important predictors.**

**Method Used**

- **Lasso Regression + SelectFromModel**

Example:

```python
from sklearn.linear_model import Lasso
from sklearn.feature_selection import SelectFromModel

feature_sel_model = SelectFromModel(Lasso(alpha=0.005, random_state=0))
feature_sel_model.fit(X_train, y_train)
🤖 Machine Learning Models

The following regression models can be used:

Linear Regression

Lasso Regression

Ridge Regression

Random Forest Regressor

Gradient Boosting Regressor

📈 Model Evaluation Metrics

Model performance is evaluated using:

RMSE (Root Mean Squared Error)

MAE (Mean Absolute Error)

R² Score

These metrics measure how well the model predicts house prices.

🛠️ Technologies Used
Tool	Purpose
Python	Programming language
Pandas	Data manipulation
NumPy	Numerical operations
Scikit-learn	Machine learning
Matplotlib	Data visualization
Seaborn	Statistical visualization
Jupyter Notebook	Development environment
🚀 Project Workflow

1️⃣ Exploratory Data Analysis
2️⃣ Feature Engineering
3️⃣ Feature Selection
4️⃣ Model Training

🎯 Key Learning Outcomes

Through this project, the following skills were developed:

Real-world data preprocessing

Handling missing values

Feature engineering techniques

Feature selection using Lasso

Regression model development

End-to-end machine learning workflow

👩‍💻 Author

Sakshi Ingale
