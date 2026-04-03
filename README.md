# Loan_Risk_Scoring

## Overview

This project implements an end-to-end **data engineering and machine learning pipeline** for loan risk scoring. It simulates how financial institutions assess borrower risk using transactional, behavioral, and credit data.



## Business Problem

Lenders must determine which borrowers are likely to repay loans and which pose a high risk of default. Traditional credit scoring systems rely on static and limited data, often missing real-time behavioral signals.

This project addresses that challenge by building a pipeline that integrates:

* Transaction patterns
* Credit history
* Income data



### Key Components

* **Data Generation**: Simulated financial datasets (users, transactions, credit history)
* **Data Storage**: SQLite
* **Transformation Layer**: SQL-based feature engineering
* **Feature Store**: Curated ML-ready features
* **ML Model**: Logistic Regression for risk classification


## Pipeline Flow

1. **Data Generation**

   * Simulates users, transactions, and credit history
   * Includes fraud signals and late payment behavior

2. **Data Ingestion**

   * Loads datasets into SQLite

3. **Data Transformation**

   * SQL models aggregate and clean data

4. **Feature Engineering**

   * Creates features such as:

     * Debt-to-income ratio
     * Fraud indicators
     * Late payment streaks

5. **Model Training**

   * Logistic Regression model predicts default risk

6. **Output**

   * Risk scores categorized as:

     * Low Risk
     * Medium Risk
     * High Risk


