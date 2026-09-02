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


# Customer Churn Prediction — Week 2

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

# Customer Churn Prediction — Week 3 Machine Learning Project

## Project Overview

This project focuses on developing machine learning classification models to predict customer churn using a telecommunications customer dataset.

The project builds on the data understanding and preprocessing work completed in Week 2. In Week 3, the processed dataset was used to train, evaluate, and compare multiple machine learning models and identify the model most suitable for predicting customers who are likely to churn.

The project also includes feature-importance analysis and business recommendations based on the modelling results.

---

## Business Problem

Customer churn is an important business problem because losing existing customers can reduce revenue and increase the cost of acquiring new customers.

The objective of this project is to develop a machine learning model that can identify customers who are likely to churn so that the business can prioritize appropriate customer-retention strategies.

### Business Objective

The main objectives are to:

- Predict whether a customer is likely to churn.
- Compare different classification algorithms.
- Evaluate model performance using appropriate classification metrics.
- Identify the most important predictors of customer churn.
- Recommend a suitable model for the churn-prediction problem.
- Provide business insights that can support customer-retention decisions.

---

## Dataset

The project uses the Telco Customer Churn dataset.

The processed dataset contains:

- **7,043 observations**
- **32 features**
- **Churn** as the target variable

The target variable is binary:

| Churn | Description |
|---|---|
| 0 | Customer did not churn |
| 1 | Customer churned |

### Target Distribution

| Class | Count | Percentage |
|---|---:|---:|
| No Churn | 5,174 | 73.46% |
| Churn | 1,869 | 26.54% |

The target variable is therefore imbalanced, with non-churn customers representing the majority of observations.

---

## Project Workflow

The Week 3 workflow followed these major stages:

1. Load the processed dataset
2. Inspect the dataset
3. Separate features and target
4. Split the data into training and testing sets
5. Train classification models
6. Generate predictions
7. Evaluate model performance
8. Compare the models
9. Analyse feature importance
10. Generate business insights
11. Select the preferred model
12. Develop recommendations and next steps

---

## Machine Learning Algorithms

Four classification algorithms were evaluated:

### 1. Logistic Regression

Logistic Regression was used as a baseline classification model.

### 2. Decision Tree

Decision Tree was used to model nonlinear relationships through a tree-based structure.

### 3. Random Forest

Random Forest combines multiple decision trees to produce a more robust prediction.

### 4. XGBoost

XGBoost is a gradient-boosting algorithm that builds an ensemble of decision trees sequentially to improve predictive performance.

---

## Model Evaluation

The models were evaluated using:

- Accuracy
- Precision
- Recall
- F1 Score
- ROC-AUC

Recall and ROC-AUC were given particular attention because the business objective involves identifying customers who are likely to churn.

### Model Performance

| Model | Accuracy | Precision | Recall | F1 Score | ROC-AUC |
|---|---:|---:|---:|---:|---:|
| XGBoost | 0.7424 | 0.5092 | **0.8102** | **0.6254** | **0.8430** |
| Logistic Regression | 0.7381 | 0.5043 | 0.7834 | 0.6136 | 0.8417 |
| Random Forest | **0.7821** | **0.6184** | 0.4679 | 0.5327 | 0.8222 |
| Decision Tree | 0.7360 | 0.5026 | 0.5080 | 0.5053 | 0.6637 |

### Model Selection

XGBoost was selected as the preferred model because it achieved:

- The highest **Recall: 0.8102**
- The highest **F1 Score: 0.6254**
- The highest **ROC-AUC: 0.8430**

Although Random Forest achieved higher Accuracy and Precision, its Recall was considerably lower.

For a customer-retention problem, identifying a larger proportion of actual churners is important because failing to identify an at-risk customer may result in a lost retention opportunity.

---

## Feature Importance

Feature importance was analysed for both Random Forest and XGBoost.

### Random Forest — Top 10 Features

| Rank | Feature | Importance |
|---:|---|---:|
| 1 | TotalCharges | 0.174278 |
| 2 | tenure | 0.157923 |
| 3 | MonthlyCharges | 0.145814 |
| 4 | Contract_Two year | 0.061937 |
| 5 | InternetService_Fiber optic | 0.044022 |
| 6 | PaymentMethod_Electronic check | 0.037899 |
| 7 | TotalServices | 0.037482 |
| 8 | Contract_One year | 0.027158 |
| 9 | gender_Male | 0.025196 |
| 10 | PaperlessBilling_Yes | 0.023981 |

