# 🚗 Car Price Predictor using Machine Learning
A Machine Learning project that predicts the resale price of used cars based on features such as car model, company, manufacturing year, kilometers driven, and fuel type. This project demonstrates the complete machine learning workflow, including data cleaning, preprocessing, feature engineering, model training, evaluation, and prediction using Scikit-learn. The final model achieved a best **R² Score of 0.8457** after optimizing the train-test split. :contentReference[oaicite:0]{index=0}
---
## 📌 Project Overview
The objective of this project is to build a regression model capable of estimating the market price of used cars. The project involves cleaning a real-world dataset, transforming features, training a Linear Regression model, and generating price predictions for unseen data. The workflow follows an end-to-end machine learning pipeline suitable for beginners and intermediate learners.
---
## 🎯 Problem Statement
Used car prices vary depending on multiple factors such as brand, manufacturing year, fuel type, and mileage. Determining a fair resale price manually is difficult and often subjective.
This project aims to develop a machine learning model that predicts the estimated selling price of a used car based on its characteristics, helping buyers and sellers make informed decisions.
---
## 📂 Dataset Information
**Dataset:** Quikr Used Car Dataset
### Features
| Feature | Description |
|----------|-------------|
| Name | Car Model |
| Company | Manufacturer |
| Year | Manufacturing Year |
| Price | Selling Price (Target Variable) |
| kms_driven | Distance Driven |
| fuel_type | Fuel Type |
### Dataset Summary
- Original Records: **892**
- Cleaned Records: **815**
- Target Variable: **Price**
The dataset required extensive cleaning due to inconsistent values, missing entries, and formatting issues before model training. :contentReference[oaicite:1]{index=1}
---
## 📊 Exploratory Data Analysis (EDA)
The dataset was explored to understand:
- Dataset shape
- Data types
- Missing values
- Unique values
- Statistical summary
- Data quality issues
### Key Findings
- Non-numeric values in the **Year** column
- "Ask For Price" entries in the **Price** column
- Missing values in **Fuel Type**
- Non-numeric values in **Kilometers Driven**
These issues were resolved during preprocessing. :contentReference[oaicite:2]{index=2}
---
## 🧹 Data Preprocessing
The following preprocessing steps were performed:
- Removed invalid year values
- Converted year to integer format
- Removed "Ask For Price" records
- Converted prices to numeric values
- Cleaned kilometers driven values
- Removed missing fuel type records
- Shortened vehicle names
- Removed extreme price outliers
- Created a cleaned dataset for modeling
---
## ⚙️ Feature Engineering
Categorical features were encoded using **OneHotEncoder**.
Features used for prediction:
- Car Name
- Company
- Manufacturing Year
- Kilometers Driven
- Fuel Type
A **ColumnTransformer** was used to combine encoded categorical variables with numerical features before model training. :contentReference[oaicite:3]{index=3}
---
## 🤖 Machine Learning Model
The project uses:
- **Linear Regression**
The preprocessing pipeline and model were combined using Scikit-learn's **Pipeline** for efficient training and prediction. :contentReference[oaicite:4]{index=4}
---
## 📈 Model Performance
### Evaluation Metric
- R² Score
### Results
| Model | Score |
|---------|-------|
| Initial Model | **0.6371** |
| Optimized Model | **0.8457** |
The model was trained multiple times using different random states, and the best-performing model was selected. :contentReference[oaicite:5]{index=5}
---
## 🔮 Prediction Example
### Input
| Feature | Value |
|----------|-------|
| Car Name | Maruti Suzuki Swift |
| Company | Maruti |
| Year | 2019 |
| Kilometers Driven | 100 |
| Fuel Type | Petrol |
### Predicted Price
```text
₹458,894
```
The trained model predicts the estimated resale value based on the provided vehicle details. :contentReference[oaicite:6]{index=6}
---
## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Jupyter Notebook
- Pickle
---
## 📦 Project Structure
```text
car-price-predictor-machine-learning/
│
├── Dataset/
│   ├── quikr_car.csv
│   └── Cleaned_Car.csv
│
├── Notebook/
│   └── Car_Price_Predictor.ipynb
│
├── Model/
│   └── LinearRegressionModel.pkl
│
│
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```
---
## 🚀 Future Improvements
- Random Forest Regressor
- XGBoost Regressor
- Hyperparameter Tuning
- Cross Validation
- Streamlit Web Application
- Flask API Deployment
- Docker Support
- Cloud Deployment
---
## 📌 Skills Demonstrated
- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Preprocessing
- Machine Learning
- Linear Regression
- Model Evaluation
- Scikit-learn Pipelines
- Predictive Analytics
- Model Serialization
---
---
## 📜 License
This project is licensed under the **MIT License**.
---
## 👨‍💻 Author
**Pradeep**
If you found this project useful, consider giving it a ⭐ on GitHub.
