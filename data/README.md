# Telco Customer Churn Dataset

This repository contains the **Telco Customer Churn** dataset, sourced from Kaggle. This dataset is designed for machine learning and data analytics projects aimed at understanding and predicting customer churn behaviors in the telecommunications industry. The data is rich with customer information, including service plans, tenure, payment methods, and churn status, making it an excellent resource for various real-world business applications.

## Dataset Overview

The **Telco Customer Churn** dataset provides detailed customer information from a telecom company, which can be used to analyze customer behavior and predict churn. The dataset can also help identify patterns and features that influence customer retention and satisfaction.

### Features

The dataset contains the following key features:

1. **Customer Demographics**:
   - `gender`: Male or Female.
   - `SeniorCitizen`: Whether the customer is a senior citizen (1: Yes, 0: No).
   - `Partner`: Whether the customer has a partner (Yes or No).
   - `Dependents`: Whether the customer has dependents (Yes or No).

2. **Service Information**:
   - `tenure`: Number of months the customer has stayed with the company.
   - `PhoneService`: Whether the customer has phone service (Yes or No).
   - `MultipleLines`: Whether the customer has multiple phone lines (Yes, No, or No phone service).
   - Internet service-related features like:
     - `InternetService`: Type of internet service (DSL, Fiber optic, or No).
     - `OnlineSecurity`: Whether the customer has online security add-on (Yes, No, or No internet service).
     - `OnlineBackup`, `DeviceProtection`, `TechSupport`: Other add-on services.

3. **Contract and Payment Details**:
   - `Contract`: Customer’s contract type (Month-to-month, One year, Two year).
   - `PaperlessBilling`: Whether the customer has opted for paperless billing (Yes or No).
   - `PaymentMethod`: How the customer pays (e.g., electronic check, mailed check, bank transfer, or credit card).
   - `MonthlyCharges`: The amount charged to the customer monthly.
   - `TotalCharges`: Total amount charged to the customer.

4. **Target Variable**:
   - `Churn`: Indicates whether the customer churned (Yes or No).

### Dataset Format

- **File Name**: `Telco-Customer-Churn.csv`
- **Format**: CSV (Comma-Separated Values)
- **Rows**: 7,043 (each row corresponds to a customer)
- **Columns**: 21 (representing different features and the target variable)

### Sample Data

| CustomerID | Gender | SeniorCitizen | Tenure | Contract        | MonthlyCharges | TotalCharges | Churn |
|------------|--------|---------------|--------|-----------------|----------------|--------------|-------|
| 7590-VHVEG | Female | 0             | 1      | Month-to-month  | 29.85          | 29.85        | No    |
| 5575-GNVDE | Male   | 0             | 34     | Two year        | 56.95          | 1889.5       | No    |
| 3668-QPYBK | Male   | 0             | 2      | Month-to-month  | 53.85          | 108.15       | Yes   |

## Dataset Source

The dataset was sourced from the Kaggle platform and is available for download at the following link:
[Telco Customer Churn on Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn?resource=download).

## Acknowledgments

- **Dataset Source**: [Kaggle](https://www.kaggle.com/datasets/blastchar/telco-customer-churn?resource=download)
- Thanks to the Kaggle community for providing access to high-quality datasets.

---