### XGBoost — Top 10 Features

| Rank | Feature | Importance |
|---:|---|---:|
| 1 | Contract_Two year | 0.363767 |
| 2 | Contract_One year | 0.178733 |
| 3 | InternetService_Fiber optic | 0.119743 |
| 4 | InternetService_No | 0.075932 |
| 5 | PaymentMethod_Electronic check | 0.040388 |
| 6 | StreamingMovies_Yes | 0.036806 |
| 7 | tenure | 0.036159 |
| 8 | OnlineSecurity_Yes | 0.026336 |
| 9 | PaperlessBilling_Yes | 0.018009 |
| 10 | StreamingTV_Yes | 0.011147 |

### Key Feature-Importance Findings

Several predictors appeared as important across the tree-based models, including:

- Contract type
- Internet service
- Tenure
- Payment method
- Paperless billing
- Customer charges

XGBoost placed particularly strong importance on contract-related variables, while Random Forest placed greater importance on TotalCharges, tenure, and MonthlyCharges.

Feature importance represents predictive contribution and should not be interpreted as proof of causation.

---

## Statistical Findings

The processed dataset was also examined statistically.

### Descriptive Statistics

| Variable | Mean | Standard Deviation | Minimum | Maximum |
|---|---:|---:|---:|---:|
| SeniorCitizen | 0.1621 | 0.3686 | 0 | 1 |
| tenure | 32.3711 | 24.5595 | 0 | 72 |
| MonthlyCharges | 64.7617 | 30.0900 | 18.25 | 118.75 |
| TotalCharges | 2279.7343 | 2266.7945 | 0 | 8684.80 |

### Correlation Analysis

The correlation between:

- **tenure and TotalCharges:** 0.8262
- **MonthlyCharges and TotalCharges:** 0.6512

The strong positive relationship between tenure and TotalCharges is expected because customers who remain with the company for longer periods have more time to accumulate charges.

---

## Business Insights

The modelling and statistical analysis provide several useful business insights:

1. **Contract type is an important predictor of churn.**  
   Contract-related variables were particularly important in the XGBoost model.

2. **Internet service is an important predictive factor.**  
   InternetService_Fiber optic and InternetService_No were among XGBoost's strongest predictors.

3. **Customer tenure is important.**  
   Tenure was one of the leading predictors in both tree-based models.

4. **Charges contain useful predictive information.**  
   TotalCharges and MonthlyCharges were particularly important to Random Forest.

5. **Payment method may be relevant to churn risk.**  
   Electronic check was among the important predictors in both models.

---

## Business Recommendations

Based on the modelling results, the following actions are recommended:

- Use the XGBoost model to identify customers with elevated churn risk.
- Prioritize retention campaigns for high-risk customers.
- Investigate customers based on contract type and consider strategies that encourage longer-term contracts.
- Examine the customer experience associated with important internet-service segments.
- Investigate electronic-check customers for possible billing or payment-related issues.
- Combine predicted churn risk with customer value when prioritizing retention activities.
- Monitor model performance regularly after deployment.

---

## Limitations

Several limitations should be considered:

- The dataset contains an imbalanced target variable.
- Model performance is based on the available dataset and test data.
- Feature importance does not establish causal relationships.
- The model should be validated on new data before being used in a production environment.
- Business intervention thresholds should consider the cost of retention campaigns and the value of customers.

---

## Technologies Used

The project was developed using Python and common machine learning and data-analysis libraries.

### Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook / Kaggle Notebook

---
Project Structure
text
week-3-customer-churn/
│
├── data/
│   └── processed_dataset.csv
│
├── notebooks/
│   └── week3_modeling.ipynb
│
├── reports/
│   ├── Business_Insights_Report.pdf
│   ├── Model_Evaluation_Report.pdf
│   ├── Feature_Importance_Report.pdf
│   └── Statistical_Analysis_Report.pdf
│
├── visualizations/
│   ├── model_performance.png
│   ├── roc_curves.png
│   └── feature_importance_comparison.png
│
├── README.md
└── requirements.txt

Machine Learning Intern
AnalystLab Africa Machine Learning Internship Programme

OJO OLAIFE OLUWAPONMILE 























