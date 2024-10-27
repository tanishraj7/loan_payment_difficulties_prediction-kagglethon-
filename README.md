# Loan Payment Difficulties Prediction
This project aims to predict whether a client will experience payment difficulties on a loan based on detailed information provided at the time of loan application, as well as data on previous loan applications. Using Python libraries and a machine learning model, we achieved a prediction accuracy of 92% with an F1 score of 0.14 by applying SMOTE to balance the dataset.

Table of Contents
Project Overview
Dataset Overview
Objective
Model and Methodology
Evaluation Metrics
Results
How to Run
Dependencies
File Structure
Contributing
License
Project Overview
In this project, we use machine learning to build a binary classification model that can predict the likelihood of a loan applicant encountering payment difficulties. By analyzing key features such as loan type, demographic details, financial attributes, and previous borrowing history, the model helps in identifying high-risk clients.

Dataset Overview
The dataset comprises multiple files:

application_data_*.csv: Contains loan application information, including demographic details, loan type, and financial attributes.
previous_application.csv: Contains previous loan application records for each client, providing insights into their historical borrowing and repayment behavior.
The dataset is divided into two categories:

Clients with Payment Difficulties: Delays exceeding X days on one or more of the first Y installments.
Clients Without Payment Difficulties: Timely repayments without significant delay.
The target variable TARGET is set as:

1: Client has payment difficulties.
0: Client does not have payment difficulties.
Objective
Our goal is to predict the target variable TARGET based on the features provided in the dataset, where the model distinguishes between clients likely to experience payment difficulties and those who are not.

Model and Methodology
Data Preprocessing:

Data cleaning, handling missing values, and feature engineering.
Using SMOTE (Synthetic Minority Over-sampling Technique) to address class imbalance.
Feature Engineering:

Aggregated features from previous loan applications.
Feature scaling and transformation to optimize model performance.
Model Training:

Various machine learning models were tested, and the best-performing model was selected.
Achieved an accuracy of 92% and an F1 score of 0.14.
Evaluation Metrics
Accuracy: Measures the percentage of correct predictions.
F1 Score: Balances precision and recall, especially useful for imbalanced datasets.
Our model achieved:

Accuracy: 92%
F1 Score: 0.14
Results
The model provides a good accuracy level but a moderate F1 score, suggesting that while it is effective at overall predictions, further improvements could focus on refining recall and precision.

Dependencies
Python 3.8+
NumPy
Pandas
Scikit-learn
Imbalanced-learn
Matplotlib (for visualizations)
#you can find dataset on kaggle.
