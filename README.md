# Customer-Churn-Prediction
Customer Churn Prediction using the Telco Customer Churn dataset. This project covers business understanding, dataset inspection, exploratory data analysis (EDA), machine learning problem framing, and model planning as part of the AnalystLab Africa Machine Learning Internship.

📌 Project Overview
This project is part of the AnalystLab Africa Machine Learning Internship Programme – Week 1 Assignment.
The project focuses on understanding and framing a real-world machine learning problem using customer churn data. The objective is to understand the business problem, inspect the dataset, perform exploratory data analysis, and propose suitable machine learning approaches for predicting customer churn.

🎯 Business Problem
ABC Communications Ltd wants to predict customers who are likely to leave the company before they actually churn.
Customer churn can lead to revenue loss and increased customer acquisition costs. A machine learning solution can help the company identify customers at risk of leaving so that appropriate customer retention strategies can be implemented.

🎯 Business Objective
The main objective is to use historical customer information to identify patterns associated with customer churn and prepare a machine learning solution capable of predicting whether a customer is likely to leave the company.
The expected business benefits include:
- Improving customer retention
- Reducing customer loss
- Supporting data-driven decision-making
- Improving customer satisfaction
- Reducing customer acquisition costs

📊 Dataset
The project uses the Telco Customer Churn Dataset.
The dataset contains information about customers, including demographic information, services subscribed to, account information, contract details, and billing information.

Target Variable
Churn
The target variable indicates whether a customer has left the company:
- "Yes" – Customer churned
- "No" – Customer did not churn

🔍 Project Tasks
The Week 1 assignment covers the following tasks:
1. Business Research
Research was conducted on:
- Machine Learning
- Predictive Analytics
- Customer Churn

2. Dataset Inspection
The dataset was inspected to identify:
- Data types
- Missing values
- Duplicate records
- Data quality issues

3. Problem Framing
The machine learning problem was defined by identifying:
- Target variable
- Input features
- Problem type
- Preprocessing requirements

4. Exploratory Data Analysis
The dataset is explored using:
- 3 bar charts
- 2 histograms
- 1 correlation heatmap

5. Machine Learning Proposal
Suitable:
- Machine learning algorithms
- Evaluation metrics
- Preprocessing strategies
were proposed for the customer churn classification problem.

🤖 Machine Learning Problem
This project is a supervised binary classification problem.
The model will predict whether a customer is likely to churn based on their available customer and service information.
Proposed Algorithms
The proposed algorithms include:
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Gradient Boosting / XGBoost

Evaluation Metrics
The proposed evaluation metrics include:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC
- Confusion Matrix

🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

📁 Project Structure

Customer-Churn-Prediction/
│
├── README.md
├── .gitignore
├── requirements.txt
│
├── data/
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── notebooks/
│   └── Customer_Churn_Analysis.ipynb
│
├── reports/
│   ├── Business_Understanding_Report.pdf
│   ├── Dataset_Inspection_Report.pdf
│   └── Machine_Learning_Proposal.pdf
│
└── images/
    ├── bar_chart_1.png
    ├── bar_chart_2.png
    ├── bar_chart_3.png
    ├── histogram_1.png
    ├── histogram_2.png
    └── correlation_heatmap.png

📄 Project Deliverables
The project includes:
- Business Understanding Report
- Dataset Inspection Report
- Jupyter Notebook
- Machine Learning Proposal
- GitHub Repository

📈 Expected Outcome
The project aims to establish a clear understanding of the customer churn problem, identify important characteristics of the dataset, explore relationships within the data, and develop a suitable plan for building a customer churn prediction model.

👨‍💻 Author

Ojo Olaife Oluwaponmile 

Machine Learning Intern
AnalystLab Africa Machine Learning Internship Programme

📌 Note
This repository represents the work completed for Week 1 of the AnalystLab Africa Machine Learning Internship Programme. The focus of this stage is business understanding, data understanding, exploratory analysis, problem framing, and machine learning planning.


Customer Churn Prediction — Week 2

Project Overview

This project is part of the AnalystLab Africa Machine Learning Internship Programme – Week 2.

The project focuses on Data Preprocessing and Feature Engineering using the Telco Customer Churn dataset. The objective is to transform the raw customer data into a clean and machine-learning-ready dataset for subsequent model development.

Business Problem

Customer churn is an important business problem for telecommunications companies because losing existing customers can negatively affect revenue and customer retention.

The goal of this project is to prepare customer data for a future machine learning model that will predict whether a customer is likely to churn.

Dataset

The project uses the Telco Customer Churn Dataset containing information about customers, their subscribed services, contract details, payment methods, charges, and churn status.

The target variable is:

- Churn — whether the customer left the company ("Yes"/"No").

Week 2 Objectives

The preprocessing workflow focuses on:

- Inspecting the dataset and identifying data-quality issues
- Handling missing values
- Validating and correcting data types
- Checking duplicate records
- Removing irrelevant features
- Engineering meaningful features
- Detecting potential outliers
- Selecting relevant features
- Encoding categorical variables
- Scaling numerical features
- Producing a machine-learning-ready dataset

Data Preprocessing

The following preprocessing steps were performed:

Missing Values

The "TotalCharges" column contained 11 missing values. Investigation showed that the affected customers had zero tenure. The missing values were therefore treated as zero after converting the column to a numerical data type.

Duplicate Records

The dataset was checked for duplicate records and duplicate customer identifiers. No duplicate customer IDs were identified.

Irrelevant Features

The "customerID" column was removed because it is an identifier and does not provide meaningful predictive information.

Feature Engineering

A new feature called "TotalServices" was created by counting the number of additional services subscribed to by each customer.

An "AverageMonthlySpend" feature was also explored. However, correlation analysis showed an extremely high correlation with "MonthlyCharges", so it was removed to reduce redundancy.

Outlier Detection

Numerical variables were examined using box plots and the Interquartile Range (IQR) method.

No potential outliers were detected, so no outlier removal or transformation was applied.

Feature Selection

Correlation analysis was used to examine relationships among numerical features. Constant-column analysis was also performed, and no constant features were identified.

Categorical Encoding

Categorical input features were converted into numerical variables using One-Hot Encoding.

The target variable "Churn" was converted to:

- "0" = No
- "1" = Yes

Feature Scaling

"StandardScaler" was used to standardize the numerical features so that they have approximately a mean of 0 and a standard deviation of 1.

The binary one-hot encoded variables remain represented as 0 and 1.

Project Structure

Customer-Churn-Prediction/
│
├── README.md
├── .gitignore
├── requirements.txt
│
├── data/
│   └── original dataset
│
├── notebooks/
│   └── Customer_Churn_Preprocessing.ipynb
│
├── reports/
│   ├── Business_Understanding_Report.pdf
│   └── Data_Preprocessing_Report.pdf
│
└── processed_data/
    └── processed_telco_customer_churn.csv

Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook
- Kaggle Notebook

Key Learning Outcomes

This project provided practical experience in preparing real-world data for machine learning. Key areas covered include data cleaning, missing-value treatment, feature engineering, categorical encoding, feature scaling, outlier detection, and feature selection.

Project Status

Week 2 — Data Preprocessing & Feature Engineering: Completed

The processed dataset is prepared for the next stage of the machine learning workflow: model development and evaluation.

Author

Ojo Olaife

Machine Learning Intern
AnalystLab Africa Machine Learning Internship Programme
