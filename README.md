# Credit Card Fraud Detection Project

## Problem Statement:  
The objective of this project is to develop machine learning models to predict fraudulent credit card transactions. The dataset used for analysis is customer-level data collected and analyzed during a research collaboration between Worldline and the Machine Learning Group. The dataset, obtained from Kaggle (https://www.kaggle.com/mlg-ulb/creditcardfraud), consists of 284,807 transactions, out of which 492 are fraudulent. Due to the highly imbalanced nature of the dataset, handling class imbalance is necessary before building the models.

## Business Problem Overview:  
For banks, retaining high-profitable customers is a top business goal. However, banking fraud poses a significant threat to this goal. It affects financial losses, trust, and credibility for both banks and customers. According to a report by Nilson (https://nilsonreport.com/upload/content_promo/The_Nilson_Report_Issue_1164.pdf), banking frauds were estimated to account for $30 billion worldwide by 2020. With the increase in digital payment channels, fraudulent transactions are also on the rise, using new and different methods. Implementing proactive monitoring and fraud prevention mechanisms, such as credit card fraud detection using machine learning, has become a necessity for banks. Machine learning helps reduce manual reviews, costly chargebacks and fees, and denials of legitimate transactions.

## Understanding and Defining Fraud :    
Credit card fraud refers to any dishonest act or behavior aimed at obtaining unauthorized information from the account holder for financial gain. Common types of fraud include skimming (duplicating information from the magnetic strip of a card), manipulation/alteration of genuine cards, creation of counterfeit cards, stolen/lost credit cards, and fraudulent telemarketing.

## Data Dictionary:  
  
The dataset includes credit card transactions made by European cardholders over a two-day period in September 2013. Out of 284,807 transactions, 492 were fraudulent. The dataset is highly unbalanced, with the positive class (frauds) accounting for 0.172% of the total transactions. The dataset has undergone Principal Component Analysis (PCA) for confidentiality, resulting in features represented as V1, V2, V3, up to V28. The "time" feature represents the elapsed seconds between the first transaction and subsequent transactions, while the "amount" feature represents the transaction amount. The "class" feature indicates the class labeling, with 1 denoting fraud and 0 denoting non-fraud.

## Project Pipeline:  

The project pipeline can be summarized in the following five steps:    
**1. Data Understanding:** Load and understand the features in the dataset to select the relevant features for the final model.  
**2. Exploratory Data Analysis (EDA):** Perform univariate and bivariate analyses of the data, considering feature transformations if necessary. Check for skewness and address it if present to avoid issues during model building.  
**3. Handling Class Imbalance:** Due to the highly imbalanced nature of the dataset, apply random oversampling, ADASYN, and SMOTE techniques to balance the classes and improve model performance.  
**4. Train/Test Split and Cross-Validation:** Split the data into training and testing sets and utilize Stratified K-fold cross-validation for model evaluation. Choose an appropriate number of folds to ensure proper representation of the minority class in the test folds.  
**5. Model Building, Hyperparameter Tuning, and Optuna:** Explore XGBoosting algorithm for model building. Use GridSearchCV and Optuna for hyperparameter tuning to optimize model performance.  
**6. Model Evaluation:** Evaluate the models using appropriate evaluation metrics. Given the imbalanced data, prioritize accurate identification of fraudulent transactions over

## Results