## 
# HealthConnect — Week 4: ML Problem Definition
## Project Overview
This project is part of the AnalystLab Africa Machine Learning Internship – Week 4 Experience Lab.
The project focuses on HealthConnect, a healthcare appointment system aimed at improving patient appointment attendance and healthcare support using data and artificial intelligence.
The Week 4 task focuses on understanding the healthcare appointment problem, examining the available data, and determining whether the dataset can support a machine learning solution for predicting appointment no-shows.
## Business Problem
Missed healthcare appointments can affect the effective use of available appointment slots and may create challenges in healthcare service delivery.
HealthConnect therefore seeks to understand patterns associated with appointment attendance and determine whether patient and appointment information can be used to identify appointments that are at risk of becoming no-shows.
A machine learning solution could eventually help healthcare teams identify higher-risk appointments and support better appointment management.
## Project Objective
The main objective of this project is to:
1. Understand the HealthConnect appointment business problem.
2. Inspect and understand the available appointment data.
3. Identify the potential machine learning target variable.
4. Examine the features that may be useful for prediction.
5. Assess data quality and potential modelling challenges.
6. Define an appropriate machine learning problem.
7. Propose a suitable modelling approach for future development.
## Dataset
The project uses the HealthConnect Appointment Dataset.
The dataset contains:
5,000 appointment records
18 columns
Each record represents an individual healthcare appointment and contains information relating to patients, appointment scheduling, and appointment outcomes.
The main outcome variable of interest is:
appointment_outcome
which records appointment outcomes such as:
Attended
No-Show
Cancelled
For the proposed machine learning problem, No-Show is the primary outcome of interest.
Machine Learning Problem
The proposed machine learning problem is a classification problem.
Target
The model will aim to predict whether an appointment is likely to result in a No-Show.
Proposed Target Definition
For the modelling stage, the outcome can be formulated as:
1 → No-Show
0 → Attended
Cancelled appointments will require separate consideration during the modelling stage based on the project requirements and data-handling decisions.
## Proposed ML Workflow
The planned machine learning workflow is:
HealthConnect Data
        ↓
Data Ingestion
        ↓
Data Validation & Inspection
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Target & Feature Definition
        ↓
Feature Selection
        ↓
Train/Test Split
        ↓
Preprocessing Pipeline
        ↓
Model Training
        ↓
Model Evaluation
        ↓
Model Comparison
        ↓
No-Show Risk Prediction
        ↓
Future Operational Use

## Technologies
The project will primarily use Python and common data science and machine learning libraries, including:
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
Jupyter Notebook / Kaggle Notebook
Additional machine learning libraries may be introduced during later modelling stages where appropriate.

## Week 4 Scope
This week's work focuses on problem definition and data understanding, rather than completing the final predictive model.
The major activities include:
Business understanding
Dataset inspection
Target variable analysis
Feature review
Data quality assessment
Machine learning problem definition
Proposed modelling approach
Identification of assumptions, risks, and dependencies


## Expected Outcome
At the end of Week 4, the project should provide a clear understanding of:
The healthcare business problem.
The proposed machine learning problem.
The prediction target.
Potential predictive features.
Data quality considerations.
The proposed modelling workflow.
Requirements and considerations for the next stage of development.


Project Structure
Week-4-HealthConnect/
│
├── notebooks/
│   └── HealthConnect_Week4_ML_Problem_Definition.ipynb
│
├── data/
│   └── README.md
│
├── reports/
│   ├── Business_Understanding_Report.pdf
│   └── ML_Problem_Definition.pdf
│
├── images/
│   └── ...
│
└── README.md

Note: The raw HealthConnect dataset and data dictionary should not be uploaded to a public GitHub repository unless their sharing permissions explicitly allow redistribution.

## Project Status
Current Stage: Week 4 — ML Problem Definition & Data Understanding
Status: In Progress
The project will proceed to data preparation and model development in subsequent stages.
Author
Ojo Olaife Oluwaponmile
Program: AnalystLab Africa — Machine Learning Internship
Project: HealthConnect — Improving Patient Appointment Attendance and Healthcare Support Using Data and AI
Machine Learning / Data Science Student
Week 4  Machine Learning Internship Project

https://drive.google.com/file/d/1kLBU6VsEy5RsQzm0HUcD15ANp897XcWe/view?usp=drivesdk

