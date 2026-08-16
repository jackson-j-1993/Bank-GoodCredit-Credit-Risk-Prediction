# Bank-GoodCredit-Credit-Risk-Prediction
An end-to-end machine learning project for Bank GoodCredit to predict credit card default risk (30+ days-past-due) using SQL and Python.

## Project Overview
In banking, credit risk prediction helps reduce default losses, improve credit approval strategy, and monitor existing customers more effectively. Bank GoodCredit wants to predict the credit risk of current credit card customers. The primary business objective is to identify customers who are likely to become risky in the future, especially those who may fall into the 30+ days-past-due (DPD) bucket.

## Target Variable
The target variable for this binary classification problem is `bad_label`:
*   `0` indicates the customer has a good credit history.
*   `1` indicates the customer has a bad credit history or a 30+ DPD risk.

*Note: Exploratory Data Analysis reveals an imbalanced dataset with an overall bad rate of 4.2% (95.8% good customers vs. 4.2% bad customers).*

## Data Sources
The project utilizes data stored in a MySQL database, combining three primary tables to create a customer-level modeling dataset:
*   `Cust_Account`: Contains account-level financial variables like current balance, credit limit, and overdue amounts.
*   `Cust_Enquiry`: Contains customer enquiry records and amounts.
*   `Cust_Demographics`: Contains anonymized demographic features.

## Project Objectives
*   Load data from the SQL database securely.
*   Perform detailed data quality checks and exploratory analysis.
*   Create a customer-level feature matrix from account, enquiry, and demographic data.
*   Build and compare multiple machine learning models.
*   Evaluate models using ROC-AUC, Gini, and rank ordering.
*   Provide business recommendations and detail the challenges faced.

## Tech Stack
*   **Data Manipulation & Cleaning:** `pandas`, `numpy`
*   **Data Visualization:** `matplotlib`, `seaborn`
*   **Database Connectivity:** `sqlalchemy`, `pymysql`
*   **Machine Learning:** `scikit-learn` (Logistic Regression, Random Forest Classifier, Gradient Boosting Classifier)
