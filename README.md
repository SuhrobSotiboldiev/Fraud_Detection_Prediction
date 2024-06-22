# Bank Account Fraud Prediction Model

### Table of Contents
- [Dataset](#dataset)
- [Model](#model)
- [Installation](#installation)
- [Contributing](#contributing)

## Overview
This project contains a machine learning model designed to detect bank account fraud. It utilizes the Bank Account Fraud (BAF) suite, a collection of six synthetic datasets that simulate realistic, biased, imbalanced, and dynamic fraud detection scenarios while preserving privacy.


## Dataset

The dataset used for this project is base.csv, which includes 1m entries and 32 features. The features are:

**fraud_bool** - Fraud label (1 if fraud, 0 if legit)

**income** - Annual income of the applicant in quantiles.Ranges between [0, 1].

**name_email_similarity** - Metric of similarity between email and applicant’s name. Higher values represent higher similarity. i.e. the applicant’s previous

**prev_address_months_count** - Number of months in previous registered address of the applicant. Ranges between [−1, 406] months (-1 is a missing

**current_address_months_count** - Months in currently registered address of the applicant.

**customer_age** - Applicant’s age in bins per decade (e.g, 20-29 is represented as 20).

**days_since_request** - Number of days passed since application was done. Ranges between [0, 78] days.

**intended_balcon_amount** - Initial transferred amount for application. Ranges between [−1, 108].

**payment_type** - Credit payment plan type. 5 possible (annonymized) values.

**zip_count_4w** - Number of applications within same zip code in last 4 weeks. Ranges between [1, 5767].

**and other 22 columns**

## Model

##### 1. Architecture 
The model is a Logistic Regeression configured as follows:

- Numerical data is imputed and scaled.
- Categorical data is imputed and one-hot encoded.
 

##### 2. Training Process
- Splitting the dataset into training and testing sets.
- Training a classification model (Logistic Regression).
- Evaluating the model's performance using appropriate metrics (precision, ROC curve, AUC score).

## Installation

##### Prerequisites

To run the model, you need to have Python installed along with the following libraries:

- pandas
- numpy
- scikit-learn

You can install the required libraries using pip:

    pip install pandas
    pip install numpy
    pip install scikit-learn 
    
##### Setup
    
1.Clone the repository:
    
    git clone https://github.com/SuhrobSotiboldiev/fraud_detection_prediction.git

2.Navigate to the project directory:

    cd bank_account_fraud_detection

3.Run the model training script:

    python bank_account_fraud_detection.py
    
This script will preprocess the data, train the model, and evaluate its performance

## Contributing
If you wish to contribute to this project, please fork the repository and submit a pull request. For major changes, please open an issue to discuss what you would like to change.
    
    
    
    
    
    
